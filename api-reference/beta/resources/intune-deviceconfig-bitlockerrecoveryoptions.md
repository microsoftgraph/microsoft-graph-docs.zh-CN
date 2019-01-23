---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398511"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>bitLockerRecoveryOptions 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




