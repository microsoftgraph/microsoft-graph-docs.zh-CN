---
title: enrollmentProfile 资源类型
description: EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4b7d2683baed89505280d8866132ce9e7846bbc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259814"
---
# <a name="enrollmentprofile-resource-type"></a>enrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 集合|列出 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 对象的属性和关系。|
|[获取 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|读取 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 对象的属性和关系。|
|[创建 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|创建新的 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 对象。|
|[删除 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|无|删除 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。|
|[更新 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|更新 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 对象的属性。|
|[setDefaultProfile 操作](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|无|尚未记录|
|[exportMobileConfig 函数](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|导出移动配置|
|[updateDeviceProfileAssignment 操作](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|displayName|String|配置文件的名称|
|description|String|配置文件的说明|
|requiresUserAuthentication|Boolean|指示配置文件是否需要用户身份验证|
|configurationEndpointUrl|String|用于注册的配置终结点 url|
|enableAuthenticationViaCompanyPortal|Boolean|指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|指示在安装助理注册设备上需要公司门户|

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




