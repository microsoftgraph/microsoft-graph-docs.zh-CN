---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
description: 表示 listItem 资源中的列值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a1a308bfcda1bf913455ca6689dbaca308daecbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032520"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="f1d4f-103">FieldValueSet 资源</span><span class="sxs-lookup"><span data-stu-id="f1d4f-103">FieldValueSet resource</span></span>

<span data-ttu-id="f1d4f-104">表示 [listItem](listitem.md) 资源中的列值。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-104">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1d4f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1d4f-105">JSON representation</span></span>

<span data-ttu-id="f1d4f-106">下面是 **fieldValueSet** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-106">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
      "optionalProperties": ["Author", "AuthorLookupId", "Name", "Color", "Quantity" ],
       "baseType": "microsoft.graph.entity", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="f1d4f-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1d4f-107">Properties</span></span>

<span data-ttu-id="f1d4f-108">**listItem** 中的每个用户可见字段作为 **fieldValueSet** 中的名称/值对返回。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-108">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="f1d4f-109">上面是针对包含**作者**、**名称**、**颜色**和**数量**这四列列表的一个示例。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-109">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="f1d4f-110">默认情况下不返回查找字段（如上述 `Author`）。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-110">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="f1d4f-111">相反，服务器会返回一个引用查找中锁定的 listItem 的“LookupId”字段（如上述 `AuthorLookupId`）。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-111">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="f1d4f-112">“LookupId”字段的名称是原始字段名称，后跟 `LookupId`。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-112">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="f1d4f-113">单个查询中可能请求最多 12 个查找字段。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-113">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="f1d4f-114">如果请求包含带所需字段的 `select` 语句，服务器将返回查找值。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-114">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="f1d4f-115">示例：</span><span class="sxs-lookup"><span data-stu-id="f1d4f-115">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="f1d4f-116">你可以在单个查询中请求最多 12 个查找字段以及任意数量的常规字段。</span><span class="sxs-lookup"><span data-stu-id="f1d4f-116">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
