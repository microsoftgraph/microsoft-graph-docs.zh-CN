---
title: depMacOSEnrollmentProfile 资源类型
description: DepMacOSEnrollmentProfile 资源表示特定于 macOS 配置的 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 注册之前，必须将此类配置文件分配给 Apple DEP 序列号。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb9661733bb33c66b011cf3186801f7a2d698473
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211392"
---
# <a name="depmacosenrollmentprofile-resource-type"></a>depMacOSEnrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepMacOSEnrollmentProfile 资源表示特定于 macOS 配置的 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 注册之前，必须将此类配置文件分配给 Apple DEP 序列号。


继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depMacOSEnrollmentProfiles](../api/intune-enrollment-depmacosenrollmentprofile-list.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 集合|列出 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象的属性和关系。|
|[获取 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|读取 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象的属性和关系。|
|[创建 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-create.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|创建新的 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象。|
|[删除 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-delete.md)|无|删除 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)。|
|[更新 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-update.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|更新 [depMacOSEnrollmentProfile 对象的](../resources/intune-enrollment-depmacosenrollmentprofile.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的对象的 GUID|
|displayName|字符串|从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的配置文件的名称|
|说明|字符串|从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的配置文件的说明|
|requiresUserAuthentication|Boolean|指示配置文件是否需要从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的用户身份验证|
|configurationEndpointUrl|String|用于从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的注册的配置终结点 URL|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple 安装助手而不是公司门户进行身份验证。 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示从 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 继承的安装助理注册设备上需要公司门户|
|isDefault|Boolean|指示这是否是从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的默认配置文件|
|supervisedModeEnabled|Boolean|监督模式，True 要启用，否则为 false。 有关其他信息，请参阅 https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune 。 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|字符串|从 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 继承的支持部门信息|
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

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depMacOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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




