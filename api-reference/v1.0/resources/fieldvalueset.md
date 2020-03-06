---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
description: 表示 listItem 资源中的列值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4b647de480c9c125d0176993dfeccc85dc3cf0ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531438"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="d1aef-103">FieldValueSet 资源</span><span class="sxs-lookup"><span data-stu-id="d1aef-103">FieldValueSet resource</span></span>

<span data-ttu-id="d1aef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1aef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1aef-105">表示 [listItem](listitem.md) 资源中的列值。</span><span class="sxs-lookup"><span data-stu-id="d1aef-105">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1aef-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1aef-106">JSON representation</span></span>

<span data-ttu-id="d1aef-107">下面是 **fieldValueSet** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1aef-107">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="d1aef-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1aef-108">Properties</span></span>

<span data-ttu-id="d1aef-109">**listItem** 中的每个用户可见字段作为 **fieldValueSet** 中的名称/值对返回。</span><span class="sxs-lookup"><span data-stu-id="d1aef-109">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="d1aef-110">上面是针对包含**作者**、**名称**、**颜色**和**数量**这四列列表的一个示例。</span><span class="sxs-lookup"><span data-stu-id="d1aef-110">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="d1aef-111">默认情况下不返回查找字段（如上述 `Author`）。</span><span class="sxs-lookup"><span data-stu-id="d1aef-111">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="d1aef-112">相反，服务器会返回一个引用查找中锁定的 listItem 的“LookupId”字段（如上述 `AuthorLookupId`）。</span><span class="sxs-lookup"><span data-stu-id="d1aef-112">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="d1aef-113">“LookupId”字段的名称是原始字段名称，后跟 `LookupId`。</span><span class="sxs-lookup"><span data-stu-id="d1aef-113">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="d1aef-114">单个查询中可能请求最多 12 个查找字段。</span><span class="sxs-lookup"><span data-stu-id="d1aef-114">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="d1aef-115">如果请求包含带所需字段的 `select` 语句，服务器将返回查找值。</span><span class="sxs-lookup"><span data-stu-id="d1aef-115">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="d1aef-116">示例：</span><span class="sxs-lookup"><span data-stu-id="d1aef-116">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="d1aef-117">你可以在单个查询中请求最多 12 个查找字段以及任意数量的常规字段。</span><span class="sxs-lookup"><span data-stu-id="d1aef-117">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
