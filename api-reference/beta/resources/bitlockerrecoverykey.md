---
title: bitlockerRecoveryKey 资源类型
description: BitLocker 恢复密钥资源
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 038feb77f7ca57d426a44c04b3d9c93ae29e5aa4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081973"
---
# <a name="bitlockerrecoverykey-resource-type"></a>bitlockerRecoveryKey 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个存储的 BitLocker 密钥，其中包含通过 **key** 属性的实际恢复密钥。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 recoveryKeys](../api/bitlocker-list-recoverykeys.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合|获取 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象及其属性的列表。|
|[获取 bitlockerRecoveryKey](../api/bitlockerrecoverykey-get.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|检索 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象的属性和关系。 注意：默认情况下不返回 **key** 属性。|

> **注意**：只有某些角色具有调用这些 api 的权限。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|密钥最初备份到 Azure Active Directory 的日期和时间。|
|deviceId|String|BitLocker 密钥最初备份的设备的 ID。|
|id|String|BitLocker 密钥的唯一标识符。|
|注册表项|String|BitLocker 恢复密钥。|
|volumeType|volumeType|指示与 BitLocker 密钥相关联的卷的类型。 可取值为：`operatingSystemVolume`、`fixedDataVolume`、`removableDataVolume`、`unknownFutureValue`。|

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
  "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
  "createdDateTime": "2020-06-15T13:45:30.0000000Z",
  "volumeType": 1,
  "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
  "key": "123456-231453-873456-213546-654678-765689-123456-324565"
}
```

