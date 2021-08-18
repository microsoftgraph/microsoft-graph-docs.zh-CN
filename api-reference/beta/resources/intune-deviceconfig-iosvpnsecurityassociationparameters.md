---
title: iosVpnSecurityAssociationParameters 资源类型
description: VPN 安全关联参数
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 10520e1302acd6e3ba0b2c8cd1af39de8e6c85ec
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266952"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a>iosVpnSecurityAssociationParameters 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 安全关联参数

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|securityEncryptionAlgorithm|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|加密算法。 可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`、`aes192`、`aes192Gcm`、`chaCha20Poly1305`。|
|securityIntegrityAlgorithm|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|完整性算法。 可取值为：`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512`、`md5`。|
|securityDiffieHellmanGroup|Int32|Diffie-Hellman 组|
|lifetimeInMinutes|Int32|生命周期 (分钟) |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```




