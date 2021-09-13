---
title: serviceHealthIssue 资源类型
description: 表示服务中的服务运行状况问题。
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b794284a4dafe16061faa5e84af9e72755d1f6b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019109"
---
# <a name="servicehealthissue-resource-type"></a>serviceHealthIssue 资源类型

命名空间：microsoft.graph

表示服务中的服务运行状况问题。

服务运行状况问题可以是服务事件或服务公告。 例如：

* 服务事件："Exchange邮箱服务关闭"。
* 服务公告："用户在接收电子邮件时可能会遇到延迟"。

继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 serviceHealthIssue](../api/servicehealthissue-get.md)|[serviceHealthIssue](../resources/servicehealthissue.md)|检索 [serviceHealthIssue](../resources/servicehealthissue.md) 对象的属性和关系。 |
|[获取事后评审报告](../api/servicehealthissue-incidentreport.md)|Stream|提供事件后报告 (PIR) 租户的指定服务问题的文档。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classification|serviceHealthClassificationType|服务运行状况问题的类型。 可取值为：`advisory`、`incident`、`unknownFutureValue`。|
|详细信息|collection ([keyValuePair](../resources/keyvaluepair.md)) |有关服务运行状况问题的其他详细信息。 此属性不支持筛选器。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|endDateTime|DateTimeOffset|服务问题的结束时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|功能|String|服务问题的功能名称。|
|featureGroup|String|服务问题的功能组名称。|
|id|String|服务问题的 ID。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|impactDescription|String|服务问题影响的说明。|
|isResolved|Boolean|指示该问题是否已解决。|
|lastModifiedDateTime|DateTimeOffset|问题的上次修改时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|origin|serviceHealthOrigin|指示服务问题的来源。 可取值为：`microsoft`、`thirdParty`、`customer`、`unknownFutureValue`。|
|公告|collection ([serviceHealthIssuePost](../resources/servicehealthissuepost.md)) |服务问题的历史文章集合。|
|service|String|指示受问题影响的服务。|
|startDateTime|DateTimeOffset|服务问题的开始时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|status|serviceHealthStatus|服务问题的状态。 可能的值是 `serviceOperational` `investigating` `restoringService` ：、、、、、、、、、 `verifyingService` `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` 。|
|title|String|服务问题的标题。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|

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

