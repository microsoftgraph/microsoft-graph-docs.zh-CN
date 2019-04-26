---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69f0bb3647e5d12d0d441f06e7436626b0d29334
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573912"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>depEnrollmentBaseProfile 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。


继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)集合|列出[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。|
|[获取 depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|读取[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID|
|displayName|String|继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称|
|说明|String|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明|
|requiresUserAuthentication|Boolean|指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证|
|configurationEndpointUrl|String|用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。 继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户|
|isDefault|Boolean|指示这是否为默认配置文件|
|supervisedModeEnabled|Boolean|监督模式, 如果启用, 则为 True, 否则为 false。 有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。|
|supportDepartment|String|支持部门信息|
|passCodeDisabled|Boolean|指示是否禁用密码设置窗格|
|isMandatory|Boolean|指示配置文件是否是必需的|
|locationDisabled|Boolean|指示是否禁用位置服务设置窗格|
|supportPhoneNumber|String|支持电话号码|
|profileRemovalDisabled|Boolean|指示是否禁用了配置文件删除选项|
|restoreBlocked|Boolean|指示是否阻止还原安装程序窗格|
|appleIdDisabled|Boolean|指示是否禁用 Apple id 设置窗格|
|termsAndConditionsDisabled|Boolean|指示是否已禁用 "条款和条件" 安装窗格|
|touchIdDisabled|Boolean|指示是否禁用了触控 id 设置窗格|
|applePayDisabled|Boolean|指示是否禁用 Apple 付费设置窗格|
|zoomDisabled|Boolean|指示是否禁用缩放设置窗格|
|siriDisabled|Boolean|指示是否禁用 siri 安装程序窗格|
|diagnosticsDisabled|Boolean|指示是否禁用诊断设置窗格|
|displayToneSetupDisabled|Boolean|指示是否禁用 displaytone 安装程序屏幕|
|privacyPaneDisabled|Boolean|指示是否禁用隐私屏幕|
|deviceNameTemplate|String|设置文本或名称模式。|

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
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "String"
}
```





