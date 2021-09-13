---
title: enrollmentProfile 资源类型
description: enrollmentProfile 资源表示配置集合，必须预先提供这些配置才能注册其标识已预先存储的某些设备。 预部署设备标识将分配给此类型的配置文件，以在注册相应设备时应用配置文件的配置。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bae158fb33e4d1fccc4e5b4b6fd527b0d17cc9df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141086"
---
# <a name="enrollmentprofile-resource-type"></a>enrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

enrollmentProfile 资源表示配置集合，必须预先提供这些配置才能注册其标识已预先存储的某些设备。 预部署设备标识将分配给此类型的配置文件，以在注册相应设备时应用配置文件的配置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 集合|列出 [enrollmentProfile 对象的属性和](../resources/intune-enrollment-enrollmentprofile.md) 关系。|
|[获取 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|读取 [enrollmentProfile 对象的属性和](../resources/intune-enrollment-enrollmentprofile.md) 关系。|
|[创建 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|创建新的 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 对象。|
|[删除 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|无|删除 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。|
|[更新 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|更新 [enrollmentProfile 对象](../resources/intune-enrollment-enrollmentprofile.md) 的属性。|
|[setDefaultProfile 操作](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|无|尚未记录|
|[exportMobileConfig 函数](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|导出移动配置|
|[updateDeviceProfileAssignment 操作](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|displayName|String|配置文件的名称|
|说明|String|配置文件的说明|
|requiresUserAuthentication|Boolean|指示配置文件是否要求用户身份验证|
|configurationEndpointUrl|String|用于注册的配置终结点 URL|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple Setup Assistant 进行身份验证，而不是公司门户。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示公司门户注册的设备上需要安装助手|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```



