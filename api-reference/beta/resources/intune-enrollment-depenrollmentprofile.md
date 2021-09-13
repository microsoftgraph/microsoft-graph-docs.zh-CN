---
title: depEnrollmentProfile 资源类型
description: depEnrollmentProfile 资源表示 Apple Device Enrollment Program (DEP) 注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ed2fa9eb93eaf03d31d54390ab77569e9b976b0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091214"
---
# <a name="depenrollmentprofile-resource-type"></a>depEnrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

depEnrollmentProfile 资源表示 Apple Device Enrollment Program (DEP) 注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。


继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 集合|列出 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象的属性和关系。|
|[获取 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|读取 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象的属性和关系。|
|[创建 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|创建新的 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象。|
|[删除 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|无|删除 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)。|
|[更新 depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|更新 [depEnrollmentProfile 对象](../resources/intune-enrollment-depenrollmentprofile.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|配置文件的名称 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|说明|String|配置文件的说明 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|指示配置文件是否要求用户身份验证 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|用于注册的配置终结点 URL 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple Setup Assistant 进行身份验证，而不是公司门户。 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示在公司门户注册的设备上需要此权限。继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|指示这是否为默认配置文件|
|supervisedModeEnabled|Boolean|监督模式，如果为 True，则启用，否则为 false。 有关 https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune 其他信息，请参阅 。|
|supportDepartment|String|支持部门信息|
|passCodeDisabled|Boolean|指示密码设置窗格是否被禁用|
|isMandatory|Boolean|指示配置文件是否是必需的|
|locationDisabled|Boolean|指示位置服务设置窗格是否被禁用|
|supportPhoneNumber|String|支持电话号码|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|指示 iTunes 配对模式。 可取值为：`disallow`、`allow`、`requiresCertificate`。|
|profileRemovalDisabled|Boolean|指示配置文件删除选项是否被禁用|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合|Apple Configurator 的管理证书|
|restoreBlocked|Boolean|指示是否阻止了"还原设置"窗格|
|restoreFromAndroidDisabled|Boolean|指示是否禁用从 Android 还原|
|appleIdDisabled|Boolean|指示 Apple ID 设置窗格是否被禁用|
|termsAndConditionsDisabled|Boolean|指示"条款和条件"设置窗格是否被禁用|
|touchIdDisabled|Boolean|指示触摸 ID 设置窗格是否被禁用|
|applePayDisabled|Boolean|指示 Apple 付款设置窗格是否被禁用|
|zoomDisabled|Boolean|指示是否禁用了缩放设置窗格|
|siriDisabled|Boolean|指示是否禁用了 siri 设置窗格|
|diagnosticsDisabled|Boolean|指示诊断设置窗格是否被禁用|
|macOSRegistrationDisabled|Boolean|指示是否禁用 Mac OS 注册|
|macOSFileVaultDisabled|Boolean|指示是否禁用 Mac OS 文件保管库|
|awaitDeviceConfiguredConfirmation|Boolean|指示设备是否需要等待配置的确认|
|sharedIPadMaximumUserCount|Int32|这指定可以使用共享网站的最大iPad。 仅适用于共享iPad模式。|
|enableSharedIPad|Boolean|这指示设备是否将在支持多用户方案的模式下注册。 仅适用于共享 iPad。|

## <a name="relationships"></a>关系
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
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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



