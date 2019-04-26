---
title: educationOneNoteResource 资源类型
description: 'educationResource 的子类。 这表示 OneNote 页面的位置。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1d7796941edebe6ad1cb126d58b5e7600373ee0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340546"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="10c40-104">educationOneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="10c40-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10c40-105">[educationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="10c40-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="10c40-106">这表示 OneNote 页面的位置。</span><span class="sxs-lookup"><span data-stu-id="10c40-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="10c40-107">属性</span><span class="sxs-lookup"><span data-stu-id="10c40-107">Properties</span></span>
| <span data-ttu-id="10c40-108">属性</span><span class="sxs-lookup"><span data-stu-id="10c40-108">Property</span></span>     | <span data-ttu-id="10c40-109">类型</span><span class="sxs-lookup"><span data-stu-id="10c40-109">Type</span></span>   |<span data-ttu-id="10c40-110">说明</span><span class="sxs-lookup"><span data-stu-id="10c40-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10c40-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="10c40-111">pageUrl</span></span>|<span data-ttu-id="10c40-112">String</span><span class="sxs-lookup"><span data-stu-id="10c40-112">String</span></span>|<span data-ttu-id="10c40-113">OneNote 中页面的 Microsoft Graph URL。</span><span class="sxs-lookup"><span data-stu-id="10c40-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="10c40-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="10c40-114">sectionName</span></span>|<span data-ttu-id="10c40-115">String</span><span class="sxs-lookup"><span data-stu-id="10c40-115">String</span></span>|<span data-ttu-id="10c40-116">应将分配复制到中或复制到中的部分名称。</span><span class="sxs-lookup"><span data-stu-id="10c40-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10c40-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10c40-117">JSON representation</span></span>

<span data-ttu-id="10c40-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10c40-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
