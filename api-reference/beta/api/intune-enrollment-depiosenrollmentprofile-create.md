---
title: 创建 depIOSEnrollmentProfile
description: 创建新的 depIOSEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e4cadbd36e6dbe46e80865e70a5d5e2cc751766
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207607"
---
# <a name="create-depiosenrollmentprofile"></a>创建 depIOSEnrollmentProfile

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 depIOSEnrollmentProfile 对象提供 JSON 表示形式。

下表显示了创建 depIOSEnrollmentProfile 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的对象的 GUID|
|displayName|String|从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的配置文件的名称|
|说明|String|从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的配置文件的说明|
|requiresUserAuthentication|Boolean|指示配置文件是否需要从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的用户身份验证|
|configurationEndpointUrl|String|用于从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的注册的配置终结点 URL|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple 安装助手而不是公司门户进行身份验证。 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的安装助理注册设备上需要公司门户|
|isDefault|Boolean|指示这是否是从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的默认配置文件|
|supervisedModeEnabled|Boolean|监督模式，True 要启用，否则为 false。 有关其他信息，请参阅 https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune 。 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的支持部门信息|
|isMandatory|Boolean|指示配置文件是否为强制继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|指示是否禁用了从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的位置服务设置窗格|
|supportPhoneNumber|字符串|支持从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的电话号码|
|profileRemovalDisabled|Boolean|指示是否禁用了从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的配置文件删除选项|
|restoreBlocked|Boolean|指示是否阻止“还原设置”窗格从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|appleIdDisabled|Boolean|指示是否禁用 Apple ID 设置窗格从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|termsAndConditionsDisabled|Boolean|指示是否禁用了“条款和条件”设置窗格从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|touchIdDisabled|Boolean|指示是否禁用了从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的触摸 ID 设置窗格|
|applePayDisabled|Boolean|指示是否禁用 Apple 付款设置窗格从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|siriDisabled|Boolean|指示是否禁用 siri 设置窗格从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|diagnosticsDisabled|Boolean|指示是否禁用诊断设置窗格从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|displayToneSetupDisabled|Boolean|指示是否禁用 displaytone 安装屏幕从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|privacyPaneDisabled|Boolean|指示是否禁用隐私屏幕从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|screenTimeScreenDisabled|Boolean|指示是否禁用屏幕超时设置从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承|
|deviceNameTemplate|String|设置文本或名称模式。 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Boolean|从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的安装助理登录的 URL|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|指示 iTunes 配对模式。 可取值为：`disallow`、`allow`、`requiresCertificate`。|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合|Apple Configurator 的管理证书|
|restoreFromAndroidDisabled|Boolean|指示是否已禁用从 Android 还原|
|awaitDeviceConfiguredConfirmation|Boolean|指示设备是否需要等待配置的确认|
|sharedIPadMaximumUserCount|Int32|这指定可以使用共享iPad的最大用户数。 仅适用于共享iPad模式。|
|enableSharedIPad|Boolean|这指示是否要在启用多用户方案的模式下注册设备。 仅适用于共享 iPad。|
|companyPortalVppTokenId|String|如果已设置，则指示应使用哪个 Vpp 令牌来部署公司门户 w/设备许可。 必须设置“enableAuthenticationViaCompanyPortal”才能设置此属性。|
|enableSingleAppEnrollmentMode|Boolean|告知设备在注册期间启用单个应用模式并应用应用锁定。 默认为 false。 必须设置“enableAuthenticationViaCompanyPortal”和“companyPortalVppTokenId”才能设置此属性。|
|homeButtonScreenDisabled|Boolean|指示是否禁用了主页按钮敏感度屏幕|
|iMessageAndFaceTimeScreenDisabled|Boolean|指示是否禁用了 iMessage 和 FaceTime 屏幕|
|onBoardingScreenDisabled|Boolean|指示是否禁用了载入设置屏幕|
|simSetupScreenDisabled|Boolean|指示是否禁用 SIMSetup 屏幕|
|softwareUpdateScreenDisabled|Boolean|指示是否禁用了必需的 sofware 更新屏幕|
|watchMigrationScreenDisabled|Boolean|指示是否禁用监视迁移屏幕|
|appearanceScreenDisabled|Boolean|指示是否禁用了 Apperance 屏幕|
|expressLanguageScreenDisabled|Boolean|指示是否禁用 Express Language 屏幕|
|preferredLanguageScreenDisabled|Boolean|指示是否禁用首选语言屏幕|
|deviceToDeviceMigrationDisabled|Boolean|指示是否禁用了设备到设备的迁移|
|welcomeScreenDisabled|Boolean|指示是否禁用了 Weclome 屏幕|
|passCodeDisabled|Boolean|指示是否禁用了密码设置窗格|
|zoomDisabled|Boolean|指示是否禁用了缩放设置窗格|
|restoreCompletedScreenDisabled|Boolean|指示是否禁用了 Weclome 屏幕|
|updateCompleteScreenDisabled|Boolean|指示是否禁用了 Weclome 屏幕|
|forceTemporarySession|Boolean|指示是否启用临时会话|
|temporarySessionTimeoutInSeconds|Int32|指示临时会话超时|
|userSessionTimeoutInSeconds|Int32|指示临时会话超时|
|passcodeLockGracePeriodInSeconds|Int32|指示锁定屏幕之前超时要求用户输入设备密码来解锁它|
|carrierActivationUrl|String|用于激活设备 eSIM 的运营商 URL。|
|userlessSharedAadModeEnabled|Boolean|指示此 apple 设备被指定为支持“共享设备模式”方案。 这与“共享iPad”方案不同。 看到 https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-shared-ios|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 2377

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true,
  "forceTemporarySession": true,
  "temporarySessionTimeoutInSeconds": 0,
  "userSessionTimeoutInSeconds": 11,
  "passcodeLockGracePeriodInSeconds": 0,
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/",
  "userlessSharedAadModeEnabled": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2426

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true,
  "forceTemporarySession": true,
  "temporarySessionTimeoutInSeconds": 0,
  "userSessionTimeoutInSeconds": 11,
  "passcodeLockGracePeriodInSeconds": 0,
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/",
  "userlessSharedAadModeEnabled": true
}
```




