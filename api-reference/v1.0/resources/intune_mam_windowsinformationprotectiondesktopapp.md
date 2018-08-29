# <a name="windowsinformationprotectiondesktopapp-resource-type"></a>windowsInformationProtectionDesktopApp 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于 Windows 信息保护的桌面应用

继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|应用显示名称。 继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|description|String|应用的说明。 继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|publisherName|String|继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 的发布者名称|
|productName|String|产品名称。 继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|denied|Boolean|如果为 true，则应用的保护或免除受到拒绝。 继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|binaryName|String|二进制名称。|
|binaryVersionLow|String|较低的二进制版本。|
|binaryVersionHigh|String|较高的二进制版本。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsInformationProtectionApp",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



