---
title: managedAllDeviceCertificateState 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4be36b8c62d661957158dce03514e3c20bc4c0c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526060"
---
# <a name="managedalldevicecertificatestate-resource-type"></a>managedAllDeviceCertificateState 资源类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedAllDeviceCertificateStates](../api/intune-deviceconfig-managedalldevicecertificatestate-list.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)集合|列出[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的属性和关系。|
|[获取 managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|读取[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的属性和关系。|
|[创建 managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-create.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|创建新的[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。|
|[删除 managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-delete.md)|无|删除[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)。|
|[更新 managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|更新[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|撤消状态。 可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。|
|managedDeviceDisplayName|String|设备显示名称|
|userPrincipalName|String|用户主体名称|
|certificateExpirationDateTime|DateTimeOffset|证书到期日期|
|certificateIssuerName|String|颁发者|
|certificateThumbprint|String|为|
|certificateSerialNumber|String|序列号|
|certificateSubjectName|String|证书主题名称|
|certificateKeyUsages|Int32|密钥用法|
|certificateExtendedKeyUsages|String|增强型密钥使用|
|certificateIssuanceDateTime|DateTimeOffset|颁发日期|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAllDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "String (identifier)",
  "certificateRevokeStatus": "String",
  "managedDeviceDisplayName": "String",
  "userPrincipalName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuerName": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectName": "String",
  "certificateKeyUsages": 1024,
  "certificateExtendedKeyUsages": "String",
  "certificateIssuanceDateTime": "String (timestamp)"
}
```



