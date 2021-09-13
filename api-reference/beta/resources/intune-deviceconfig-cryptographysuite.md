---
title: cryptographySuite 资源类型
description: VPN 安全关联参数
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de14441335242a8a59f4011055ebae1f5cedc6e2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127378"
---
# <a name="cryptographysuite-resource-type"></a>cryptographySuite 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 安全关联参数

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|encryptionMethod|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|加密方法。 可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`、`aes192`、`aes192Gcm`、`chaCha20Poly1305`。|
|integrityCheckMethod|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|完整性检查方法。 可取值为：`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512`、`md5`。|
|dhGroup|[diffieHellmanGroup](../resources/intune-deviceconfig-diffiehellmangroup.md)|Diffie Hellman 组。 可取值为：`group1`、`group2`、`group14`、`ecp256`、`ecp384`、`group24`。|
|cipherTransformConstants|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|加密转换常量。 可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`、`aes192`、`aes192Gcm`、`chaCha20Poly1305`。|
|authenticationTransformConstants|[authenticationTransformConstant](../resources/intune-deviceconfig-authenticationtransformconstant.md)|身份验证转换常量。 可取值为：`md5_96`、`sha1_96`、`sha_256_128`、`aes128Gcm`、`aes192Gcm`、`aes256Gcm`。|
|pfsGroup|[perfectForwardSecrecyGroup](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|完全向前保密组。 可取值为：`pfs1`、`pfs2`、`pfs2048`、`ecp256`、`ecp384`、`pfsMM`、`pfs24`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cryptographySuite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cryptographySuite",
  "encryptionMethod": "String",
  "integrityCheckMethod": "String",
  "dhGroup": "String",
  "cipherTransformConstants": "String",
  "authenticationTransformConstants": "String",
  "pfsGroup": "String"
}
```



