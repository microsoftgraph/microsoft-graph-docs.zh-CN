---
title: pfxUserCertificate 资源类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d1b7482da130a0c5208aa3e0b36315be0a3bd98
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080672"
---
# <a name="pfxusercertificate-resource-type"></a>pfxUserCertificate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 pfxUserCertificates](../api/intune-raimportcerts-pfxusercertificate-list.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 集合|列出 [pfxUserCertificate 对象的属性和](../resources/intune-raimportcerts-pfxusercertificate.md) 关系。|
|[获取 pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-get.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|读取 [pfxUserCertificate 对象的属性和](../resources/intune-raimportcerts-pfxusercertificate.md) 关系。|
|[创建 pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-create.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|创建新的 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象。|
|[删除 pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-delete.md)|无|删除 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)。|
|[更新 pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-update.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|更新 [pfxUserCertificate 对象](../resources/intune-raimportcerts-pfxusercertificate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|tenantId|Guid|尚未记录|
|userId|Guid|尚未记录|
|thumbprint|String|尚未记录|
|userUpn|String|尚未记录|
|encryptedPfxBlob|String|尚未记录|
|encryptedPfxPassword|String|尚未记录|
|certStartDate|DateTimeOffset|尚未记录|
|certExpirationDate|DateTimeOffset|尚未记录|
|providerName|String|尚未记录|
|encryptionKeyName|String|尚未记录|
|paddingScheme|Int32|尚未记录|
|status|Int32|尚未记录|
|intendedPurpose|Int32|尚未记录|
|createdTime|DateTimeOffset|尚未记录|
|isDeleted|Boolean|尚未记录|
|lastModifiedTime|DateTimeOffset|尚未记录|
|eTag|String|尚未记录|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxUserCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "Guid",
  "userId": "Guid",
  "thumbprint": "String",
  "userUpn": "String",
  "encryptedPfxBlob": "String",
  "encryptedPfxPassword": "String",
  "certStartDate": "String (timestamp)",
  "certExpirationDate": "String (timestamp)",
  "providerName": "String",
  "encryptionKeyName": "String",
  "paddingScheme": 1024,
  "status": 1024,
  "intendedPurpose": 1024,
  "createdTime": "String (timestamp)",
  "isDeleted": true,
  "lastModifiedTime": "String (timestamp)",
  "eTag": "String"
}
```



