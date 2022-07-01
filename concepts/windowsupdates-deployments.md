---
title: 适用于企业的 Windows 更新部署服务中的部署
description: 使用 Windows 更新 for Business 部署服务创建部署、配置设置和设置生命周期状态。 将设备分配到多个部署。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 38165c5f4da09e97102cb3a7f6bc9e26c9f60ff6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437511"
---
# <a name="deployments-in-the-windows-update-for-business-deployment-service"></a>适用于企业的 Windows 更新部署服务中的部署

部署是业务部署服务Windows 更新的基础。 通过部署，可以针对一组设备从Windows 更新接收特定内容，例如[软件更新](windowsupdates-software-updates.md)。

部署具有以下关键方面：

1. 内容：可从目录部署的更新。 这由 [deployableContent](/graph/api/resources/windowsupdates-deployablecontent) 类型的 **内容** 属性表示。
2. 受众：要接收内容的设备。 这是 [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) 类型的 **受众** 关系。
3. 设置：控制内容应如何以及何时传递到设备的设置。 这由 [deploymentSettings](/graph/api/resources/windowsupdates-deploymentsettings) 类型的 **settings** 属性表示。
4. 状态：部署在其生命周期内的当前状态。 这由 [deploymentState](/graph/api/resources/windowsupdates-deploymentstate) 类型的 **状态** 属性表示。

## <a name="create-a-deployment-with-content-and-an-audience"></a>创建包含内容和受众的部署

由于内容和受众是部署定义的关键，因此需要在创建时同时分配这两项内容。 虽然以后无法更改内容和受众分配，但受众中的设备成员身份可以更改。

若要详细了解如何创建部署，请参阅 [“部署功能更新](windowsupdates-deploy-update.md) ”和 [“部署加速安全更新](windowsupdates-deploy-expedited-update.md)”。

## <a name="configure-settings"></a>配置设置

### <a name="rollout"></a>推出

[推出设置](/graph/api/resources/windowsupdates-rolloutsettings) 控制内容随时间推移部署到部署受众中的设备的方式。 可以为功能更新的部署配置推出设置。

若要了解有关推出设置的详细信息，请参阅 [计划部署](windowsupdates-schedule-deployment.md)。

### <a name="monitoring"></a>监控

可以使用 [监视设置](/graph/api/resources/windowsupdates-monitoringsettings) 来配置警报和自动操作，以根据来自设备的更新信号执行。 可以为功能更新的部署配置监视设置。


若要详细了解监视设置，请参阅 [“管理监视规则](windowsupdates-manage-monitoring-rules.md)”。

### <a name="user-experience"></a>用户体验

对于加速质量更新的部署， [用户体验设置](/graph/api/resources/windowsupdates-userexperiencesettings) 会暂时覆盖设备上的现有策略以获得更新体验。

若要详细了解用户体验设置，请 [参阅部署加速的安全更新](windowsupdates-deploy-expedited-update.md)。

## <a name="get-or-set-lifecycle-state"></a>获取或设置生命周期状态

### <a name="states"></a>状态

按照下表所述，部署在生命周期状态中移动。

| 状态       | 说明                                                                                       |
|-------------|---------------------------------------------------------------------------------------------------|
| `scheduled` | 部署正在等待满足产品/服务条件，以开始向设备提供更新。 |
| `offering`  | 部署向设备提供更新。                                                 |
| `paused`    | 部署暂停，并阻止向设备提供更新，直到未暂停。  |
| `faulted`   | 由于服务无法解析的原因，部署未向设备提供更新。  |


### <a name="transitions"></a>Transitions

| Transition                           | 条件                                |
|--------------------------------------|------------------------------------------|
| `scheduled` → `offering`             | 满足计划条件。             |
| `offering` → `scheduled`             | 未满足计划条件。         |
| `scheduled` 或 `offering` → `paused` | 有一个请求或自动操作要暂停。 |
| `paused``scheduled`→或`offering` | 不再有要暂停的请求或自动操作。 |
| `offering`、 `scheduled`或 `paused` → `faulted` | 存在服务无法解析的错误。 |

### <a name="resource-model"></a>资源模型

[部署](/graph/api/resources/windowsupdates-deployment)资源具有 [deploymentState](/graph/api/resources/windowsupdates-deploymentstate) 类型的 **状态** 属性，该属性提供有关当前生命周期状态的信息。

该服务将部署状态的有效 **值** 确定为多个输入和异步进程的最终结果，但可以通过将 **requestValue** 设置为其中一个输入来请求特定值。 对有效部署状态值的其他输入包括推出设置和监视设置。

## <a name="assign-a-device-to-multiple-deployments"></a>将设备分配到多个部署

可以一次将设备分配到多个部署。 这些部署可以用于同一更新类别的内容 (例如，所有部署都是功能更新) 或不同更新类别的内容。

为不同更新类别的内容（例如，功能更新和加速质量更新 () ）分配设备到两个部署时，部署服务会根据 Microsoft 的建议按顺序提供内容。

将设备分配到同一更新类别内容的两个部署 (例如，功能更新版本 20H1 和 20H2，或 2021 年 3 月和 2021 年 4 月) 的质量更新时，部署服务提供 Microsoft 排名较高的内容。 对于功能更新和质量更新，最近的更新排名较高。 如果其中一个部署仍为设备计划并且尚未准备好提供内容，则此行为不适用。 在这种情况下，其他部署会将内容传送到设备。
