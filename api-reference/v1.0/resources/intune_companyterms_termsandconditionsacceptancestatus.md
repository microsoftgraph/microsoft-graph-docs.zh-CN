# <a name="termsandconditionsacceptancestatus-resource-type"></a>termsAndConditionsAcceptanceStatus 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List termsAndConditionsAcceptanceStatuses](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 集合|列出 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的属性和关系。|
|[Get termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|读取 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的属性和关系。|
|[Create termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象。|
|[Delete termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|无|删除 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)。|
|[Update termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|更新 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符。|
|userDisplayName|String|实体所表示的接受状态所属用户的显示名称。|
|acceptedVersion|Int32|用户所接受的最新 T&C 版本号。|
|acceptedDateTime|DateTimeOffset|用户上次接受条款时的日期/时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|所分配的条款和条件的导航链接。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



