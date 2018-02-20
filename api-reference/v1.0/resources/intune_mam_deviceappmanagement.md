# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备应用管理单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[Get deviceAppManagement](../api/intune_mam_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|读取 [deviceAppManagement](../resources/intune_mam_deviceappmanagement.md) 对象的属性和关系。|
|[Update deviceAppManagement](../api/intune_mam_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|更新 [deviceAppManagement](../resources/intune_mam_deviceappmanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedAppPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合|托管应用策略。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) 集合|iOS 托管应用策略。|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 集合|Android 托管应用策略。|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 集合|默认的托管应用策略。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 集合|托管应用配置目标。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) 集合|对已注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 集合|对未注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合|托管应用注册。|
|managedAppStatuses|[managedAppStatus](../resources/intune_mam_managedappstatus.md) 集合|托管应用状态。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



