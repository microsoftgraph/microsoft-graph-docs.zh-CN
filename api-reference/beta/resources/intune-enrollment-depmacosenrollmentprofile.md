---
title: depMacOSEnrollmentProfile 资源类型
description: DepMacOSEnrollmentProfile 资源表示特定于 macOS 配置的 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cd23167a10f3d7a40b09ce1f348f90340ac60c6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163117"
---
# <a name="depmacosenrollmentprofile-resource-type"></a>depMacOSEnrollmentProfile 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepMacOSEnrollmentProfile 资源表示特定于 macOS 配置的 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。


继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depMacOSEnrollmentProfiles](../api/intune-enrollment-depmacosenrollmentprofile-list.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)集合|列出[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性和关系。|
|[获取 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|读取[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性和关系。|
|[创建 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-create.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|创建新的[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象。|
|[删除 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-delete.md)|无|删除[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)。|
|[更新 depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-update.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|更新[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID|
|displayName|字符串|继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称|
|说明|字符串|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明|
|requiresUserAuthentication|布尔|指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证|
|configurationEndpointUrl|字符串|用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url|
|enableAuthenticationViaCompanyPortal|布尔|指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。 继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|布尔|指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户|
|isDefault|布尔|指示这是否是从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件|
|supervisedModeEnabled|布尔|监督模式, 如果启用, 则为 True, 否则为 false。 有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。 继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|字符串|支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息|
|passCodeDisabled|布尔|指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格|
|isMandatory|布尔|指示是否必须从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件|
|locationDisabled|布尔|指示是否禁用从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格|
|supportPhoneNumber|字符串|支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码|
|profileRemovalDisabled|布尔|指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项|
|restoreBlocked|布尔|指示是否阻止从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格|
|appleIdDisabled|布尔|指示是否禁用了 Apple id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承|
|termsAndConditionsDisabled|布尔|指示是否已禁用 "条款和条件" 安装窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承|
|touchIdDisabled|布尔|指示是否禁用了触控 id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承|
|applePayDisabled|布尔|指示是否禁用了 Apple 付费设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承|
|zoomDisabled|布尔|指示是否禁用了缩放设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承|
|siriDisabled|布尔|指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格|
|diagnosticsDisabled|布尔|指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格|
|displayToneSetupDisabled|布尔|指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕|
|privacyPaneDisabled|布尔|指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕|
|registrationDisabled|布尔|指示是否禁用注册|
|fileVaultDisabled|布尔|指示是否禁用了文件电子仓库|
|iCloudDiagnosticsDisabled|布尔|指示是否禁用了 iCloud 分析屏幕|

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```




