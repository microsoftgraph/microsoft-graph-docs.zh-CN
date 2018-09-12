# <a name="reportroot-resource-type"></a>reportRoot 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示一个历史记录报告实例的资源。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 reportRoot](../api/intune_shared_reportroot_get.md)|[reportRoot](../resources/intune_shared_reportroot.md)|读取 [reportRoot](../resources/intune_shared_reportroot.md) 对象的属性和关系。|
|[更新 reportRoot](../api/intune_shared_reportroot_update.md)|[reportRoot](../resources/intune_shared_reportroot.md)|更新 [reportRoot](../resources/intune_shared_reportroot.md) 对象的属性。|
|**设备配置**|
|[deviceConfigurationDeviceActivity 函数](../api/intune_shared_reportroot_deviceconfigurationdeviceactivity.md)|[report](../resources/intune_shared_report.md)|设备配置设备活动报告的元数据|
|[deviceConfigurationUserActivity 函数](../api/intune_shared_reportroot_deviceconfigurationuseractivity.md)|[report](../resources/intune_shared_report.md)|设备配置用户活动报告的元数据|
|**疑难解答**|
|[managedDeviceEnrollmentFailureDetails function](../api/intune_shared_reportroot_manageddeviceenrollmentfailuredetails.md)|[report](../resources/intune_shared_report.md)|尚未编档。|
|[managedDeviceEnrollmentTopFailures 函数](../api/intune_shared_reportroot_manageddeviceenrollmenttopfailures.md)|[report](../resources/intune_shared_report.md)|尚未编档。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|此实体的唯一标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>示例

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```