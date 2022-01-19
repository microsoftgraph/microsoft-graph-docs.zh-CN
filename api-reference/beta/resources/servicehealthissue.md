---
title: serviceHealthIssue 资源类型
description: 表示服务中的服务运行状况问题。
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 3588c167a895781304e14cdb88016dd6e016fccb
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072458"
---
# <a name="servicehealthissue-resource-type"></a>serviceHealthIssue 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示服务中的服务运行状况问题。

服务运行状况问题可以是服务事件或服务公告。 例如：

* 服务事件："Exchange邮箱服务关闭"。
* 服务公告："用户在接收电子邮件时可能会遇到延迟"。

继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 serviceHealthIssue](../api/servicehealthissue-get.md)|[serviceHealthIssue](../resources/servicehealthissue.md)|检索 [serviceHealthIssue](../resources/servicehealthissue.md) 对象的属性和关系。 |
|[获取事后评审报告](../api/servicehealthissue-incidentreport.md)|Stream|获取事件后报告 (PIR) 租户的指定服务问题的文档。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classification|serviceHealthClassificationType|服务运行状况问题的类型。 可取值为：`advisory`、`incident`、`unknownFutureValue`。|
|详细信息|集合 ([keyValuePair](../resources/keyvaluepair.md)) |有关服务运行状况问题的其他详细信息。 此属性不支持筛选器。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|endDateTime|DateTimeOffset|服务问题的结束时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|功能|字符串|服务问题的功能名称。|
|featureGroup|String|服务问题的功能组名称。|
|id|String|服务问题的 ID。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|impactDescription|字符串|服务问题影响的说明。|
|isResolved|布尔|指示该问题是否已解决。|
|lastModifiedDateTime|DateTimeOffset|问题的上次修改时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|origin|serviceHealthOrigin|指示服务问题的来源。 可能的值是：`microsoft`、`thirdParty`、`customer`、`unknownFutureValue`。|
|公告|collection ([serviceHealthIssuePost](../resources/servicehealthissuepost.md)) |服务问题的历史文章集合。|
|service|String|指示受问题影响的服务。|
|startDateTime|DateTimeOffset|服务问题的开始时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|状态|serviceHealthStatus|服务问题的状态。 可能的值是 `serviceOperational` `investigating` `restoringService` ：、、、、、、、、、 `verifyingService` `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` 。 有关详细信息，请参阅 [serviceHealthStatus 值](#servicehealthstatus-values)。|
|title|String|服务问题的标题。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|

### <a name="servicehealthstatus-values"></a>serviceHealthStatus 值
|成员|说明|
|:---|:---|
|serviceOperational|服务运行正常，未发现任何问题。|
|正在调查|发现了一个潜在问题，并正在收集有关所进行情况以及影响范围的信息。|
|restoringService|已识别问题的原因，并采取措施使服务恢复正常运行状态。|
|verifyingService|已采取措施来缓解问题，我们确认服务运行正常。|
|serviceRestored|更正操作已解决基础问题，并且服务已还原到正常状态。 若要了解出了什么问题，请查看问题详细信息。|
|postIncidentReviewPublished|已发布特定问题的事件后报告，其中包括根本原因信息，并采取了下一步操作以确保不会再次出现类似问题。|
|serviceDegradation|确认可能影响服务或功能使用的问题。 例如，如果服务的执行速度比平常慢、存在间歇性中断或某功能运行不正常，则可能看到此状态。|
|serviceInterruption|如果确定问题会影响用户访问服务的能力，则会看到此状态。 在本例中，问题十分重大且可持续重现。|
|extendedRecovery|此状态指示正在采取纠正措施将服务还原到大多数用户，但需要一些时间到达所有受影响的系统。 如果进行了临时修复来减少影响，而永久修复正在等待应用，则你也可能看到此状态。|
|falsePositive|经过详细调查后，服务将确认正常运行，并正常运行。 未观察到对服务的任何影响，或事件的原因源自服务之外。 具有此状态的事件和建议出现在历史视图中，直到它们过期 (在该事件最后帖子中所述的时间段之后)。|
|investigationSuspended|如果我们对潜在问题的详细调查导致请求客户提供其他信息，以允许服务团队进一步调查，你将看到此状态。 如果服务团队需要你采取行动，他们将告知你他们需要哪些数据或日志。|
|已解决|Microsoft Windows还原的服务状态对应的服务状态。|
|mitigatedExternal|与Windows对应的服务状态。|
|已缓解|与Windows恢复对应的服务状态。|
|resolvedExternal|与Windows调查挂起对应的服务状态。|
|confirmed|与Windows对应的服务状态。|
|reported|与Windows调查对应的服务状态。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssue",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "impactDescription": "String",
  "classification": "String",
  "origin": "String",
  "posts": [
    {
      "@odata.type": "microsoft.graph.serviceHealthIssuePost"
    }
  ],
  "status": "String",
  "service": "String",
  "feature": "String",
  "featureGroup": "String",
  "isResolved": "Boolean"
}
```

