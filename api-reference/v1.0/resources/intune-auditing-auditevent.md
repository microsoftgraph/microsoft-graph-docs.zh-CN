---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a97d5a0f2c3febf242c358679fb3c3551afedaab
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60453335"
---
# <a name="auditevent-resource-type"></a>auditEvent 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含审核事件的属性的类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 auditEvents](../api/intune-auditing-auditevent-list.md)|[auditEvent](../resources/intune-auditing-auditevent.md) 集合|列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。|
|[获取 auditEvent](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。|
|[创建 auditEvent](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。|
|[删除 auditEvent](../api/intune-auditing-auditevent-delete.md)|无|删除 [auditEvent](../resources/intune-auditing-auditevent.md)。|
|[更新 auditEvent](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。|
|[getAuditCategories 函数](../api/intune-auditing-auditevent-getauditcategories.md)|String collection|尚未记录|
|[getAuditActivityTypes 函数](../api/intune-auditing-auditevent-getauditactivitytypes.md)|String collection|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|事件显示名称。|
|componentName|String|组件名称。|
|actor|[auditActor](../resources/intune-auditing-auditactor.md)|与审核事件关联的 AAD 用户和应用程序。|
|activity|String|活动的友好名称。|
|activityDateTime|DateTimeOffset|执行活动时的日期时间（UTC 时间）。|
|activityType|String|执行的活动类型。|
|activityOperationType|String|活动的 HTTP 操作类型。|
|activityResult|String|活动结果。|
|correlationId|Guid|用于关联系统内的活动的客户端请求 ID。|
|resources|[auditResource](../resources/intune-auditing-auditresource.md) 集合|正在修改的资源。|
|“类别”|String|审核类别。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```



