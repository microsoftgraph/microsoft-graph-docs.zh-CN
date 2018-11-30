---
title: enrollmentProfile 资源类型
description: EnrollmentProfile 资源表示它必须提供预注册启用注册其标识已预暂存某些设备配置的集合。 预暂存的设备标识分配给此类型的配置文件，以应用在相应的设备的注册的配置文件的配置。
ms.openlocfilehash: 884fee5c6851e79d96cd036294e5e5485d6df66a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045130"
---
# <a name="enrollmentprofile-resource-type"></a>enrollmentProfile 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

EnrollmentProfile 资源表示它必须提供预注册启用注册其标识已预暂存某些设备配置的集合。 预暂存的设备标识分配给此类型的配置文件，以应用在相应的设备的注册的配置文件的配置。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)集合|列出属性和[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象之间的关系。|
|[获取 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|读取属性和[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的关系。|
|[创建 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|创建新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。|
|[删除 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|无|删除[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。|
|[更新 enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。|
|[setDefaultProfile 操作](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|无|尚未记录|
|[exportMobileConfig 函数](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|字符串|导出移动配置|
|[updateDeviceProfileAssignment 操作](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的 GUID|
|displayName|字符串|配置文件的名称|
|说明|字符串|配置文件的说明|
|requiresUserAuthentication|布尔|指示该配置文件是否要求用户身份验证|
|configurationEndpointUrl|字符串|配置用于注册的终结点 url|
|enableAuthenticationViaCompanyPortal|布尔|指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。|

## <a name="relationships"></a>Relationships
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
  "enableAuthenticationViaCompanyPortal": true
}
```





