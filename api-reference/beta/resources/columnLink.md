---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: c6fc12dcfaeffcb3cd4fb08a6863611ae33541d5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341415"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="bf54c-102">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf54c-102">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf54c-103">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="bf54c-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="bf54c-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf54c-105">JSON representation</span></span>

<span data-ttu-id="bf54c-106">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf54c-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="bf54c-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf54c-107">Properties</span></span>

| <span data-ttu-id="bf54c-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="bf54c-108">Property name</span></span> | <span data-ttu-id="bf54c-109">类型</span><span class="sxs-lookup"><span data-stu-id="bf54c-109">Type</span></span>   | <span data-ttu-id="bf54c-110">说明</span><span class="sxs-lookup"><span data-stu-id="bf54c-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="bf54c-111">**id**</span><span class="sxs-lookup"><span data-stu-id="bf54c-111">**id**</span></span>        | <span data-ttu-id="bf54c-112">string</span><span class="sxs-lookup"><span data-stu-id="bf54c-112">string</span></span> | <span data-ttu-id="bf54c-113">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bf54c-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="bf54c-114">**name**</span><span class="sxs-lookup"><span data-stu-id="bf54c-114">**name**</span></span>      | <span data-ttu-id="bf54c-115">string</span><span class="sxs-lookup"><span data-stu-id="bf54c-115">string</span></span> | <span data-ttu-id="bf54c-116">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="bf54c-116">The name of the column  in this content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->
