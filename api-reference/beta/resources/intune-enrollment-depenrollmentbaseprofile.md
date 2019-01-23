---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423753"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>depEnrollmentBaseProfile 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号


继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)集合|列出属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象之间的关系。|
|[获取 depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|读取属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的关系。|

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
|isDefault|Boolean|指示是否这是默认配置文件|
|supervisedModeEnabled|Boolean|监管模式下，设置为 True 可启用，false 否则。 请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。|
|supportDepartment|String|支持部门信息|
|passCodeDisabled|Boolean|指示是否密码设置窗格被禁用|
|isMandatory|Boolean|指示是否强制配置文件|
|locationDisabled|Boolean|指示是否位置服务设置窗格被禁用|
|supportPhoneNumber|String|支持电话号码|
|profileRemovalDisabled|Boolean|指示是否已禁用配置文件删除选项|
|restoreBlocked|Boolean|指示是否还原设置窗格被阻止|
|appleIdDisabled|Boolean|指示是否 Apple id 设置窗格被禁用|
|termsAndConditionsDisabled|Boolean|指示是否已禁用条款和条件设置窗格|
|touchIdDisabled|Boolean|指示是否触摸 id 设置窗格被禁用|
|applePayDisabled|Boolean|指示是否 Apple 付薪设置窗格被禁用|
|zoomDisabled|Boolean|指示是否缩放设置窗格被禁用|
|siriDisabled|Boolean|指示是否 siri 设置窗格被禁用|
|diagnosticsDisabled|Boolean|指示是否诊断设置窗格被禁用|
|displayToneSetupDisabled|Boolean|指示是否禁用 displaytone 设置屏幕|
|privacyPaneDisabled|Boolean|指示是否禁用隐私屏幕|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
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
  "privacyPaneDisabled": true
}
```




