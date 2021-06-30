---
title: cloudPcAuditEvent 资源类型
description: 表示审核事件实体。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a863ea4128b7383c70bd14f025fcc5ce116dda25
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211223"
---
# <a name="cloudpcauditevent-resource-type"></a>cloudPcAuditEvent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示审核事件实体。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 auditEvents](../api/virtualendpoint-list-auditevents.md)|[cloudPcAuditEvent](../resources/cloudpcauditevent.md) 集合|列出租户 [中所有 cloudPcAuditEvent](../resources/cloudpcauditevent.md) 对象。|
|[获取 cloudPcAuditEvent](../api/cloudpcauditevent-get.md)|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|读取 [cloudPcAuditEvent 对象的属性和](../resources/cloudpcauditevent.md) 关系。|
|[getAuditActivityTypes 函数](../api/cloudpcauditevent-getauditactivitytypes.md)|String collection|获取审核活动类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|审核实体的键。 只读。|
|displayName|String|事件显示名称。 只读。|
|componentName|String|组件名称。 只读。|
|actor|[cloudPcAuditActor](../resources/cloudpcauditactor.md)|与审核事件关联的 Azure AD 用户和应用程序。 只读。|
|activity|String|活动的友好名称。可选。|
|activityDateTime|DateTimeOffset|执行活动时的日期时间（UTC 时间）。只读。|
|activityType|String|执行的活动类型。只读。|
|activityOperationType|[cloudPcAuditActivityOperationType](#cloudpcauditactivityoperationtype-values)|活动的 HTTP 操作类型。 可能的值包括  `create` 、 `delete` 和 `patch` `other` 。 只读。|
|activityResult|[cloudPcAuditActivityResult](#cloudpcauditactivityresult-values)|活动结果。只读。|
|correlationId|String|客户端请求标识符，用于关联系统内的活动。只读。|
|resources|[cloudPcAuditResource](../resources/cloudpcauditresource.md) 集合|cloudPcAuditResource 对象的列表。只读。|
|“类别”|[cloudPcAuditCategory](#cloudpcauditcategory-values)|审核类别。 只读。|

### <a name="cloudpcauditactivityoperationtype-values"></a>cloudPcAuditActivityOperationType 值

|成员|说明|
|:---|:---|
|create|创建操作。|
|delete|删除操作。|
|patch|修补程序操作。|
|other|其他操作。|

### <a name="cloudpcauditactivityresult-values"></a>cloudPcAuditActivityResult 值

|成员|说明|
|:---|:---|
|success|操作成功。|
|clientError|操作失败，出现客户端错误。|
|failure|操作失败。|
|timeExceeded|操作失败，超时。|
|other|其他结果。|

### <a name="cloudpcauditcategory-values"></a>cloudPcAuditCategory 值

|成员|说明|
|:---|:---|
|cloudPC|云电脑类别。|
|other |其他类别。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.cloudPcAuditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ],
    "remoteTenantId": "String",
    "remoteUserId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditProperty",
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
