---
title: userPFXCertificate 资源类型
description: 封装用户的 PFX 证书所需的所有信息的实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9b3ed77f4448bdfbe881f6f659208f9dbdff691
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967705"
---
# <a name="userpfxcertificate-resource-type"></a>userPFXCertificate 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

封装用户的 PFX 证书所需的所有信息的实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)集合|列出[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。|
|[获取 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|读取[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。|
|[创建 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。|
|[删除 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|无|删除[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)。|
|[更新 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|PFX 证书的唯一标识符。|
|为|String|SHA-1 PFX 证书的指纹。|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|证书的预期目的是从部署的角度来看。 可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。|
|userPrincipalName|String|PFX 证书的用户主体名称。|
|startDateTime|DateTimeOffset|证书的有效期开始日期/时间。|
|expirationDateTime|DateTimeOffset|证书的有效期到期日期/时间。|
|providerName|String|用于加密此 blob 的加密提供程序。|
|名|String|用于对 blob 进行加密的密钥 (在提供程序中) 的名称。|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|加密/解密过程中提供程序使用的填充方案。 可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。|
|encryptedPfxBlob|Binary|加密的 PFX blob。|
|encryptedPfxPassword|String|加密的 PFX 密码。|
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





