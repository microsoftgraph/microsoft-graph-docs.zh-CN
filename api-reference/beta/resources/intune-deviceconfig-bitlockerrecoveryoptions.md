---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40ca273b46a1e104afbeac4cbafe967ba76faa22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924837"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>bitLockerRecoveryOptions 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

BitLocker 恢复选项。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolean|指示是否阻止基于证书的数据恢复代理。|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许用户或所需的固定生成 48 位数恢复密码或系统磁盘。 可取值为：`blocked`、`required`、`allowed`。|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|指示是否允许用户或所需的固定生成 256 位恢复密钥或系统磁盘。 可取值为：`blocked`、`required`、`allowed`。|
|hideRecoveryOptions|Boolean|指示允许在 BitLocker 安装向导中显示恢复选项的固定或系统磁盘。|
|enableRecoveryInformationSaveToStore|Boolean|指示允许 BitLocker 恢复信息将存储在 AD DS。|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|配置存储到 AD DS BitLocker 恢复信息的哪些部分。 可取值为：`passwordAndKey`、`passwordOnly`。|
|enableBitLockerAfterRecoveryInformationToStore|Boolean|指示启用 BitLocker，直到恢复信息存储在 AD DS。|

## <a name="relationships"></a>Relationships
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





