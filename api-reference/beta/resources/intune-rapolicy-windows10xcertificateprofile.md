---
title: windows10XCertificateProfile 资源类型
description: " (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 840b898599ec6fc97e6d1c6eba2d1f94cd84329f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301494"
---
# <a name="windows10xcertificateprofile-resource-type"></a>windows10XCertificateProfile 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

 (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型


继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10XCertificateProfiles](../api/intune-rapolicy-windows10xcertificateprofile-list.md)|[windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) 集合|列出 [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) 对象的属性和关系。|
|[获取 windows10XCertificateProfile](../api/intune-rapolicy-windows10xcertificateprofile-get.md)|[windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md)|读取 [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件标识符|
|version|Int32|继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的配置文件的版本|
|displayName|String|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件显示名称|
|description|String|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件说明|
|creationDateTime|DateTimeOffset|已创建从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的 DateTime 配置文件|
|lastModifiedDateTime|DateTimeOffset|上次修改的日期时间配置文件继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|String 集合|继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的范围标记|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|assignments|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCertificateProfile",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




