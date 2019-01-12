---
title: bitLockerFixedDrivePolicy 资源类型
description: BitLocker 固定驱动器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2af642f85e9ae1847b159296cc46298c42d26317
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991130"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a>bitLockerFixedDrivePolicy 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

BitLocker 固定驱动器策略。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|选择固定驱动器的加密方法。 可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`|
|requireEncryptionForWriteAccess|Boolean|此策略设置确定是否需要对固定的数据驱动器可写入的计算机上 BitLocker 保护。|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|此策略设置可以控制如何受保护的 BitLocker 驱动器恢复所需的凭据不存在的固定的数据。 Bitlocker 打开时，将应用此策略设置。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```





