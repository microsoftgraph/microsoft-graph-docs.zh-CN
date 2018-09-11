# <a name="auditactor-resource-type"></a>auditActor 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含审核主角的属性的类。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|类型|字符串|主角类型。|
|userPermissions|String 集合|执行审核时的用户权限列表。|
|applicationId|字符串|AAD 应用程序 ID。|
|applicationDisplayName|字符串|应用程序的名称。|
|userPrincipalName|字符串|用户主体名称 (UPN)。|
|servicePrincipalName|字符串|服务主体名称 (SPN)。|
|ipAddress|字符串|IPAddress。|
|userId|字符串|用户 ID。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
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
}
```








