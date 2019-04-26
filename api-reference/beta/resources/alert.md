---
title: 警报资源类型
description: 表示 Microsoft 或合作伙伴安全解决方案已确定的客户租户中的潜在安全问题。 使用警报在所有集成的解决方案中统一并优化安全问题管理。 若要了解详细信息, 请参阅 Graph 浏览器中的示例查询。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: f4bd1acfd140a4c0c4412441c92463061ecf7c86
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339102"
---
# <a name="alert-resource-type"></a>警报资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 或合作伙伴安全解决方案已确定的客户租户中的潜在安全问题。 使用警报在所有集成的解决方案中统一并优化安全问题管理。 若要了解详细信息, 请参阅[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的示例查询。

可以从[Microsoft Graph 安全概述](security-api-overview.md)中列出的不同安全提供程序中检索警报。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[获取警报](../api/alert-get.md) | [警报](alert.md) |读取 alert 对象的属性和关系。|
|[更新警报](../api/alert-update.md) | [警报](alert.md) |更新 alert 对象。 |
|[List alerts](../api/alert-list.md) | [通知](alert.md)集合 |获取一个警报对象集合。|
|[更新警报](../api/alert-updatealerts.md)|[通知](alert.md)集合|更新多个 alert 对象。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|activityGroupName|String|此警报所针对的活动组 (攻击者) 的名称或别名。|
|assignedTo|String|为会审、调查或修正分配了警报的分析员的名称 (支持[更新](../api/alert-update.md))。|
|azureSubscriptionId|String|azure 订阅 ID, 如果此警报与 Azure 资源相关, 则显示此 ID。|
|azureTenantId |String|Azure Active Directory 租户 ID。 必需。 |
|category|String|警报类别 (例如, credentialTheft、勒索软件, 等等)。|
|closedDateTime|DateTimeOffset|警报关闭的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如, 2014 年1月1日午夜 UTC 将如下所示: `'2014-01-01T00:00:00Z'` (支持[更新](../api/alert-update.md))。|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md)集合|提供程序生成的与此警报相关的云应用程序生成的与安全相关的状态信息。|
|comments|String 集合|客户提供的有关通知的注释 (针对客户通知管理) (支持[更新](../api/alert-update.md))。|
|confidence|Int32|对检测逻辑的可信度 (1-100 之间的百分比)。|
|createdDateTime |DateTimeOffset|通知提供程序创建警报的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 必需。|
|说明|字符串|通知说明。|
|detectionIds|String 集合|与此警报实体相关的一组警报 (每个警报以单独的记录的形式推送到 SIEM)。|
|eventDateTime |DateTimeOffset|触发警报 (s) 的事件发生时所发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 必需。|
|征求|alertFeedback|通知的分析师反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。 (支持[更新](../api/alert-update.md))|
|fileStates|[fileSecurityState](filesecuritystate.md)集合|提供程序生成的与安全相关的状态信息关于与此警报相关的文件。|
|historyStates|[alertHistoryState](alerthistorystate.md)集合| 由包含对警报的所有更新的审核日志的**alertHistoryStates**组成的集合。 |
|hostStates|[hostSecurityState](hostsecuritystate.md)集合|提供程序生成的与安全相关的状态信息关于与此警报相关的主机。|
|id |字符串|提供程序生成的 GUID/唯一标识符。 只读。 必需。|
|lastModifiedDateTime|DateTimeOffset|上次修改警报实体的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|malwareStates|[malwareState](malwarestate.md)集合|与此警报相关的恶意软件的威胁智能。|
|networkConnections|[networkConnection](networkconnection.md)集合|由提供程序生成的有关与此警报相关的网络连接的安全相关的状态信息。|
|进程|[过程](process.md)集合|提供程序生成的与此警报相关的进程的、与安全相关的状态信息。|
|recommendedActions|String 集合|作为警报的结果 (例如, 隔离计算机、enforce2FA、映像主机) 而要采取的供应商/提供商建议的操作。|
|registryKeyStates|[registryKeyState](registrykeystate.md)集合|提供程序生成的与安全相关的状态信息关于与此警报相关的注册表项。|
|度 |alertSeverity|警报严重性-由供应商/提供商设置。 可取值为：`unknown`、`informational`、`low`、`medium`、`high`。 必需。|
|sourceMaterials|String 集合|指向与警报相关的源材料的超链接 (uri), 例如, 提供商用于通知或日志搜索等的用户界面。|
|status |alertStatus|警报生命周期状态 (阶段)。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。 (支持[更新](../api/alert-update.md))。 必需。|
|tags|String 集合|可应用于警报并可用作筛选条件的用户可定义标签 (例如, "HVA"、"锯" 等)(支持[更新](../api/alert-update.md))。|
|title |String|通知标题。 必需。|
|触发|[alertTrigger](alerttrigger.md)集合|有关触发警报的特定属性的安全相关信息 (出现在警报中的属性)。 警报可能包含有关多个用户、主机、文件和 ip 地址的信息。 此字段指示哪些属性触发了警报生成。|
|userStates|[logonip](usersecuritystate.md)集合|提供程序生成的与此警报相关的用户帐户生成的、与安全相关的状态信息。|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息的复杂类型 (例如, 供应商 = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。 必需。|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md)集合|与此警报相关的一个或多个漏洞相关的威胁智能。|

## <a name="relationships"></a>Relationships

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "historyStates": [{"@odata.type": "microsoft.graph.alertHistoryState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
