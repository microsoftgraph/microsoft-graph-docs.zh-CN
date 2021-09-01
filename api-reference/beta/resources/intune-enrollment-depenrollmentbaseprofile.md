---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple Device Enrollment Program (DEP) 注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 935703a1a74bbd0b35ba0987311f62bce9072a8f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820847"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>depEnrollmentBaseProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepEnrollmentBaseProfile 资源表示 Apple Device Enrollment Program (DEP) 注册配置文件。 必须先将此类配置文件分配给 Apple DEP 序列号，然后相应的设备才能通过 DEP 注册。


继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 集合|列出 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 对象的属性和关系。|
|[获取 depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|读取 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|配置文件的名称 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|字符串|配置文件的说明 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|指示配置文件是否要求用户身份验证 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|用于注册的配置终结点 URL 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple Setup Assistant 而不是 公司门户。 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|布尔值|指示在公司门户注册的设备上需要此权限。继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|指示这是否为默认配置文件|
|supervisedModeEnabled|Boolean|监督模式，如果为 True，则启用，否则为 false。 有关 https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune 其他信息，请参阅 。|
|supportDepartment|String|支持部门信息|
|isMandatory|Boolean|指示配置文件是否是必需的|
|locationDisabled|Boolean|指示位置服务设置窗格是否被禁用|
|supportPhoneNumber|String|支持电话号码|
|profileRemovalDisabled|Boolean|指示配置文件删除选项是否被禁用|
|restoreBlocked|Boolean|指示是否阻止了"还原设置"窗格|
|appleIdDisabled|Boolean|指示 Apple ID 设置窗格是否被禁用|
|termsAndConditionsDisabled|Boolean|指示"条款和条件"设置窗格是否被禁用|
|touchIdDisabled|Boolean|指示触摸 ID 设置窗格是否被禁用|
|applePayDisabled|Boolean|指示 Apple 付款设置窗格是否被禁用|
|siriDisabled|布尔值|指示是否禁用了 siri 设置窗格|
|diagnosticsDisabled|Boolean|指示诊断设置窗格是否被禁用|
|displayToneSetupDisabled|布尔值|指示是否禁用了显示铃声设置屏幕|
|privacyPaneDisabled|Boolean|指示隐私屏幕是否被禁用|
|screenTimeScreenDisabled|布尔值|指示屏幕超时设置是否被禁用|
|deviceNameTemplate|String|设置文字或名称模式。|
|configurationWebUrl|Boolean|设置助手登录的 URL|

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
  "configurationWebUrl": true
}
```



