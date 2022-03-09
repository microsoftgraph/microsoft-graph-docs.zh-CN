---
title: depIOSEnrollmentProfile 资源类型
description: DepIOSEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 特定于 iOS 配置的注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38c61aa1f27a13a613e2a2dd062b56ebe03f7ae3
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367620"
---
# <a name="depiosenrollmentprofile-resource-type"></a>depIOSEnrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepIOSEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 特定于 iOS 配置的注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。


继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 集合|列出 [depIOSEnrollmentProfile 对象的属性和](../resources/intune-enrollment-depiosenrollmentprofile.md) 关系。|
|[获取 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|读取 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象的属性和关系。|
|[创建 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|创建新的 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象。|
|[删除 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|无|删除 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)。|
|[更新 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|更新 [depIOSEnrollmentProfile 对象](../resources/intune-enrollment-depiosenrollmentprofile.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|字符串|配置文件的名称 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|说明|String|配置文件的说明 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|指示配置文件是否要求用户身份验证 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|字符串|用于注册的配置终结点 URL 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple Setup Assistant 而不是 公司门户。 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示在公司门户注册的设备上需要此权限。继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|指示这是否为默认配置文件 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolean|监督模式，如果为 True，则启用，否则为 false。 有关 [其他信息，请参阅 Intune](/mem/intune/enrollment/device-enrollment) 设备注册。 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|字符串|支持部门信息 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Boolean|指示配置文件是否必需 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|指示位置服务设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|支持电话号码 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|指示配置文件删除选项是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Boolean|指示是否阻止"还原"设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|指示 Apple id 设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean|指示是否禁用"条款和条件"设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|指示触摸 ID 设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|指示 Apple 付款设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Boolean|指示是否禁用了 siri 设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean|指示诊断设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boolean|指示是否禁用显示铃声设置屏幕 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boolean|指示是否禁用隐私屏幕 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Boolean|指示是否禁用屏幕超时设置 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|String|设置文字或名称模式。 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Boolean|安装助手登录的 URL 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|指示 iTunes 配对模式。 可取值为：`disallow`、`allow`、`requiresCertificate`。|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合|Apple Configurator 的管理证书|
|restoreFromAndroidDisabled|Boolean|指示是否禁用从 Android 还原|
|awaitDeviceConfiguredConfirmation|Boolean|指示设备是否需要等待配置的确认|
|sharedIPadMaximumUserCount|Int32|这指定可以使用共享网站的最大iPad。 仅适用于共享iPad模式。|
|enableSharedIPad|Boolean|这指示设备是否将在支持多用户方案的模式下注册。 仅适用于共享 iPad。|
|companyPortalVppTokenId|String|如果设置，则指示应该使用哪个 Vpp 令牌来部署公司门户许可。 必须设置"enableAuthenticationViaCompanyPortal"才能设置此属性。|
|enableSingleAppEnrollmentMode|Boolean|指示设备在注册期间启用单个应用模式和应用锁。 默认为 false。 必须设置"enableAuthenticationViaCompanyPortal"和"companyPortalVppTokenId"才能设置此属性。|
|homeButtonScreenDisabled|Boolean|指示是否禁用了"开始"按钮敏感度屏幕|
|iMessageAndFaceTimeScreenDisabled|Boolean|指示 iMessage 和 FaceTime 屏幕是否被禁用|
|onBoardingScreenDisabled|Boolean|指示载入设置屏幕是否处于禁用状态|
|simSetupScreenDisabled|Boolean|指示是否禁用 SIMSetup 屏幕|
|softwareUpdateScreenDisabled|Boolean|指示是否禁用了必需的软件更新屏幕|
|watchMigrationScreenDisabled|Boolean|指示监视迁移屏幕是否被禁用|
|appearanceScreenDisabled|Boolean|指示是否禁用 Apperance 屏幕|
|expressLanguageScreenDisabled|Boolean|指示是否禁用 Express Language 屏幕|
|preferredLanguageScreenDisabled|Boolean|指示是否禁用首选语言屏幕|
|deviceToDeviceMigrationDisabled|Boolean|指示设备到设备迁移是否被禁用|
|welcomeScreenDisabled|Boolean|指示是否禁用 Weclome 屏幕|
|passCodeDisabled|Boolean|指示密码设置窗格是否被禁用|
|zoomDisabled|Boolean|指示是否禁用了缩放设置窗格|
|restoreCompletedScreenDisabled|Boolean|指示是否禁用 Weclome 屏幕|
|updateCompleteScreenDisabled|Boolean|指示是否禁用 Weclome 屏幕|
|forceTemporarySession|Boolean|指示是否已启用临时会话|
|temporarySessionTimeoutInSeconds|Int32|指示临时会话的超时|
|userSessionTimeoutInSeconds|Int32|指示临时会话的超时|
|passcodeLockGracePeriodInSeconds|Int32|指示锁定屏幕之前超时要求用户输入设备 passocde 以解锁它|
|carrierActivationUrl|String|用于激活设备 eSIM 的运营商 URL。|
|userlessSharedAadModeEnabled|Boolean|指示此 apple 设备被指定为支持"共享设备模式"方案。 这不同于"共享iPad"方案。 请参阅 [共享 iOS 和 iPadOS 设备](/mem/intune/enrollment/device-enrollment-shared-ios)|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
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
  "deviceNameTemplate": "String",
  "configurationWebUrl": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
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
  "temporarySessionTimeoutInSeconds": 1024,
  "userSessionTimeoutInSeconds": 1024,
  "passcodeLockGracePeriodInSeconds": 1024,
  "carrierActivationUrl": "String",
  "userlessSharedAadModeEnabled": true
}
```




