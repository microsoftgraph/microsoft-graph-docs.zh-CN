---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
ms.localizationpriority: medium
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 26b4899d01f37307158220059791ff6edac8322d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036002"
---
# <a name="privacyprofile-resource-type"></a>privacyProfile 资源类型

命名空间：microsoft.graph

表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。

## <a name="properties"></a>属性
| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|contactEmail|String| 隐私声明联系人的有效 smtp 电子邮件地址。 可选。|
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

