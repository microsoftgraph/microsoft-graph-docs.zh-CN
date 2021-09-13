---
title: bitLockerFixedDrivePolicy 资源类型
description: BitLocker 固定驱动器策略。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0cfebf1ca0560cfa99d157f37bbc6e52a1ce8c2b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146742"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a>bitLockerFixedDrivePolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

BitLocker 固定驱动器策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|选择固定驱动器的加密方法。 可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`|
|requireEncryptionForWriteAccess|Boolean|此策略设置确定是否需要 BitLocker 保护才能在计算机上写入固定数据驱动器。|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|此策略设置允许你控制在没有所需凭据的情况下如何恢复受 BitLocker 保护的固定数据驱动器。 当你打开 BitLocker 时，将应用此策略设置。|

## <a name="relationships"></a>关系
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



