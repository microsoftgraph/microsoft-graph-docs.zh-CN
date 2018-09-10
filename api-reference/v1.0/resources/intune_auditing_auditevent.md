# <a name="auditevent-resource-type"></a>auditEvent 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含审核事件的属性的类。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 auditEvents](../api/intune_auditing_auditevent_list.md)|[auditEvent](../resources/intune_auditing_auditevent.md) 集合|列出 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性和关系。|
|[获取 auditEvent](../api/intune_auditing_auditevent_get.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|读取 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性和关系。|
|[创建 auditEvent](../api/intune_auditing_auditevent_create.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|创建新的 [auditEvent](../resources/intune_auditing_auditevent.md) 对象。|
|[删除 auditEvent](../api/intune_auditing_auditevent_delete.md)|无|删除 [auditEvent](../resources/intune_auditing_auditevent.md)。|
|[更新 auditEvent](../api/intune_auditing_auditevent_update.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|更新 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性。|
|[getAuditCategories 函数](../api/intune_auditing_auditevent_getauditcategories.md)|字符串集合|尚未记录|
|[getAuditActivityTypes 函数](../api/intune_auditing_auditevent_getauditactivitytypes.md)|字符串集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。|
|displayName|字符串|事件显示名称。|
|componentName|字符串|组件名称。|
|执行人|[auditActor](../resources/intune_auditing_auditactor.md)|与审核事件关联的 AAD 用户和应用程序。|
|活动|字符串|活动的友好名称。|
|activityDateTime|DateTimeOffset|执行活动时的日期时间（UTC 时间）。|
|activityType|字符串|执行的活动类型。|
|activityOperationType|字符串|活动的 HTTP 操作类型。|
|activityResult|字符串|活动结果。|
|correlationId|全局唯一标识符|用于关联系统内的活动的客户端请求 ID。|
|资源|[auditResource](../resources/intune_auditing_auditresource.md) 集合|正在修改的资源。|
|分类|字符串|审核类别。|

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








