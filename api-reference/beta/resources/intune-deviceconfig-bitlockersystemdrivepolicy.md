---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密的基本策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425706"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>bitLockerSystemDrivePolicy 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

BitLocker 加密的基本策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|选择操作系统驱动器的加密的方法。 可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。|
|startupAuthenticationRequired|Boolean|需要在启动时的其他身份验证。|
|startupAuthenticationBlockWithoutTpmChip|Boolean|指示是否允许 BitLocker 不兼容的 TPM （需要密码或 USB 闪存驱动器上的启动项）。|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许使用或所需/禁止 TPM 启动。 可取值为：`blocked`、`required`、`allowed`。|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许使用或所需/禁止 TPM 启动 pin。 可取值为：`blocked`、`required`、`allowed`。|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许使用或所需/禁止 TPM 启动密钥。 可取值为：`blocked`、`required`、`allowed`。|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否 TPM 启动固定键和密钥是允许/所需/被禁止。 可取值为：`blocked`、`required`、`allowed`。|
|minimumPinLength|Int32|指示启动旋转中心点的最小长度。 有效值 4 到 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|允许恢复需要的启动关键信息不存在的 BitLocker 加密操作系统驱动器。 Bitlocker 打开时，将应用此策略设置。|
|prebootRecoveryEnableMessageAndUrl|Boolean|启用预启动恢复消息和 Url。 如果 requireStartupAuthentication 为 false，则不会影响此值。|
|prebootRecoveryMessage|String|定义的自定义恢复消息。|
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




