---
title: userPFXCertificate 资源类型
description: 封装用户的 PFX 证书所需全部信息的实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9873d6e5a17e356ce166a90107bbf74cf8a341411fa8e741d3b989f684e967bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242424"
---
# <a name="userpfxcertificate-resource-type"></a>userPFXCertificate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

封装用户的 PFX 证书所需全部信息的实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 集合|列出 [userPFXCertificate 对象的属性和](../resources/intune-raimportcerts-userpfxcertificate.md) 关系。|
|[获取 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|读取 [userPFXCertificate 对象的属性和](../resources/intune-raimportcerts-userpfxcertificate.md) 关系。|
|[创建 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|创建新的 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 对象。|
|[删除 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|无|删除用户 [PFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)。|
|[更新 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|更新 [userPFXCertificate 对象](../resources/intune-raimportcerts-userpfxcertificate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|PFX 证书的唯一标识符。|
|thumbprint|字符串|PFX 证书的 SHA-1 指纹。|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|从部署的角度来看，证书的目的。 可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。|
|userPrincipalName|字符串|用户主体 PFX 证书的名称。|
|startDateTime|DateTimeOffset|证书的有效期开始日期/时间。|
|expirationDateTime|DateTimeOffset|证书的有效期过期日期/时间。|
|providerName|String|用于加密此 blob 的加密提供程序。|
|keyName|String|提供程序中用于 (blob 的) 的名称。|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|提供程序在加密/解密期间使用的填充方案。 可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。|
|encryptedPfxBlob|二进制|加密的 PFX blob。|
|encryptedPfxPassword|字符串|加密的 PFX 密码。|
|createdDateTime|DateTimeOffset|导入此 PFX 证书的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改此 PFX 证书的日期/时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




