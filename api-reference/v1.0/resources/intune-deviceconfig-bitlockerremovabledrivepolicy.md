---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 254a57d8da1bd6940096377de0bbc183b6893197
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760263"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a>bitLockerRemovableDrivePolicy 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

BitLocker 可移动驱动器策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|选择可移动驱动器的加密方法。 可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`|
|requireEncryptionForWriteAccess|Boolean|指示是否阻止对其他组织中配置的设备的写入权限。  如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。|
|blockCrossOrganizationWriteAccess|Boolean|此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```




