---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 12310f8f471c8719972c7c4def540c67b2e5176f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795748"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>bitLockerRecoveryOptions 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

BitLocker 恢复选项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|blockDataRecoveryAgent|布尔值|指示是否阻止基于证书的数据恢复代理。|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许用户或需要用户为固定或系统磁盘生成48位数的恢复密码。 可取值为：`blocked`、`required`、`allowed`。|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许用户或需要用户生成用于固定或系统磁盘的256位恢复密钥。 可取值为：`blocked`、`required`、`allowed`。|
|hideRecoveryOptions|布尔值|指示是否允许在 BitLocker 安装向导中显示固定或系统磁盘的恢复选项。|
|enableRecoveryInformationSaveToStore|布尔值|指示是否允许 BitLocker 恢复信息存储在 AD DS 中。|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|配置存储在 AD DS 中的 BitLocker 恢复信息的哪些部分。 可取值为：`passwordAndKey`、`passwordOnly`。|
|enableBitLockerAfterRecoveryInformationToStore|布尔值|指示在将恢复信息存储在 AD DS 中之前是否启用 BitLocker。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```



