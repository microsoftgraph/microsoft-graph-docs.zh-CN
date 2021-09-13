---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密基本策略。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc18eac1aca5f78af3379e5f22de575b5fa35133
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127525"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>bitLockerSystemDrivePolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

BitLocker 加密基本策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|选择操作系统驱动器的加密方法。 可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。|
|startupAuthenticationRequired|Boolean|启动时需要其他身份验证。|
|startupAuthenticationBlockWithoutTpmChip|Boolean|指示是否允许没有兼容的 TPM (BitLocker 需要密码或 U 盘上的启动密钥) 。|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许/要求/禁止 TPM 启动。 可取值为：`blocked`、`required`、`allowed`、`notConfigured`。|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许/要求/不允许 TPM 启动引脚。 可取值为：`blocked`、`required`、`allowed`、`notConfigured`。|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许/要求/不允许 TPM 启动密钥。 可取值为：`blocked`、`required`、`allowed`、`notConfigured`。|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许/要求/禁止 TPM 启动引脚密钥和密钥。 可取值为：`blocked`、`required`、`allowed`、`notConfigured`。|
|minimumPinLength|Int32|指示启动引脚的最小长度。 有效值为 4 至 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|允许在缺少所需的启动密钥信息的情况下恢复 BitLocker 加密的操作系统驱动器。 当你打开 BitLocker 时，将应用此策略设置。|
|prebootRecoveryEnableMessageAndUrl|Boolean|启用预启动恢复消息和 Url。 如果 requireStartupAuthentication 为 false，则此值不会影响。|
|prebootRecoveryMessage|String|定义自定义恢复邮件。|
|prebootRecoveryUrl|String|定义自定义恢复 URL。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```



