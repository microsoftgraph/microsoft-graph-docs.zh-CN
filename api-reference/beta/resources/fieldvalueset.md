---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: 7108c47aecf842f31382ad170fbb058a1aabb39d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815657"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="a4692-102">FieldValueSet 资源</span><span class="sxs-lookup"><span data-stu-id="a4692-102">FieldValueSet resource</span></span>

> <span data-ttu-id="a4692-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4692-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4692-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4692-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4692-105">表示 [listItem](listitem.md) 资源中的列值。</span><span class="sxs-lookup"><span data-stu-id="a4692-105">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4692-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4692-106">JSON representation</span></span>

<span data-ttu-id="a4692-107">下面是 **fieldValueSet** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4692-107">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="a4692-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4692-108">Properties</span></span>

<span data-ttu-id="a4692-109">**listItem** 中的每个用户可见字段作为 **fieldValueSet** 中的名称/值对返回。</span><span class="sxs-lookup"><span data-stu-id="a4692-109">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="a4692-110">上面是针对包含**作者**、**名称**、**颜色**和**数量**这四列列表的一个示例。</span><span class="sxs-lookup"><span data-stu-id="a4692-110">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="a4692-111">默认情况下不返回查找字段（如上述 `Author`）。</span><span class="sxs-lookup"><span data-stu-id="a4692-111">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="a4692-112">相反，服务器会返回一个引用查找中锁定的 listItem 的“LookupId”字段（如上述 `AuthorLookupId`）。</span><span class="sxs-lookup"><span data-stu-id="a4692-112">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="a4692-113">“LookupId”字段的名称是原始字段名称，后跟 `LookupId`。</span><span class="sxs-lookup"><span data-stu-id="a4692-113">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="a4692-114">单个查询中可能请求最多 12 个查找字段。</span><span class="sxs-lookup"><span data-stu-id="a4692-114">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="a4692-115">如果请求包含带所需字段的 `select` 语句，服务器将返回查找值。</span><span class="sxs-lookup"><span data-stu-id="a4692-115">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="a4692-116">示例：</span><span class="sxs-lookup"><span data-stu-id="a4692-116">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="a4692-117">你可以在单个查询中请求最多 12 个查找字段以及任意数量的常规字段。</span><span class="sxs-lookup"><span data-stu-id="a4692-117">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
