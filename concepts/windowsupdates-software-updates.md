---
title: 使用 Windows 更新 for Business 部署服务进行软件更新
description: 软件更新是部署服务部署的主要内容类型。 可以在目录中查找可用于部署的特定更新。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 206fe1fd09caacbf4db8715104fba54eefd9e113
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437392"
---
# <a name="software-updates-with-the-windows-update-for-business-deployment-service"></a>使用 Windows 更新 for Business 部署服务进行软件更新

软件更新是部署服务部署的主要内容类型。 可以在目录中查找可用于部署的特定更新。

你可能已经熟悉 [Microsoft 更新目录](https://www.catalog.update.microsoft.com/)，其中列出了 Windows 的软件更新。 部署服务提供自己的 [目录](/graph/api/resources/windowsupdates-catalog)，并在单个 [catalogEntry](/graph/api/resources/windowsupdates-catalogentry) 下聚合等效更新，以简化决策和审批工作流。

## <a name="windows-update-categories"></a>Windows 更新类别

通常，有两个高级类别的Windows 10更新：功能更新和质量更新。 属于质量更新类别包括安全更新、驱动程序更新和其他内容。

部署服务 [目录](/graph/api/resources/windowsupdates-catalog?view=graph-rest-beta&preserve-view=true) 还会将更新分类为功能和质量更新。 [质量更新目录条目](/graph/api/resources/windowsupdates-qualityupdatecatalogentry?view=graph-rest-beta&preserve-view=true) 以特定的方式定义安全和非安全更新，并排除驱动程序更新。 请注意，该定义与 Microsoft 更新目录不同。 有关更多详细信息，请参阅下面 [的质量更新](#quality-updates) 。

实际上，部署服务当前仅部署其目录中定义的功能更新 _和安全_ 质量更新。 该服务当前不部署非安全质量更新或驱动程序更新。

若要详细了解Windows 10更新和服务，请参阅[快速Windows 即服务指南](/windows/deployment/update/waas-quick-start)。

## <a name="identifying-updates-for-deployment"></a>标识部署更新

Microsoft 更新目录中的更新非常精细，特定于单个产品、版本和 CPU 体系结构。 

例如，以下两个安全质量更新在 Microsoft 更新目录中被视为不同的版本，尽管它们仅因体系结构而异。

| Title                                                                                   | 产品                           | 分类   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| 基于 **x86** 的系统 (KB5000802 的 Windows 10 版本 20H2 的 2021-03 累积更新)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 **x64** 的系统Windows 10版本 20H2 的 2021-03 累积更新 (KB5000802)  | Windows 10 版本 1903 和更高版本： | 安全更新 |

在由 Windows 更新 for Business 部署服务提供的目录中，这些更新聚合到单个条目中。

| 显示名称                                           | 类型                                                     |
|--------------------------------------------------------|----------------------------------------------------------|
| 2021/03/09 - 2021.03 B 安全更新，适用于Windows 10 | microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry |

此聚合简化了跨不同安装的基础批准更新的过程。 同样，部署服务也会汇总功能更新版本。

### <a name="common-properties"></a>通用属性

部署服务目录中的所有更新都具有以下常见属性。

| 属性                | 说明                                                        |
|-------------------------|--------------------------------------------------------------------|
| id                      | 目录条目的唯一标识符。                           |
| displayName             | 软件更新的标题。                                      |
| releaseDateTime         | 发布或刷新更新的日期和时间。                |
| deployableUntilDateTime | 无法再部署更新的日期和时间（如果已知）。|

### <a name="feature-updates"></a>功能更新

部署服务目录中的功能更新按版本标识。 条目聚合了体系结构 (（例如 x86 与 x64) 和 Microsoft 更新目录中的产品 (）之间的差异，所有功能更新都适用于 *Windows 10* 产品) 。

| 属性 | 说明                                       |
|----------|---------------------------------------------------|
| version  | Windows 10版本的功能更新版本。|

下面是部署服务目录中功能更新的一些示例。

| 显示名称                               | 版本 |
|--------------------------------------------|---------|
| Windows 10版本 20H1 的功能更新 | 20H1    |
| 功能更新到 Windows 10 版本 1909 | 1909    |
| 功能更新到 Windows 10 版本 1903 | 1903    |
| 功能更新到Windows 10 版本 1809 | 1809    |

标识所需版本后，使用 [featureUpdateReference](/graph/api/resources/windowsupdates-featureupdatereference) 将其作为内容分配到部署，并指定 **版本** 属性。

### <a name="quality-updates"></a>质量更新

部署服务目录中的质量更新由发布日期/时间和更新分类进行标识。 条目聚合了体系结构、产品 (（例如 *Windows 10、版本 1903 及更高版本* 与 *Windows 10* 与 *Windows 10 LTSB*) ）以及相应的功能更新版本之间的差异。

| 属性 | 说明 |
|----------|-------------|
| classification | 分类 (质量更新的安全性或非安全性) 。 |
| releaseDateTime | 发布或刷新更新的日期和时间。 |

下表显示了部署服务目录和 Microsoft 更新目录之间的分类映射。

| 部署服务目录 | Microsoft 更新目录                                                                                                               |
|------------------|--------------------------------------------------------------------------------------------------------------------------------|
| 安全性         | 安全更新<br>关键更新<br>根据需要更新 (作为依赖项) <br>服务堆栈更新 (（如果需要）作为依赖项)  |
| 非安全性     | 更新<br>服务堆栈更新                                                                                               |

Microsoft 更新目录中与`classification = security``releaseDateTime = 2021-03-09`部署服务目录中的质量更新相对应的条目，其中可能包括以下内容。

| Title                                                                                   | 产品                           | 分类   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| 基于 x86 的系统 (KB5000802 的 Windows 10 版本 20H2 的 2021-03 累积更新)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 x64 的系统Windows 10版本 20H2 的 2021-03 累积更新 (KB5000802)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 x86 的系统Windows 10版本 1909 的 2021-03 累积更新 (KB5000808)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 x64 的系统的 Windows 10 版本 1809 的 2021-03 累积更新 (KB5000822)  | Windows 10、Windows 10 LTSB        | 安全更新 |

确定所需更新后，使用 [qualityUpdateReference](/graph/api/resources/windowsupdates-qualityupdatereference) 将其作为内容分配到部署，并指定 **releaseDateTime** 和 **分类** 属性。

## <a name="examples"></a>示例

若要查看 [列出目录条目的](/graph/api/windowsupdates-catalog-list-entries)示例，请 [参阅部署功能更新](windowsupdates-deploy-update.md) 并 [部署加速的安全更新](windowsupdates-deploy-expedited-update.md)。
