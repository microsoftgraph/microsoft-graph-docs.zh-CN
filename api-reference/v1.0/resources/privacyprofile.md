---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 09c3b8ad246bb8c653f31bfebda6013d8519007c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533955"
---
# <a name="privacyprofile-resource-type"></a>privacyProfile 资源类型

命名空间：microsoft.graph

表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。

## <a name="properties"></a>属性
| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|contactEmail|字符串| 隐私声明联系人的有效 smtp 电子邮件地址。 可选。|
|statementUrl|String| 以 http:// 或 https:// 开头的有效 URL 格式。 最大长度为 255 个字符。 定向到公司隐私声明的 URL。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
