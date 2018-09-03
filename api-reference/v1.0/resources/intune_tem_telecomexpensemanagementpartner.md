# <a name="telecomexpensemanagementpartner-resource-type"></a>telecomExpenseManagementPartner 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List telecomExpenseManagementPartners](../api/intune_tem_telecomexpensemanagementpartner_list.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 集合|列出 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 对象的属性和关系。|
|[Get telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_get.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|读取 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 对象的属性和关系。|
|[Create telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_create.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|创建新的 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 对象。|
|[Delete telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_delete.md)|无|删除 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)。|
|[Update telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_update.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|更新 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|TEM 合作伙伴的唯一标识符。|
|displayName|字符串|TEM 合作伙伴的显示名称。|
|url|字符串|TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。|
|appAuthorized|布尔值|是否已授权合作伙伴的 AAD 应用访问 Intune。|
|enabled|布尔值|当前是启用还是禁用了 Intune 的 TEM 服务连接。|
|lastConnectionDateTime|DateTimeOffset|TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```



