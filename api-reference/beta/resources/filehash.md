---
title: fileHash 资源类型
description: 包含有关文件哈希 (加密和位置敏感) 的状态信息。
localization_priority: Normal
ms.openlocfilehash: f5d865a7ded230ca611b8628c3648ec1e331c67d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547604"
---
# <a name="filehash-resource-type"></a>fileHash 资源类型

包含有关文件哈希 (加密和位置敏感) 的状态信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hashType|[fileHashType](filehashtypeenumtype.md)枚举|文件哈希类型。 可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256`。|
|hashValue|String|文件哈希值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
