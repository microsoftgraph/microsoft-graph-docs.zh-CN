---
title: userPFXCertificate 资源类型
description: 封装用户的 PFX 证书所需的所有信息的实体。
ms.openlocfilehash: 89040cafa976c88ce84cb8f73bc8a68e2cdfbdf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045919"
---
# <a name="userpfxcertificate-resource-type"></a>userPFXCertificate 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

封装用户的 PFX 证书所需的所有信息的实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)集合|列出属性和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象之间的关系。|
|[获取 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|读取属性和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的关系。|
|[创建 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。|
|[删除 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|无|删除[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)。|
|[更新 userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|PFX 证书的唯一标识符。|
|指纹|字符串|Sha-1 PFX 证书的指纹。|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|证书的适用于从部署的视图点的用途。 可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。|
|userPrincipalName|字符串|PFX 证书的用户主体名称。|
|startDateTime|DateTimeOffset|证书的有效性开始日期/时间。|
|expirationDateTime|DateTimeOffset|证书的有效性过期日期/时间。|
|providerName|字符串|用于加密此 blob 的加密提供程序。|
|键名|字符串|用于加密 blob （在提供程序） 项的名称。|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|填充在加密/解密过程中使用提供程序的方案。 可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。|
|encryptedPfxBlob|二进制数|加密的 PFX blob。|
|encryptedPfxPassword|字符串|加密的 PFX 密码。|
|createdDateTime|DateTimeOffset|日期/时间时此 PFX 证书已导入。|
|lastModifiedDateTime|DateTimeOffset|上次修改此 PFX 证书时的日期/时间。|

## <a name="relationships"></a>Relationships
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





