---
title: recentNotebook 资源类型
description: 最近访问过的 OneNote 笔记本。 **recentNotebook** 类似于 notebook，不同之处在于属性较少。
ms.openlocfilehash: 7beeb23926210d5b8c2c364ceb81726c5a28becb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011423"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="32ff4-104">recentNotebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="32ff4-104">recentNotebook resource type</span></span>

<span data-ttu-id="32ff4-105">最近访问过的 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="32ff4-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="32ff4-106">**recentNotebook** 类似于 [notebook](notebook.md)，不同之处在于属性较少。</span><span class="sxs-lookup"><span data-stu-id="32ff4-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="32ff4-107">属性</span><span class="sxs-lookup"><span data-stu-id="32ff4-107">Properties</span></span>
| <span data-ttu-id="32ff4-108">属性</span><span class="sxs-lookup"><span data-stu-id="32ff4-108">Property</span></span>     | <span data-ttu-id="32ff4-109">类型</span><span class="sxs-lookup"><span data-stu-id="32ff4-109">Type</span></span>   |<span data-ttu-id="32ff4-110">说明</span><span class="sxs-lookup"><span data-stu-id="32ff4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32ff4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="32ff4-111">displayName</span></span>|<span data-ttu-id="32ff4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="32ff4-112">String</span></span>|<span data-ttu-id="32ff4-113">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="32ff4-113">The name of the notebook.</span></span>|
|<span data-ttu-id="32ff4-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="32ff4-114">lastAccessedTime</span></span>|<span data-ttu-id="32ff4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32ff4-115">DateTimeOffset</span></span>|<span data-ttu-id="32ff4-p103">上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="32ff4-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="32ff4-120">links</span><span class="sxs-lookup"><span data-stu-id="32ff4-120">links</span></span>|[<span data-ttu-id="32ff4-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="32ff4-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="32ff4-122">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="32ff4-122">Links for opening the notebook.</span></span> <span data-ttu-id="32ff4-123">`oneNoteClientURL` 链接可以在 OneNote 客户端（如果已安装的话）中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="32ff4-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="32ff4-124">`oneNoteWebURL` 链接可以在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="32ff4-124">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="32ff4-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="32ff4-125">sourceService</span></span>|<span data-ttu-id="32ff4-126">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="32ff4-126">onenoteSourceService</span></span>|<span data-ttu-id="32ff4-127">笔记本驻留的后端存储，可以是 `OneDriveForBusiness` 或 `OneDrive`。</span><span class="sxs-lookup"><span data-stu-id="32ff4-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32ff4-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32ff4-128">JSON representation</span></span>

<span data-ttu-id="32ff4-129">下面是此资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32ff4-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="32ff4-130">方法</span><span class="sxs-lookup"><span data-stu-id="32ff4-130">Methods</span></span>

| <span data-ttu-id="32ff4-131">方法</span><span class="sxs-lookup"><span data-stu-id="32ff4-131">Method</span></span>           | <span data-ttu-id="32ff4-132">返回类型</span><span class="sxs-lookup"><span data-stu-id="32ff4-132">Return Type</span></span>    |<span data-ttu-id="32ff4-133">说明</span><span class="sxs-lookup"><span data-stu-id="32ff4-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32ff4-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="32ff4-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="32ff4-135">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32ff4-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="32ff4-136">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="32ff4-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
