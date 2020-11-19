---
title: windows10XTrustedRootCertificate 资源类型
description: Windows X 受信任的根证书配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f86204ce50cf7eb5123388ab1f7f3637a44f0913
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301561"
---
# <a name="windows10xtrustedrootcertificate-resource-type"></a>windows10XTrustedRootCertificate 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows X 受信任的根证书配置文件


继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10XTrustedRootCertificates](../api/intune-rapolicy-windows10xtrustedrootcertificate-list.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 集合|列出 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象的属性和关系。|
|[获取 windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-get.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|读取 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象的属性和关系。|
|[创建 windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-create.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|创建新的 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象。|
|[删除 windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-delete.md)|无|删除 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)。|
|[更新 windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-update.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|更新 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件标识符|
|version|Int32|继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的配置文件的版本|
|displayName|字符串|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件显示名称|
|description|字符串|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件说明|
|creationDateTime|DateTimeOffset|已创建从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的 DateTime 配置文件|
|lastModifiedDateTime|DateTimeOffset|上次修改的日期时间配置文件继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|String 集合|继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的范围标记|
|trustedRootCertificate|Binary|受信任的根证书|
|certFileName|字符串|要在 UI 中显示的文件名。|
|destinationStore|[certificateDestinationStore](../resources/intune-shared-certificatedestinationstore.md)|受信任的根证书的目标存储位置。 可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XTrustedRootCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "destinationStore": "String"
}
```




