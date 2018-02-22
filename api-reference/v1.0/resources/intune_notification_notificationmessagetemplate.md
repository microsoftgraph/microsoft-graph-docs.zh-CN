# <a name="notificationmessagetemplate-resource-type"></a>notificationMessageTemplate 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。 管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List notificationMessageTemplates](../api/intune_notification_notificationmessagetemplate_list.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 集合|列出 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象的属性和关系。|
|[Get notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_get.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|读取 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象的属性和关系。|
|[创建 notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_create.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|创建新的 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象。|
|[Delete notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_delete.md)|无|删除 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)。|
|[Update notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_update.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|更新 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象的属性。|
|[sendTestMessage 操作](../api/intune_notification_notificationmessagetemplate_sendtestmessage.md)|无|使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|String|通知消息模板的显示名称。|
|defaultLocale|String|请求的区域设置不可用时要回退到的默认区域设置。|
|brandingOptions|String|消息模板品牌选项。 已在 Intune 管理员控制台中定义品牌。 可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) 集合|此通知消息模板的本地化消息列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```



