---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: 226666875b9364f33954e7f932227562a9734267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888569"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="0da15-102">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="0da15-102">ColumnLink resource type</span></span>

> <span data-ttu-id="0da15-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0da15-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0da15-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0da15-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0da15-105">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="0da15-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="0da15-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0da15-107">JSON representation</span></span>

<span data-ttu-id="0da15-108">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0da15-108">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0da15-109">属性</span><span class="sxs-lookup"><span data-stu-id="0da15-109">Properties</span></span>

| <span data-ttu-id="0da15-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="0da15-110">Property name</span></span> | <span data-ttu-id="0da15-111">类型</span><span class="sxs-lookup"><span data-stu-id="0da15-111">Type</span></span>   | <span data-ttu-id="0da15-112">说明</span><span class="sxs-lookup"><span data-stu-id="0da15-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="0da15-113">**id**</span><span class="sxs-lookup"><span data-stu-id="0da15-113">**id**</span></span>        | <span data-ttu-id="0da15-114">string</span><span class="sxs-lookup"><span data-stu-id="0da15-114">string</span></span> | <span data-ttu-id="0da15-115">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0da15-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="0da15-116">**name**</span><span class="sxs-lookup"><span data-stu-id="0da15-116">**name**</span></span>      | <span data-ttu-id="0da15-117">string</span><span class="sxs-lookup"><span data-stu-id="0da15-117">string</span></span> | <span data-ttu-id="0da15-118">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="0da15-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
