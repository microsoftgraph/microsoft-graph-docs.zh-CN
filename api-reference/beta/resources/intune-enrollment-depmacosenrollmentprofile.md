---
title: depMacOSEnrollmentProfile 资源类型
description: DepMacOSEnrollmentProfile 资源表示特定于 macOS 配置的 Apple 设备注册 (DEP) 注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d74022e23e7f79ea1c8b0e42eb5f56f0ba1a4a65
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494127"
---
# <a name="depmacosenrollmentprofile-resource-type"></a>depMacOSEnrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepMacOSEnrollmentProfile 资源表示特定于 macOS 配置的 Apple 设备注册 (DEP) 注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。


继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depMacOSEnrollmentProfiles](../api/intune-enrollment-depmacosenrollmentprofile-list.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 集合|列出 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象的属性和关系。|
|[获取 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|读取 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象的属性和关系。|
|[创建 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-create.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|创建新的 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象。|
|[删除 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-delete.md)|无|删除 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)。|
|[更新 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-update.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|更新 [depMacOSEnrollmentProfile 对象](../resources/intune-enrollment-depmacosenrollmentprofile.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|配置文件的名称 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|说明|String|配置文件的说明 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|指示配置文件是否要求用户身份验证 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|用于注册的配置终结点 URL 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple Setup Assistant 而不是 公司门户。 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示在公司门户注册的设备上需要安装文件。继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|指示这是否为默认配置文件 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolean|监督模式，如果为 True，则启用，否则为 false。 有关 https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune 其他信息，请参阅 。 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|支持部门信息 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
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
|registrationDisabled|Boolean|指示注册是否被禁用|
|fileVaultDisabled|Boolean|指示文件保管库是否被禁用|
|iCloudDiagnosticsDisabled|Boolean|指示 iCloud Analytics 屏幕是否被禁用|
|passCodeDisabled|Boolean|指示密码设置窗格是否被禁用|
|zoomDisabled|Boolean|指示是否禁用了缩放设置窗格|
|iCloudStorageDisabled|Boolean|指示 iCloud 文档和桌面屏幕是否被禁用|
|chooseYourLockScreenDisabled|Boolean|指示 iCloud 文档和桌面屏幕是否被禁用|
|accessibilityScreenDisabled|Boolean|指示辅助功能屏幕是否被禁用|

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
  "accessibilityScreenDisabled": true
}
```



