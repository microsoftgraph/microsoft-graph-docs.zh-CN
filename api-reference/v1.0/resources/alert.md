---
title: 警报资源类型
description: 指 Microsoft 或其合作伙伴安全解决方案在客户的租户中识别的潜在安全问题。 使用警报统一并简化所有集成解决方案中的安全问题管理。 若要了解详细信息，请参阅 Graph 浏览器中的查询示例。
localization_priority: Priority
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2726eeac1a1b355a27ba45f998a463c3fc8ecbc4855c5caee9b58c8528f825f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126709"
---
# <a name="alert-resource-type"></a>警报资源类型

命名空间：microsoft.graph

指 Microsoft 或其合作伙伴安全解决方案在客户的租户中识别的潜在安全问题。 使用警报统一并简化所有集成解决方案中的安全问题管理。 若要了解详细信息，请参阅 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的查询示例。

可以从 [Microsoft Graph 安全概述](security-api-overview.md)中列出的不同安全提供程序检索警报。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[获取警报](../api/alert-get.md) | [警报](alert.md) |读取警报对象的属性和关系。|
|[更新警报](../api/alert-update.md) | [警报](alert.md) |更新警报对象。 |
|[列出警报](../api/alert-list.md) | [警报](alert.md)集合 |获取警报对象集合。|

## <a name="properties"></a>属性

| 属性             | 类型                                                         | 说明                                                                                                                                                                                                                                                                                          |
|:---------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityGroupName    | 字符串                                                       | 此警报归因于的活动组（攻击者）的名称或别名。                                                                                                                                                                                                                          |
| assignedTo           | String                                                       | 分配警报的分析员名称，用于分类、调查或修复（支持[更新](../api/alert-update.md)）。                                                                                                                                                                  |
| azureSubscriptionId  | 字符串                                                       | Azure 订阅 ID，如果此警报与 Azure 资源相关时显示。                                                                                                                                                                                                                        |
| azureTenantId        | 字符串                                                       | Azure Active Directory 租户 ID。必需。                                                                                                                                                                                                                                                          |
| “类别”             | 字符串                                                       | 警报的类别（例如，credentialTheft、ransomware 等）。                                                                                                                                                                                                                              |
| closedDateTime       | DateTimeOffset                                               | 警报关闭的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z` （支持 [更新](../api/alert-update.md)）。                    |
| cloudAppStates       | [cloudAppSecurityState](cloudappsecuritystate.md) 集合 | 提供程序生成的与此警报相关的云应用程序的安全相关状态信息。                                                                                                                                                                                 |
| comments             | 字符串集合                                            | 客户提供的警报评论（用于客户警报管理）（支持[更新](../api/alert-update.md)）。                                                                                                                                                                                     |
| confidence           | Int32                                                        | 检测逻辑的可信度（1-100 之间的百分比）。                                                                                                                                                                                                                                        |
| createdDateTime      | DateTimeOffset                                               | 警报提供程序创建警报的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 必需。                               |
| description          | String                                                       | 警报说明。                                                                                                                                                                                                                                                                                   |
| detectionIds         | 字符串集合                                            | 与此警报实体相关的警报集（每个警报作为单独的记录推送到 SIEM）。                                                                                                                                                                                                  |
| eventDateTime        | DateTimeOffset                                               | 发生用作生成警报触发器的事件的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 必需。 |
| 反馈             | alertFeedback                                                | 分析师对警报的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。 （支持[更新](../api/alert-update.md)）                                                                                                                                        |
| fileStates           | [fileSecurityState](filesecuritystate.md) 集合         | 提供程序生成的与此警报相关的文件的安全相关状态信息。                                                                                                                                                                                             |
| hostStates           | [hostSecurityState](hostsecuritystate.md) 集合         | 提供程序生成的与此警报相关的主机的安全相关状态信息。                                                                                                                                                                                             |
| id                   | String                                                       | 提供程序生成的 GUID/唯一标识符。 只读。 必填。                                                                                                                                                                                                                                      |
| incidentIds          | String collection                                            | 与当前警报相关的事件的 ID。                                                                                                                                                                                                                                                           |
| lastModifiedDateTime | DateTimeOffset                                               | 上次修改警告实体的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。                                                  |
| malwareStates        | [malwareState](malwarestate.md) 集合                   | 威胁智能，属于与此警报相关的恶意软件。                                                                                                                                                                                                                                     |
| networkConnections   | [networkConnection](networkconnection.md) 集合         | 提供程序生成的与此警报相关的网络连接的安全相关状态信息。                                                                                                                                                                               |
| processes            | [process](process.md) 集合                             | 提供程序生成的与此警报相关的流程的安全相关状态信息。                                                                                                                                                                                |
| recommendedActions   | 字符串集合                                            | 供应商/提供程序建议对警报采取的措施（例如，隔离计算机、enforce2FA、重新映像主机）。                                                                                                                                                                     |
| registryKeyStates    | [registryKeyState](registrykeystate.md) 集合           | 提供程序生成的与此警报相关的注册表项的安全相关状态信息。                                                                                                                                                                                       |
| securityResources    | [securityResource](securityResource.md) collection           | 与当前警报相关的资源。例如，对于某些警报，可能有 Azure 资源值。                                                                                                                                                                                             |
| severity             | alertSeverity                                                | 警报严重性 - 由供应商/提供程序设置。 可取值为：`unknown`、`informational`、`low`、`medium`、`high`。 必需。                                                                                                                                                                         |
| sourceMaterials      | 字符串集合                                            | 与警报相关的源材料的超链接 (URI)，例如，提供程序的警报或日志搜索的用户界面等。                                                                                                                                                                 |
| status               | alertStatus                                                  | 警告生命周期的状态（阶段）。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。 （支持[更新](../api/alert-update.md)）。 必需。                                                                                                                                         |
| 标记                 | String collection                                            | 用户可定义的标签，可应用于警报并可用作筛选条件（例如“HVA”、“SAW”等）（支持[更新](../api/alert-update.md)）。                                                                                                                               |
| title                | String                                                       | 警报标题。 必需。                                                                                                                                                                                                                                                                               |
| 触发器             | [alertTrigger](alerttrigger.md) 集合                   | 有关触发警报的特定属性的安全相关信息（警报中显示的属性）。 警报可能包含有关多个用户、主机、文件、ip 地址的信息。 此字段指示哪些属性触发警报生成。                    |
| userStates           | [userSecurityState](usersecuritystate.md) 集合         | 提供程序生成的与此警报相关的用户帐户的安全相关状态信息。                                                                                                                                                                                       |
| vendorInformation    | [securityVendorInformation](securityvendorinformation.md)    | 包含有关安全产品/服务供应商、提供程序和子提供程序的详细信息的复杂类型（例如，供应商 = Microsoft；提供程序 = Windows Defender ATP；子提供程序 = AppLocker）。必需。                                                                                                |
| vulnerabilityStates  | [vulnerabilityState](vulnerabilitystate.md) 集合       | 威胁智能，属于与此警报相关的一个或多个漏洞。                                                                                                                                                                                                                 |

## <a name="relationships"></a>关系

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
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "incidentIds": ["String"],
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "securityResources": [{"@odata.type": "microsoft.graph.securityResource"}],
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
<!-- {
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

