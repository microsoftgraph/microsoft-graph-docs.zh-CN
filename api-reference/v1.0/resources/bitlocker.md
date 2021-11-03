---
title: bitLocker 资源
description: 包含实际恢复密钥的导航属性 bitlockerRecoveryKey 的已存储 BitLocker 密钥的父资源。
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ac73c0e7237f4d41217cb53c2c4c33d8cfcdb784
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689073"
---
# <a name="bitlocker-resource-type"></a>bitlocker 资源类型

命名空间：microsoft.graph

包含实际恢复密钥的导航属性 **bitlockerRecoveryKey** 的已存储 BitLocker 密钥的父资源。

## <a name="methods"></a>方法
无。

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

