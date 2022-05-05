---
title: 更新 depMacOSEnrollmentProfile
description: 更新 depMacOSEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a0aaa235e0a66739946828c90eab02922933590
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208909"
---
# <a name="update-depmacosenrollmentprofile"></a>更新 depMacOSEnrollmentProfile

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [depMacOSEnrollmentProfile 对象的](../resources/intune-enrollment-depmacosenrollmentprofile.md) 属性。

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象提供 JSON 表示形式。

下表显示了创建 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 时所需的属性。

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
|registrationDisabled|Boolean|指示是否已禁用注册|
|fileVaultDisabled|Boolean|指示是否禁用文件保管库|
|iCloudDiagnosticsDisabled|Boolean|指示是否禁用了 iCloud Analytics 屏幕|
|passCodeDisabled|Boolean|指示是否禁用了密码设置窗格|
|zoomDisabled|Boolean|指示是否禁用了缩放设置窗格|
|iCloudStorageDisabled|Boolean|指示是否禁用了 iCloud 文档和桌面屏幕|
|chooseYourLockScreenDisabled|Boolean|指示是否禁用了 iCloud 文档和桌面屏幕|
|accessibilityScreenDisabled|Boolean|指示是否禁用了辅助功能屏幕|
|autoUnlockWithWatchDisabled|Boolean|指示是否禁用了 UnlockWithWatch 屏幕|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true,
  "autoUnlockWithWatchDisabled": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1389

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true,
  "autoUnlockWithWatchDisabled": true
}
```




