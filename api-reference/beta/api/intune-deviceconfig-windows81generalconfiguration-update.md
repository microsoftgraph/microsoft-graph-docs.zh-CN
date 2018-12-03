---
title: 更新 windows81GeneralConfiguration
description: 更新 windows81GeneralConfiguration 对象的属性。
ms.openlocfilehash: 1469d204349694f453eb7571d90aa7a1ab427387
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046895"
---
# <a name="update-windows81generalconfiguration"></a>更新 windows81GeneralConfiguration

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的 JSON 表示形式。

下表显示了创建 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔值|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。|
|applyOnlyToWindows81|Boolean|指示此策略是否仅适用于 Windows 8.1 的值。 此属性是只读的。|
|browserBlockAutofill|Boolean|指示是否阻止自动填充。|
|browserBlockAutomaticDetectionOfIntranetSites|Boolean|指示是否阻止自动检测 Intranet 站点。|
|browserBlockEnterpriseModeAccess|Boolean|指示是否阻止企业模式访问。|
|browserBlockJavaScript|Boolean|指示是否阻止用户使用 JavaScript。|
|browserBlockPlugins|Boolean|指示是否阻止插件。|
|browserBlockPopups|Boolean|指示是否阻止弹出窗口。|
|browserBlockSendingDoNotTrackHeader|Boolean|指示是否阻止用户发送 Do Not Track 标头。|
|browserBlockSingleWordEntryOnIntranetSites|Boolean|指示是否阻止在 Intranet 站点上使用单字条目。|
|browserRequireSmartScreen|Boolean|指示是否要求用户使用智能屏幕筛选器。|
|browserEnterpriseModeSiteListLocation|String|企业模式网站列表位置。 可能是本地文件、本地网络或 http 位置。|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|Internet 安全级别。 可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|Intranet 安全级别。 可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。|
|browserLoggingReportLocation|String|日志记录报表位置。|
|browserRequireHighSecurityForRestrictedSites|Boolean|指示是否要求受限站点具有高安全性。|
|browserRequireFirewall|Boolean|指示是否需要防火墙。|
|browserRequireFraudWarning|Boolean|指示是否需要诈骗警告。|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|受信任的站点安全级别。 可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。|
|cellularBlockDataRoaming|Boolean|指示是否阻止数据漫游。|
|diagnosticsBlockDataSubmission|Boolean|指示是否阻止诊断数据提交。|
|passwordBlockPicturePasswordAndPin|Boolean|指示是否阻止用户使用图片密码和 PIN。|
|passwordExpirationDays|Int32|密码过期天数。|
|passwordMinimumLength|Int32|密码最短长度。|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordPreviousPasswordBlockCount|Int32|防止重复使用的先前密码的数量。 有效值为 0 至 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前登录失败的次数。|
|storageRequireDeviceEncryption|Boolean|指示是否要求对移动设备加密。|
|minimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|最小值更新分类自动安装。 可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。|
|updatesMinimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|最小值更新分类自动安装。 可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。|
|updatesRequireAutomaticUpdates|Boolean|指示是否需要自动更新。|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|用户帐户控制设置。 可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。|
|workFoldersUrl|String|工作文件夹 URL。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1920

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





