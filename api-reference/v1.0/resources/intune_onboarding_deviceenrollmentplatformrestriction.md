# <a name="deviceenrollmentplatformrestriction-resource-type"></a>deviceEnrollmentPlatformRestriction 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

平台特定注册限制
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|platformBlocked|Boolean|阻止平台注册|
|personalDeviceEnrollmentBlocked|Boolean|阻止个人拥有的设备注册|
|osMinimumVersion|String|支持的最小 OS 版本|
|osMaximumVersion|String|支持的最大 OS 版本|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```








