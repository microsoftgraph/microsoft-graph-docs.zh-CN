# <a name="windowsinformationprotectionapplockerfile-resource-type"></a>windowsInformationProtectionAppLockerFile 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 信息保护 AppLocker 文件
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsInformationProtectionAppLockerFiles](../api/intune_mam_windowsinformationprotectionapplockerfile_list.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 集合|列出 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象的属性和关系。|
|[获取 windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_get.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|读取 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象的属性和关系。|
|[创建 windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_create.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象。|
|[删除 windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_delete.md)|无|删除 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)。|
|[更新 windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_update.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|更新 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|友好名称|
|fileHash|String|文件的 SHA256 哈希|
|file|Binary|字节数组形式的文件|
|id|String|实体的键。|
|version|String|实体版本。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "String",
  "fileHash": "String",
  "file": "binary",
  "id": "String (identifier)",
  "version": "String"
}
```



