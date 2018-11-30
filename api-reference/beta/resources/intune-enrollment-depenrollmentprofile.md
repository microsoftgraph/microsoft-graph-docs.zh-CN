---
title: depEnrollmentProfile 资源类型
description: DepEnrollmentProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
ms.openlocfilehash: 5c09bac440d2dce8cb141787d0809c74aed747c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048884"
---
# <a name="depenrollmentprofile-resource-type"></a>depEnrollmentProfile 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

DepEnrollmentProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号

继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)集合|列出属性和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象之间的关系。|
|[获取 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|读取属性和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的关系。|
|[创建 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。|
|[删除 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|无|删除[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)。|
|[更新 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|更新[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID|
|displayName|字符串|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称|
|说明|字符串|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明|
|requiresUserAuthentication|布尔|指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承|
|configurationEndpointUrl|字符串|配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|布尔|指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。 继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|布尔|指示是否这是默认配置文件|
|supervisedModeEnabled|布尔|监管模式下，设置为 True 可启用，false 否则。 请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。|
|supportDepartment|字符串|支持部门信息|
|passCodeDisabled|布尔|指示是否密码设置窗格被禁用|
|isMandatory|布尔|指示是否强制配置文件|
|locationDisabled|布尔|指示是否位置服务设置窗格被禁用|
|supportPhoneNumber|字符串|支持电话号码|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|指示 iTunes 配对模式。 可取值为：`disallow`、`allow`、`requiresCertificate`。|
|profileRemovalDisabled|布尔|指示是否已禁用配置文件删除选项|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合|Apple 配置程序的管理证书|
|restoreBlocked|布尔|指示是否还原设置窗格被阻止|
|restoreFromAndroidDisabled|布尔|指示是否从 Android 还原被禁用|
|appleIdDisabled|布尔|指示是否 Apple id 设置窗格被禁用|
|termsAndConditionsDisabled|布尔|指示是否已禁用条款和条件设置窗格|
|touchIdDisabled|布尔|指示是否触摸 id 设置窗格被禁用|
|applePayDisabled|布尔|指示是否 Apple 付薪设置窗格被禁用|
|zoomDisabled|布尔|指示是否缩放设置窗格被禁用|
|siriDisabled|布尔|指示是否 siri 设置窗格被禁用|
|diagnosticsDisabled|布尔|指示是否诊断设置窗格被禁用|
|macOSRegistrationDisabled|布尔|指示已禁用 Mac OS 注册功能|
|macOSFileVaultDisabled|布尔|指示是否禁用 Mac OS 文件存储库|
|awaitDeviceConfiguredConfirmation|布尔|指示是否设备需要等待配置确认|
|sharedIPadMaximumUserCount|Int32|此选项指定的最大可以使用共享的 iPad 的用户数。 仅适用于共享的 iPad 模式。|
|enableSharedIPad|布尔|这指示是否要启用多用户方案模式注册设备。 仅适用于共享 Ipad。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```





