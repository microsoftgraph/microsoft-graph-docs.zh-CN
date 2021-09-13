---
title: Windows Update for Business 部署服务中的部署
description: 部署是 Windows Update for Business 部署服务的基础。 通过部署，你可以将一组设备作为目标，以从 Windows 更新（如软件更新）接收特定内容。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 550879fed2ea694f4c7c8c9dd5470c2eeace446b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117576"
---
# <a name="deployments-in-the-windows-update-for-business-deployment-service"></a>Windows Update for Business 部署服务中的部署

部署是 Windows Update for Business 部署服务的基础。 通过部署，你可以面向一组设备，以接收来自 Windows Update 的特定内容，例如[软件更新](windowsupdates-software-updates.md)。

部署具有以下主要方面：

1. 内容：可从目录部署的更新。 这由 [deployableContent](/graph/api/resources/windowsupdates-deployablecontent)**类型的** content 属性表示。
2. 访问群体：用于接收内容的设备。 这是[deploymentAudience 类型的访问群体](/graph/api/resources/windowsupdates-deploymentaudience)关系。 
3. 设置：用于管理内容传递到设备的方式和时间的设置。 这由 [deploymentSettings](/graph/api/resources/windowsupdates-deploymentsettings)类型的 **settings** 属性表示。
4. 状态：部署在其生命周期中的当前状态。 这由 [deploymentState](/graph/api/resources/windowsupdates-deploymentstate)类型的 **state** 属性表示。

## <a name="create-a-deployment-with-content-and-an-audience"></a>创建包含内容和访问群体部署的部署


由于内容和访问群体是定义部署的关键，因此在创建时必须同时分配这两者。 尽管以后无法更改内容和访问群体分配，但访问群体中的设备成员身份可以。

若要详细了解如何创建部署，请参阅 [部署功能更新](windowsupdates-deploy-update.md) 和 [部署加速安全更新](windowsupdates-deploy-expedited-update.md)。

## <a name="configure-settings"></a>配置设置

### <a name="rollout"></a>推出

[推出](/graph/api/resources/windowsupdates-rolloutsettings) 设置控制内容在一段时间之后如何部署到部署访问群体中的设备。 你可以为部署功能更新配置推出设置。

若要了解有关推出设置的信息，请参阅计划 [部署](windowsupdates-schedule-deployment.md)。

### <a name="monitoring"></a>监控

可以使用监视 [设置](/graph/api/resources/windowsupdates-monitoringsettings) 来配置警报，并基于来自设备的更新信号自动执行操作。 可以针对功能更新的部署配置监视设置。


若要了解有关监视设置的信息，请参阅 [管理监视规则](windowsupdates-manage-monitoring-rules.md)。

### <a name="user-experience"></a>用户体验

对于快速质量更新的部署， [用户体验设置](/graph/api/resources/windowsupdates-userexperiencesettings) 会临时替代设备上现有的策略，以便获得更新体验。

若要了解有关用户体验设置的信息，请参阅 [部署加速安全更新](windowsupdates-deploy-expedited-update.md)。

## <a name="get-or-set-lifecycle-state"></a>获取或设置生命周期状态

### <a name="states"></a>状态

部署在生命周期状态中移动，如下表所述。

| 状态     | 说明                                                                                       |
|-----------|---------------------------------------------------------------------------------------------------|
| `scheduled` | 部署正在等待满足产品/服务条件，以开始向设备提供更新。 |
| `offering`  | 部署正在向设备提供更新。                                                 |
| `paused`    | 部署将暂停，并阻止向设备提供更新，直到未暂停。  |


### <a name="transitions"></a>Transitions

| Transition                     | Condition                                |
|--------------------------------|------------------------------------------|
| `scheduled` → `offering`           | 满足计划条件。             |
| `offering` → `scheduled`           | 不满足计划条件。         |
| `scheduled` 或 `offering` → `paused` | 有一个暂停的请求或自动操作。 |
| `paused` → `scheduled` 或 `offering` | 不再有要暂停的请求或自动操作。 |

### <a name="resource-model"></a>资源模型

部署 [资源](/graph/api/resources/windowsupdates-deployment)具有 [deploymentState](/graph/api/resources/windowsupdates-deploymentstate)类型的 **state** 属性，该属性提供有关当前生命周期状态的信息。

该服务确定部署 **状态** 的有效值作为多个输入和异步进程的结果，但可以通过将 **requestedValue** 设置为这些输入之一来请求特定值。 有效部署状态值的其他输入包括推出设置和监视设置。

## <a name="multiple-deployments"></a>多个部署

你可以一次将设备分配给多个部署。 这些部署可以针对相同更新类别的内容 (例如，所有部署都是功能更新) 或用于不同更新类别的内容。

为不同更新类别的内容分配设备 (例如功能更新和快速质量更新) 时，部署服务根据 Microsoft 的建议按顺序提供内容。

当您为同一更新类别 (的内容分配设备（例如，功能更新版本 20H1 和 20H2）或 2021 年 3 月和 2021 年 4 月的质量更新（从) 年 3 月到 2021 年 4 月）时，部署服务会提供 Microsoft 排名更高的内容。 对于功能更新和质量更新，最新更新的排名更高。 如果其中一个部署仍为设备计划，并且尚未准备好提供内容，则此行为不适用。 在这种情况下，其他部署将内容交付到设备。
