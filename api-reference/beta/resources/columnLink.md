---
author: daspek
description: contentType 上的 columnLink 将网站 columnDefinition 附加到该内容类型。
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4add6ac0edc401815d8072371ce0faca48d5852b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012942"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="93f5c-103">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="93f5c-103">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93f5c-104">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="93f5c-104">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="93f5c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93f5c-106">JSON representation</span></span>

<span data-ttu-id="93f5c-107">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93f5c-107">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="93f5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="93f5c-108">Properties</span></span>

| <span data-ttu-id="93f5c-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="93f5c-109">Property name</span></span> | <span data-ttu-id="93f5c-110">类型</span><span class="sxs-lookup"><span data-stu-id="93f5c-110">Type</span></span>   | <span data-ttu-id="93f5c-111">说明</span><span class="sxs-lookup"><span data-stu-id="93f5c-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="93f5c-112">**id**</span><span class="sxs-lookup"><span data-stu-id="93f5c-112">**id**</span></span>        | <span data-ttu-id="93f5c-113">string</span><span class="sxs-lookup"><span data-stu-id="93f5c-113">string</span></span> | <span data-ttu-id="93f5c-114">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="93f5c-114">The unique identifier for the column.</span></span>
| <span data-ttu-id="93f5c-115">**name**</span><span class="sxs-lookup"><span data-stu-id="93f5c-115">**name**</span></span>      | <span data-ttu-id="93f5c-116">string</span><span class="sxs-lookup"><span data-stu-id="93f5c-116">string</span></span> | <span data-ttu-id="93f5c-117">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="93f5c-117">The name of the column  in this content type.</span></span>

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
