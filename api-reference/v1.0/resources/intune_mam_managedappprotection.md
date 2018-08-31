# <a name="managedappprotection-resource-type"></a>managedAppProtection 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于为指定的一组应用配置详细管理设置的策略

继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppProtections](../api/intune_mam_managedappprotection_list.md)|[managedAppProtection](../resources/intune_mam_managedappprotection.md) 集合|列出 [managedAppProtection](../resources/intune_mam_managedappprotection.md) 对象的属性和关系。|
|[Get managedAppProtection](../api/intune_mam_managedappprotection_get.md)|[managedAppProtection](../resources/intune_mam_managedappprotection.md)|读取 [managedAppProtection](../resources/intune_mam_managedappprotection.md) 对象的属性和关系。|
|[targetApps 操作](../api/intune_mam_managedappprotection_targetapps.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|id|字符串|实体的键。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|设备未连接到 Internet 时在该时间段后检查访问权限。|
|periodOnlineBeforeAccessCheck|Duration|设备连接到 Internet 时在该时间段后检查访问权限。|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|允许传输其中的数据的源。 可取值为：`allApps`、`managedApps`、`none`。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|允许向其传输数据的目标。 可取值为：`allApps`、`managedApps`、`none`。|
|organizationalCredentialsRequired|布尔值|指示是否需要组织凭据才能使用应用。|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|可以在托管设备上的应用之间共享剪贴板的级别。 可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。|
|dataBackupBlocked|布尔值|指示是否阻止备份托管应用的数据。|
|deviceComplianceRequired|布尔值|指示是否需要设备合规性。|
|managedBrowserToOpenLinksRequired|布尔值|指示是否应在托管浏览器应用中打开 Internet 链接。|
|saveAsBlocked|布尔值|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。|
|pinRequired|布尔值|指示是否需要应用级 pin。|
|maximumPinRetries|Int32|在阻止或擦除托管应用之前，不正确 PIN 重新尝试的最大尝试次数。|
|simplePinBlocked|布尔值|指示是否阻止 simplePin。|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 pin 所需的最小 pin 长度。|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 PIN 的字符集。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 pin。|
|allowedDataStorageLocations|[managedAppDataStorageLocation enum](../resources/intune_mam_managedappdatastoragelocation.md) 集合|用户可能存储托管数据的数据存储位置。|
|contactSyncBlocked|布尔值|指示联系人是否可以同步到用户的设备。|
|printBlocked|布尔值|指示是否允许从托管应用进行打印。|
|fingerprintBlocked|布尔值|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 pin。|
|disableAppPinIfDevicePinIsSet|布尔值|指示如果设置了设备 pin，是否需要使用应用 pin。|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.managedAppProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String"
}
```



