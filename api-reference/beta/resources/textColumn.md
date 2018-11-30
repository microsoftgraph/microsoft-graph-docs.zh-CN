---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 5ff280b6c969d9832e2f81f77dc32237f9905aad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044968"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="96ceb-102">TextColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="96ceb-102">TextColumn resource type</span></span>

> <span data-ttu-id="96ceb-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="96ceb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96ceb-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="96ceb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96ceb-105">[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。</span><span class="sxs-lookup"><span data-stu-id="96ceb-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96ceb-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96ceb-106">JSON representation</span></span>

<span data-ttu-id="96ceb-107">下面是 **textColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96ceb-107">Here is a JSON representation of a **textColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a><span data-ttu-id="96ceb-108">属性</span><span class="sxs-lookup"><span data-stu-id="96ceb-108">Properties</span></span>

| <span data-ttu-id="96ceb-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="96ceb-109">Property name</span></span>                   | <span data-ttu-id="96ceb-110">类型</span><span class="sxs-lookup"><span data-stu-id="96ceb-110">Type</span></span>   | <span data-ttu-id="96ceb-111">说明</span><span class="sxs-lookup"><span data-stu-id="96ceb-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="96ceb-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="96ceb-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="96ceb-113">string</span><span class="sxs-lookup"><span data-stu-id="96ceb-113">string</span></span> | <span data-ttu-id="96ceb-114">是否支持多行文本。</span><span class="sxs-lookup"><span data-stu-id="96ceb-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="96ceb-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="96ceb-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="96ceb-116">string</span><span class="sxs-lookup"><span data-stu-id="96ceb-116">string</span></span> | <span data-ttu-id="96ceb-117">对此列的更新应替换现有文本，还是附加到现有文本。</span><span class="sxs-lookup"><span data-stu-id="96ceb-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="96ceb-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="96ceb-118">**linesForEditing**</span></span>             | <span data-ttu-id="96ceb-119">整数</span><span class="sxs-lookup"><span data-stu-id="96ceb-119">int</span></span>    | <span data-ttu-id="96ceb-120">文本框的大小。</span><span class="sxs-lookup"><span data-stu-id="96ceb-120">The size of the text box.</span></span>
| <span data-ttu-id="96ceb-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="96ceb-121">**maxLength**</span></span>                   | <span data-ttu-id="96ceb-122">整数</span><span class="sxs-lookup"><span data-stu-id="96ceb-122">int</span></span>    | <span data-ttu-id="96ceb-123">值的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="96ceb-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="96ceb-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="96ceb-124">**textType**</span></span>                    | <span data-ttu-id="96ceb-125">string</span><span class="sxs-lookup"><span data-stu-id="96ceb-125">string</span></span> | <span data-ttu-id="96ceb-126">要存储的文本类型。</span><span class="sxs-lookup"><span data-stu-id="96ceb-126">The type of text being stored.</span></span> <span data-ttu-id="96ceb-127">必须为 `plain` 或 `richText`.的其中一个</span><span class="sxs-lookup"><span data-stu-id="96ceb-127">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
