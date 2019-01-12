---
title: 创建 androidWorkProfileGeneralDeviceConfiguration
description: 创建新的 androidWorkProfileGeneralDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 53cd8f310cfa50aafde7b8be3afae7fae2758171
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925355"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a>创建 androidWorkProfileGeneralDeviceConfiguration

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。
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
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。

下表显示时创建 androidWorkProfileGeneralDeviceConfiguration 所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|passwordBlockFingerprintUnlock|Boolean|指示是否阻止指纹解锁。|
|passwordBlockTrustAgents|Boolean|指示是否阻止 Smart Lock 和其他信任代理。|
|passwordExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|密码的最小长度。 有效值为 4 至 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。 有效值为 0 至 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前允许登录失败的次数。 有效值为 4 至 11|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|允许共享的数据的类型。 可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。|
|workProfileBlockNotificationsWhileDeviceLocked|布尔|指示阻止通知时设备锁定。|
|workProfileBlockAddingAccounts|布尔|阻止用户添加/移除工作配置文件中的帐户。|
|workProfileBluetoothEnableContactSharing|布尔|允许蓝牙设备访问企业联系人。|
|workProfileBlockScreenCapture|布尔|阻止工作配置文件中的屏幕截图。|
|workProfileBlockCrossProfileCallerId|布尔|阻止显示工作 profile 呼叫者 ID 个人配置文件中。|
|workProfileBlockCamera|布尔|阻止工作 profile 摄像头。|
|workProfileBlockCrossProfileContactsSearch|布尔|个人配置文件中，阻止工作 profile 联系人可用性。|
|workProfileBlockCrossProfileCopyPaste|布尔|布尔值，指示设置不允许跨是否启用配置文件复制/粘贴。|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|必需的密码类型。 可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。|
|workProfilePasswordBlockFingerprintUnlock|布尔|指示是否阻止指纹解锁工作配置文件。|
|workProfilePasswordBlockTrustAgents|布尔|指示阻止智能锁定和其他信任代理工作配置文件。|
|workProfilePasswordExpirationDays|Int32|过期工作配置文件密码之前的天数。 有效值为 1 至 365。|
|workProfilePasswordMinimumLength|Int32|工作配置文件密码最小长度。 有效值为 4 至 16|
|workProfilePasswordMinNumericCharacters|Int32|最小 ハ  工作配置文件密码中所需的数字字符。 有效的值 1 到 10|
|workProfilePasswordMinNonLetterCharacters|Int32|最小 ハ  中工作配置文件密码必须包含非字母字符。 有效的值 1 到 10|
|workProfilePasswordMinLetterCharacters|Int32|最小 ハ  中工作配置文件密码必须包含字母字符。 有效的值 1 到 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|最小 ハ  工作配置文件密码中需要的小写字符。 有效的值 1 到 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|最小 ハ  中工作配置文件密码必须大写字符。 有效的值 1 到 10|
|workProfilePasswordMinSymbolCharacters|Int32|最小 ハ  工作配置文件密码中需要的符号。 有效的值 1 到 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|workProfilePasswordPreviousPasswordBlockCount|Int32|以前的工作配置文件密码，以阻止数。 有效值为 0 至 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|登录失败之前删除工作配置文件允许和已删除的所有企业数据的数量。 有效值为 4 至 11|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|工作所需的配置文件密码的类型。 可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。|
|workProfileRequirePassword|布尔|密码，则需要或不工作配置文件|
|securityRequireVerifyApps|Boolean|要求启用 Android 验证应用功能。|
|vpnAlwaysOnPackageIdentifier|字符串|始终在 VPN 中启用锁定模式。|
|vpnEnableAlwaysOnLockdownMode|布尔|始终在 VPN 中启用锁定模式。|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2106

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```





