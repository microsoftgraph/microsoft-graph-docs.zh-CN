---
title: depIOSEnrollmentProfile 资源类型
description: DepIOSEnrollmentProfile 资源表示为 iOS 配置特定的 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0068921c65085417712efbe41e9145ac0b122cab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400891"
---
# <a name="depiosenrollmentprofile-resource-type"></a>depIOSEnrollmentProfile 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepIOSEnrollmentProfile 资源表示为 iOS 配置特定的 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号


继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)集合|列出属性和[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象之间的关系。|
|[获取 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|读取属性和[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的关系。|
|[创建 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|创建新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。|
|[删除 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|无|删除[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)。|
|[更新 depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|更新[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID|
|displayName|String|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称|
|说明|String|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明|
|requiresUserAuthentication|Boolean|指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承|
|configurationEndpointUrl|String|配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。 继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示安装程序注册的助手设备继承[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) ，需要的公司门户|
|isDefault|Boolean|指示是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的默认配置文件继承|
|supervisedModeEnabled|Boolean|监管模式下，设置为 True 可启用，false 否则。 请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。 继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)支持部门信息继承|
|passCodeDisabled|Boolean|指示是否密码设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承|
|isMandatory|Boolean|指示是否强制继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)配置文件|
|locationDisabled|Boolean|指示是否服务设置窗格中的位置禁用[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承|
|supportPhoneNumber|String|支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的电话号码继承|
|profileRemovalDisabled|Boolean|指示是否已禁用配置文件删除选项继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Boolean|指示是否还原设置窗格被阻止继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|指示是否 Apple id 设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承|
|termsAndConditionsDisabled|Boolean|指示是否已禁用条款和条件设置窗格继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|指示是否触摸 id 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|指示是否 Apple 付薪设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|zoomDisabled|Boolean|指示是否缩放设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Boolean|指示是否 siri 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean|指示安装程序窗格是的诊断是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承|
|displayToneSetupDisabled|Boolean|指示是否禁用 displaytone 设置屏幕继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boolean|指示是否禁用隐私屏幕继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|指示 iTunes 配对模式。 可取值为：`disallow`、`allow`、`requiresCertificate`。|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合|Apple 配置程序的管理证书|
|restoreFromAndroidDisabled|Boolean|指示是否从 Android 还原被禁用|
|awaitDeviceConfiguredConfirmation|Boolean|指示是否设备需要等待配置确认|
|sharedIPadMaximumUserCount|Int32|此选项指定的最大可以使用共享的 iPad 的用户数。 仅适用于共享的 iPad 模式。|
|enableSharedIPad|Boolean|这指示是否要启用多用户方案模式注册设备。 仅适用于共享 Ipad。|
|companyPortalVppTokenId|String|如果设置，则指示用于部署具有设备许可的公司门户的 Vpp 令牌。 要设置此属性，必须设置 enableAuthenticationViaCompanyPortal。|
|enableSingleAppEnrollmentMode|Boolean|通知要启用单个应用程序模式并应用在注册期间应用锁的设备。 默认值为 false。 必须为要设置此属性设置 enableAuthenticationViaCompanyPortal' 和 'companyPortalVppTokenId。|
|homeButtonScreenDisabled|Boolean|指示是否已禁用主页按钮敏感度屏幕|
|iMessageAndFaceTimeScreenDisabled|Boolean|指示如果 iMessage 并禁用 FaceTime 屏幕|
|onBoardingScreenDisabled|Boolean|指示是否禁用欢迎使用安装程序屏幕|
|screenTimeScreenDisabled|Boolean|指示是否禁用屏幕超时设置|
|simSetupScreenDisabled|Boolean|指示是否禁用 SIMSetup 屏幕|
|softwareUpdateScreenDisabled|Boolean|指示是否必需的软件更新屏幕上被禁用|
|watchMigrationScreenDisabled|Boolean|指示是否禁用监视迁移屏幕|

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
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




