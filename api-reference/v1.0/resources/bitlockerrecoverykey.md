---
title: bitlockerRecoveryKey 资源类型
description: BitLocker 恢复密钥资源
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8805b8cd633558145787f6a3c4f941fcabad0c62
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696138"
---
# <a name="bitlockerrecoverykey-resource-type"></a>bitlockerRecoveryKey 资源类型

命名空间：microsoft.graph

表示通过 key 属性包含实际恢复密钥的已存储 BitLocker **密钥。**

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 recoveryKeys](../api/bitlocker-list-recoverykeys.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合|获取 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象及其属性的列表。|
|[获取 bitlockerRecoveryKey](../api/bitlockerrecoverykey-get.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|检索 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象的属性和关系。 注意： **默认情况下** 不返回 key 属性。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|最初备份密钥的日期和时间Azure Active Directory。 不可为 null。|
|deviceId|String|最初备份 BitLocker 密钥的设备标识符。 支持 `$filter`（`eq`）。|
|id|String|BitLocker 密钥的唯一标识符。|
|注册表项|String|BitLocker 恢复密钥。 仅在 `$select` 上返回。 不可为 null。|
|volumeType|volumeType|指示 BitLocker 密钥关联的卷的类型。 可能的值包括 `1` ： (for `operatingSystemVolume` `2`) 、 (for `fixedDataVolume`) 、 (for `3`) `removableDataVolume` `4` `unknownFutureValue` 和 (for) 。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "volumeType": "String",
  "deviceId": "String",
  "key": "String"
}
```

