---
title: yomiPersonName 资源类型
description: yomiPersonName 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 926479832db04e427e7ca1d73744008db7dc6aaa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079625"
---
# <a name="yomipersonname-resource-type"></a>yomiPersonName 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为用户提供了一种机制，用于存储有关如何对表示 [contact.personname](personname.md) 资源的语言的非本机扬声器的名称进行发音的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |String       | 姓和名的发音参考线组合。  |
|前         |String       | 用户名字的发音指南。     |
|末          |String       | 用户姓氏的发音指南。      |
|maiden        |String       | 用户的 maiden 名称的发音指南。    |
|中间        |String       | 用户中间名的发音指南。    |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yomiPersonName"
}
-->

``` json

{
  "displayName": "String",
  "first": "String",
  "maiden": "String",
  "middle": "String",
  "last": "String"
}
```


