---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57a3ad19e988327e126b6da757c2dc5b90c280de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425615"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a>bitLockerRemovableDrivePolicy 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




