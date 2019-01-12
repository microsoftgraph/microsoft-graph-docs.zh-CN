---
title: educationOneNoteResource 资源类型
description: 'EducationResource 一个子类。 这表示在 OneNote 页面的位置。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b10bef551cdc2dd29a8a20c69d2c4657ee66af4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927917"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="93d31-104">educationOneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="93d31-104">educationOneNoteResource resource type</span></span>

> <span data-ttu-id="93d31-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="93d31-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93d31-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="93d31-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93d31-107">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="93d31-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="93d31-108">这表示在 OneNote 页面的位置。</span><span class="sxs-lookup"><span data-stu-id="93d31-108">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="93d31-109">属性</span><span class="sxs-lookup"><span data-stu-id="93d31-109">Properties</span></span>
| <span data-ttu-id="93d31-110">属性</span><span class="sxs-lookup"><span data-stu-id="93d31-110">Property</span></span>     | <span data-ttu-id="93d31-111">类型</span><span class="sxs-lookup"><span data-stu-id="93d31-111">Type</span></span>   |<span data-ttu-id="93d31-112">Description</span><span class="sxs-lookup"><span data-stu-id="93d31-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93d31-113">pageUrl</span><span class="sxs-lookup"><span data-stu-id="93d31-113">pageUrl</span></span>|<span data-ttu-id="93d31-114">字符串</span><span class="sxs-lookup"><span data-stu-id="93d31-114">String</span></span>|<span data-ttu-id="93d31-115">在 OneNote 中页的 Microsoft Graph URL。</span><span class="sxs-lookup"><span data-stu-id="93d31-115">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="93d31-116">sectionName</span><span class="sxs-lookup"><span data-stu-id="93d31-116">sectionName</span></span>|<span data-ttu-id="93d31-117">字符串</span><span class="sxs-lookup"><span data-stu-id="93d31-117">String</span></span>|<span data-ttu-id="93d31-118">分配应复制到或已复制到的部分名称。</span><span class="sxs-lookup"><span data-stu-id="93d31-118">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93d31-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93d31-119">JSON representation</span></span>

<span data-ttu-id="93d31-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93d31-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
