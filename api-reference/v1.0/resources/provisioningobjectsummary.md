---
title: provisioningObjectSummary 资源类型
description: 表示 Azure AD 预配服务及其关联属性执行的操作。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d9852745ed14cacd47389da5031cb83af306e2d0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241494"
---
# <a name="provisioningobjectsummary-resource-type"></a>provisioningObjectSummary 资源类型

命名空间：microsoft.graph


表示 Azure AD 预配服务及其关联属性执行的操作。 

## <a name="methods"></a>方法

| 方法  | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 provisioningObjectSummary](../api/provisioningobjectsummary-list.md) | [provisioningObjectSummary](provisioningobjectsummary.md) | 获取租户中发生的所有预配事件的列表。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|provisioningAction|provisioningAction|指示活动名称或操作名称。 可能的值是 `create` `update` `delete` ：、、、、 `stageddelete` `disable` 和 `other` `unknownFutureValue` 。 有关记录的活动列表，请参阅 Azure AD 活动列表。|
|activityDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|changeId|String|此周期中此更改的唯一 ID。|
|cycleId|String|每个作业迭代的唯一 ID。|
|durationInMilliseconds|Int32|指示完成此预配操作所需要的时间。 以毫秒为单位。|
|id|String| 指示活动的唯一 ID。 这是只读 GUID。|
|initiatedBy|[initiator](initiator.md)|此预配的发起人的详细信息。|
|jobId|String|整个预配作业的唯一 ID。|
|ModifiedProperties|[modifiedProperty](modifiedproperty.md) 集合|在此对象的此设置操作中修改的每个属性的详细信息。|
|provisioningSteps|[provisioningStep](provisioningstep.md) 集合|预配中每个步骤的详细信息。|
|servicePrincipal|[servicePrincipal](provisioningserviceprincipal.md) 集合|表示用于设置的服务主体。|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|要预配的源对象的详细信息。|
|sourceSystem|[provisioningSystem](provisioningsystem.md)|要设置的对象的源系统的详细信息。|
|provisioningStatusInfo|[provisioningStatusInfo](provisioningstatusinfo.md)|设置状态的详细信息。|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|正在设置的目标对象的详细信息。|
|targetSystem|[provisioningSystem](provisioningsystem.md)|要设置的对象的目标系统的详细信息。|
|tenantId|String|唯一的 Azure AD 租户 ID。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "provisioningAction":  "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "provisioningStatusInfo": {"@odata.type": "microsoft.graph.provisioningStatusInfo"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


