---
title: bitlocker 类型
description: BitLocker 资源
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ad8a05e82cd3f300bedf034fe18f67ce3359f16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038864"
---
# <a name="bitlocker-resource-type"></a>bitlocker 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

存储的 BitLocker 密钥的父资源，其中包含包含实际恢复密钥的 **bitlockerRecoveryKey** 导航属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 recoveryKeys](../api/bitlocker-list-recoverykeys.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合|获取 bitlockerRecoveryKey 对象及其属性的列表。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
| 关系 | 类型 | 说明 |
|--|--|--|
| recoveryKeys | [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合 | 与 bitlocker 实体关联的恢复密钥。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitlocker",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlocker"
}
```

