---
title: bitlocker 类型
description: BitLocker 资源
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3e714015b3834051371861880355360f02d12166
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761833"
---
# <a name="bitlocker-resource-type"></a>bitlocker 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含实际恢复密钥的导航属性 **bitlockerRecoveryKey** 的已存储 BitLocker 密钥的父资源。

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

