---
title: educationOneNoteResource 资源类型
description: 'EducationResource 的子类。 这表示 OneNote 页面的位置。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cec9c2f2a092175c7ccecaa09c7b8b510000205c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501547"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="2ec7a-104">educationOneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ec7a-104">educationOneNoteResource resource type</span></span>

<span data-ttu-id="2ec7a-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2ec7a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ec7a-106">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="2ec7a-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2ec7a-107">这表示 OneNote 页面的位置。</span><span class="sxs-lookup"><span data-stu-id="2ec7a-107">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="2ec7a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ec7a-108">Properties</span></span>
| <span data-ttu-id="2ec7a-109">属性</span><span class="sxs-lookup"><span data-stu-id="2ec7a-109">Property</span></span>     | <span data-ttu-id="2ec7a-110">类型</span><span class="sxs-lookup"><span data-stu-id="2ec7a-110">Type</span></span>   |<span data-ttu-id="2ec7a-111">说明</span><span class="sxs-lookup"><span data-stu-id="2ec7a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ec7a-112">pageUrl</span><span class="sxs-lookup"><span data-stu-id="2ec7a-112">pageUrl</span></span>|<span data-ttu-id="2ec7a-113">String</span><span class="sxs-lookup"><span data-stu-id="2ec7a-113">String</span></span>|<span data-ttu-id="2ec7a-114">OneNote 中页面的 Microsoft Graph URL。</span><span class="sxs-lookup"><span data-stu-id="2ec7a-114">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="2ec7a-115">sectionName</span><span class="sxs-lookup"><span data-stu-id="2ec7a-115">sectionName</span></span>|<span data-ttu-id="2ec7a-116">String</span><span class="sxs-lookup"><span data-stu-id="2ec7a-116">String</span></span>|<span data-ttu-id="2ec7a-117">应将分配复制到中或复制到中的部分名称。</span><span class="sxs-lookup"><span data-stu-id="2ec7a-117">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ec7a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ec7a-118">JSON representation</span></span>

<span data-ttu-id="2ec7a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ec7a-119">The following is a JSON representation of the resource.</span></span>

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
