# <a name="user-resource-type"></a>用户资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List users](../api/intune_onboarding_user_list.md)|[user](../resources/intune_onboarding_user.md) 集合|列出 [user](../resources/intune_onboarding_user.md) 对象的属性和关系。|
|[获取 user](../api/intune_onboarding_user_get.md)|[user](../resources/intune_onboarding_user.md)|读取 [user](../resources/intune_onboarding_user.md) 对象的属性和关系。|
|[创建 user](../api/intune_onboarding_user_create.md)|[user](../resources/intune_onboarding_user.md)|创建新的 [user](../resources/intune_onboarding_user.md) 对象。|
|[删除 user](../api/intune_onboarding_user_delete.md)|无|删除 [user](../resources/intune_onboarding_user.md)。|
|[更新 user](../api/intune_onboarding_user_update.md)|[user](../resources/intune_onboarding_user.md)|更新 [user](../resources/intune_onboarding_user.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户的唯一标识符。|
|deviceEnrollmentLimit|Int32|允许用户注册的最大设备数的限制。 允许的值为 5 或 1000。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```



