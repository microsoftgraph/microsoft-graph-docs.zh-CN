---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 2c224e4e9db87f8da98ef34296cc193eb2fb564c
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849756"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="1bda6-103">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="1bda6-103">itemBody resource type</span></span>

<span data-ttu-id="1bda6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bda6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bda6-105">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="1bda6-105">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="1bda6-106">属性</span><span class="sxs-lookup"><span data-stu-id="1bda6-106">Properties</span></span>
| <span data-ttu-id="1bda6-107">属性</span><span class="sxs-lookup"><span data-stu-id="1bda6-107">Property</span></span>     | <span data-ttu-id="1bda6-108">类型</span><span class="sxs-lookup"><span data-stu-id="1bda6-108">Type</span></span>   |<span data-ttu-id="1bda6-109">说明</span><span class="sxs-lookup"><span data-stu-id="1bda6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bda6-110">内容</span><span class="sxs-lookup"><span data-stu-id="1bda6-110">content</span></span>|<span data-ttu-id="1bda6-111">String</span><span class="sxs-lookup"><span data-stu-id="1bda6-111">String</span></span>|<span data-ttu-id="1bda6-112">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="1bda6-112">The content of the item.</span></span>|
|<span data-ttu-id="1bda6-113">contentType</span><span class="sxs-lookup"><span data-stu-id="1bda6-113">contentType</span></span>|<span data-ttu-id="1bda6-114">String</span><span class="sxs-lookup"><span data-stu-id="1bda6-114">String</span></span>|<span data-ttu-id="1bda6-p101">内容的类型。可能的值为 `text` 和 `html`。</span><span class="sxs-lookup"><span data-stu-id="1bda6-p101">The type of the content. Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1bda6-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1bda6-117">JSON representation</span></span>

<span data-ttu-id="1bda6-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bda6-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
