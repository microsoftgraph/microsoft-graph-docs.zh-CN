---
title: recentNotebook 资源类型
description: 最近访问过的 OneNote 笔记本。 **recentNotebook** 类似于 notebook，不同之处在于属性较少。
ms.openlocfilehash: c3b717fcebdc229864aefe13c6452ce5eb95fc53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045216"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="d093f-104">recentNotebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="d093f-104">recentNotebook resource type</span></span>

> <span data-ttu-id="d093f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d093f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d093f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d093f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d093f-107">最近访问过的 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="d093f-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="d093f-108">**recentNotebook** 类似于 [notebook](notebook.md)，不同之处在于属性较少。</span><span class="sxs-lookup"><span data-stu-id="d093f-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="d093f-109">属性</span><span class="sxs-lookup"><span data-stu-id="d093f-109">Properties</span></span>
| <span data-ttu-id="d093f-110">属性</span><span class="sxs-lookup"><span data-stu-id="d093f-110">Property</span></span>     | <span data-ttu-id="d093f-111">类型</span><span class="sxs-lookup"><span data-stu-id="d093f-111">Type</span></span>   |<span data-ttu-id="d093f-112">说明</span><span class="sxs-lookup"><span data-stu-id="d093f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d093f-113">name</span><span class="sxs-lookup"><span data-stu-id="d093f-113">name</span></span>|<span data-ttu-id="d093f-114">字符串</span><span class="sxs-lookup"><span data-stu-id="d093f-114">String</span></span>|<span data-ttu-id="d093f-115">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="d093f-115">The name of the notebook.</span></span>|
|<span data-ttu-id="d093f-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="d093f-116">lastAccessedTime</span></span>|<span data-ttu-id="d093f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d093f-117">DateTimeOffset</span></span>|<span data-ttu-id="d093f-p104">上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="d093f-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="d093f-122">links</span><span class="sxs-lookup"><span data-stu-id="d093f-122">links</span></span>|[<span data-ttu-id="d093f-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="d093f-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="d093f-124">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="d093f-124">Links for opening the notebook.</span></span> <span data-ttu-id="d093f-125">`oneNoteClientURL` 链接可以在 OneNote 客户端（如果已安装的话）中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="d093f-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="d093f-126">`oneNoteWebURL` 链接可以在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="d093f-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="d093f-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="d093f-127">sourceService</span></span>|<span data-ttu-id="d093f-128">String</span><span class="sxs-lookup"><span data-stu-id="d093f-128">String</span></span>|<span data-ttu-id="d093f-129">笔记本驻留的后端存储，可以是 `OneDriveForBusiness` 或 `OneDrive`。</span><span class="sxs-lookup"><span data-stu-id="d093f-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d093f-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d093f-130">JSON representation</span></span>

<span data-ttu-id="d093f-131">下面是此资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d093f-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="d093f-132">方法</span><span class="sxs-lookup"><span data-stu-id="d093f-132">Methods</span></span>

| <span data-ttu-id="d093f-133">方法</span><span class="sxs-lookup"><span data-stu-id="d093f-133">Method</span></span>           | <span data-ttu-id="d093f-134">返回类型</span><span class="sxs-lookup"><span data-stu-id="d093f-134">Return Type</span></span>    |<span data-ttu-id="d093f-135">说明</span><span class="sxs-lookup"><span data-stu-id="d093f-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d093f-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="d093f-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="d093f-137">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d093f-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="d093f-138">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="d093f-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
