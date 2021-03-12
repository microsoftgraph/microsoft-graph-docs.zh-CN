---
title: recentNotebook 资源类型
description: 最近访问过的 OneNote 笔记本。 **recentNotebook** 类似于 notebook，不同之处在于属性较少。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6f096aff01104e36b25e42725c462735f024fc82
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722417"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="68e26-104">recentNotebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="68e26-104">recentNotebook resource type</span></span>

<span data-ttu-id="68e26-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68e26-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68e26-106">最近访问过的 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="68e26-106">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="68e26-107">**recentNotebook** 类似于 [notebook](notebook.md)，不同之处在于属性较少。</span><span class="sxs-lookup"><span data-stu-id="68e26-107">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="68e26-108">属性</span><span class="sxs-lookup"><span data-stu-id="68e26-108">Properties</span></span>
| <span data-ttu-id="68e26-109">属性</span><span class="sxs-lookup"><span data-stu-id="68e26-109">Property</span></span>     | <span data-ttu-id="68e26-110">类型</span><span class="sxs-lookup"><span data-stu-id="68e26-110">Type</span></span>   |<span data-ttu-id="68e26-111">说明</span><span class="sxs-lookup"><span data-stu-id="68e26-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68e26-112">displayName</span><span class="sxs-lookup"><span data-stu-id="68e26-112">displayName</span></span>|<span data-ttu-id="68e26-113">字符串</span><span class="sxs-lookup"><span data-stu-id="68e26-113">String</span></span>|<span data-ttu-id="68e26-114">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="68e26-114">The name of the notebook.</span></span>|
|<span data-ttu-id="68e26-115">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="68e26-115">lastAccessedTime</span></span>|<span data-ttu-id="68e26-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e26-116">DateTimeOffset</span></span>|<span data-ttu-id="68e26-117">上次修改笔记本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="68e26-117">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="68e26-118">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="68e26-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68e26-119">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="68e26-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="68e26-120">只读。</span><span class="sxs-lookup"><span data-stu-id="68e26-120">Read-only.</span></span>|
|<span data-ttu-id="68e26-121">links</span><span class="sxs-lookup"><span data-stu-id="68e26-121">links</span></span>|[<span data-ttu-id="68e26-122">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="68e26-122">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="68e26-123">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="68e26-123">Links for opening the notebook.</span></span> <span data-ttu-id="68e26-124">`oneNoteClientURL` 链接可以在 OneNote 客户端（如果已安装的话）中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="68e26-124">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="68e26-125">该 `oneNoteWebURL` 链接在 OneNote 网页中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="68e26-125">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="68e26-126">sourceService</span><span class="sxs-lookup"><span data-stu-id="68e26-126">sourceService</span></span>|<span data-ttu-id="68e26-127">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="68e26-127">onenoteSourceService</span></span>|<span data-ttu-id="68e26-128">笔记本驻留的后端存储，可以是 `OneDriveForBusiness` 或 `OneDrive`。</span><span class="sxs-lookup"><span data-stu-id="68e26-128">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68e26-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68e26-129">JSON representation</span></span>

<span data-ttu-id="68e26-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68e26-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}
```

## <a name="methods"></a><span data-ttu-id="68e26-131">Methods</span><span class="sxs-lookup"><span data-stu-id="68e26-131">Methods</span></span>

| <span data-ttu-id="68e26-132">方法</span><span class="sxs-lookup"><span data-stu-id="68e26-132">Method</span></span>           | <span data-ttu-id="68e26-133">返回类型</span><span class="sxs-lookup"><span data-stu-id="68e26-133">Return Type</span></span>    |<span data-ttu-id="68e26-134">说明</span><span class="sxs-lookup"><span data-stu-id="68e26-134">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68e26-135">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="68e26-135">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="68e26-136">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68e26-136">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="68e26-137">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="68e26-137">Get a collection of the most recently accessed notebooks for the user.</span></span> |

