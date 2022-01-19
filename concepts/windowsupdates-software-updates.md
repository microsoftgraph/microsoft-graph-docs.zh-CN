---
title: Windows Update for Business 部署服务的软件更新
description: 软件更新是部署服务部署的主要内容类型。 您可以在目录中查找以查找可部署的特定更新。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 3f3dd0a1da1c6426c8415fe3c6f37767d1613627
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072234"
---
# <a name="software-updates-with-the-windows-update-for-business-deployment-service"></a>Windows Update for Business 部署服务的软件更新

软件更新是部署服务部署的主要内容类型。 您可以在目录中查找以查找可部署的特定更新。

您可能已经熟悉 Microsoft[更新目录，](https://www.catalog.update.microsoft.com/)该目录列出了 Windows。 部署服务提供自己的 [目录](/graph/api/resources/windowsupdates-catalog)，并聚合单个 [catalogEntry](/graph/api/resources/windowsupdates-catalogentry) 下的等效更新，以简化决策制定和审批工作流。

## <a name="windows-update-categories"></a>Windows 更新类别

通常，有两种高级类别的Windows 10更新：功能更新和质量更新。 属于质量更新类别包括安全更新、驱动程序更新和其他更新。

部署服务 [目录还将](/graph/api/resources/windowsupdates-catalog?view=graph-rest-beta&preserve-view=true) 更新分类为功能和质量更新。 [质量更新目录条目](/graph/api/resources/windowsupdates-qualityupdatecatalogentry?view=graph-rest-beta&preserve-view=true) 以特定方式定义安全更新和非安全更新，并排除驱动程序更新。 请注意，该定义不同于 Microsoft 更新目录。 有关详细信息 [，请参阅](#quality-updates) 下面的质量更新。

实际上，部署服务当前仅部署在其目录中定义的功能更新和安全质量更新。 该服务当前不部署非安全质量更新或驱动程序更新。

若要了解有关更新Windows 10服务的信息，请参阅快速[指南Windows 即服务。](/windows/deployment/update/waas-quick-start)

## <a name="identifying-updates-for-deployment"></a>确定部署的更新

Microsoft 更新目录中的更新非常具体，特定于各个产品、版本和 CPU 体系结构。 

例如，以下两个安全质量更新在 Microsoft 更新目录中被视为不同的版本，尽管它们仅因体系结构不同而不同。

| Title                                                                                   | 产品                           | 分类   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| 基于 **x86** 的系统的 Windows 10 版本 20H2 的 2021-03 累积 (KB5000802)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 **x64** 的系统的 Windows 10 版本 20H2 的 2021-03 累积 (KB5000802)  | Windows 10 版本 1903 和更高版本： | 安全更新 |

在 Windows Update for Business 部署服务提供的目录中，这些更新聚合到单个条目中。

| 显示名称                                           | 类型                                                     |
|--------------------------------------------------------|----------------------------------------------------------|
| 03/09/2021 - 2021.03 B Windows 10 | microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry |

此聚合简化了跨不同安装群批准更新的过程。 同样，部署服务会汇总功能更新版本。

### <a name="common-properties"></a>通用属性

部署服务目录中的所有更新都具有以下通用属性。

| 属性                | 说明                                                        |
|-------------------------|--------------------------------------------------------------------|
| id                      | 目录项的唯一标识符。                           |
| displayName             | 软件更新的标题。                                      |
| releaseDateTime         | 发布或刷新更新的日期和时间。                |
| deployableUntilDateTime | 无法再部署更新的日期和时间（如果已知）。|

### <a name="feature-updates"></a>功能更新

部署服务目录中的功能更新由版本标识。 条目聚合了体系结构 (例如，x86 与 x64) 以及 Microsoft 更新目录中的产品 (，所有功能更新均针对 Windows 10 *产品*) 。

| 属性 | 说明                                       |
|----------|---------------------------------------------------|
| version  | Windows 10 版本的功能更新版本。|

下面是部署服务目录中功能更新的一些示例。

| 显示名称                               | 版本 |
|--------------------------------------------|---------|
| 功能更新到 Windows 10 20H1 版本 | 20H1    |
| 功能更新到 Windows 10 版本 1909 | 1909    |
| 功能更新到 Windows 10 版本 1903 | 1903    |
| 要更新的功能Windows 10 版本 1809 | 1809    |

确定所需版本后，使用 [featureUpdateReference](/graph/api/resources/windowsupdates-featureupdatereference) 并指定 **version** 属性将其作为内容分配给部署。

### <a name="quality-updates"></a>质量更新

部署服务目录中的质量更新由发布日期/时间和更新分类标识。 条目聚合体系结构、产品 (（例如 *Windows 10、版本 1903* 及更高版本与 *Windows 10* 与 *Windows 10 LTSB) ）* 以及相应功能更新版本之间的差异。

| 属性 | 说明 |
|----------|-------------|
| classification | 分类 (更新的安全性) 或非安全性。 |
| releaseDateTime | 发布或刷新更新的日期和时间。 |

下表显示了部署服务目录和 Microsoft 更新目录之间的分类映射。

| 部署服务目录 | Microsoft 更新目录                                                                                                               |
|------------------|--------------------------------------------------------------------------------------------------------------------------------|
| 安全性         | 安全更新<br>关键更新<br>如果需要 (依赖项，请更新) <br>如果需要， (堆栈更新作为依赖项进行)  |
| 非安全性     | 更新<br>服务堆栈更新                                                                                               |

与部署服务目录中的质量更新相对应的 Microsoft 更新目录中的条目和 `classification = security` `releaseDateTime = 2021-03-09` 可能包括以下内容。

| Title                                                                                   | 产品                           | 分类   |
|-----------------------------------------------------------------------------------------|------------------------------------|------------------|
| 基于 x86 的系统 2021-03 Windows 10 20H2 累积更新 (KB5000802)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 x64 的系统 2021-03 Windows 10 20H2 累积更新 (KB5000802)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 x86 的系统版本 1909 的 Windows 10 2021-03 年累积更新 (KB5000808)  | Windows 10 版本 1903 和更高版本： | 安全更新 |
| 基于 x64 的系统版本 1809 的 Windows 10 2021-03 累积更新 (KB5000822)  | Windows 10、Windows 10 LTSB        | 安全更新 |

确定所需更新后，使用 [qualityUpdateReference](/graph/api/resources/windowsupdates-qualityupdatereference) 并将其指定为部署的内容并指定 **releaseDateTime** 和 **classification** 属性。

## <a name="examples"></a>示例

若要查看列出 [目录条目的示例，](/graph/api/windowsupdates-catalog-list-entries)请参阅 [部署功能更新](windowsupdates-deploy-update.md) 和 [部署加速安全更新](windowsupdates-deploy-expedited-update.md)。