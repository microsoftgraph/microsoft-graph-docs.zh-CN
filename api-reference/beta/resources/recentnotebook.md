---
title: recentNotebook 资源类型
description: 最近访问过的 OneNote 笔记本。 **recentNotebook** 类似于 notebook，不同之处在于属性较少。
localization_priority: Normal
ms.openlocfilehash: f2dd1ca642203cde36bb636b9cb2eb7c79344e3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833829"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="a8955-104">recentNotebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8955-104">recentNotebook resource type</span></span>

> <span data-ttu-id="a8955-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a8955-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8955-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8955-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8955-107">最近访问过的 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="a8955-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="a8955-108">**recentNotebook** 类似于 [notebook](notebook.md)，不同之处在于属性较少。</span><span class="sxs-lookup"><span data-stu-id="a8955-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="a8955-109">属性</span><span class="sxs-lookup"><span data-stu-id="a8955-109">Properties</span></span>
| <span data-ttu-id="a8955-110">属性</span><span class="sxs-lookup"><span data-stu-id="a8955-110">Property</span></span>     | <span data-ttu-id="a8955-111">类型</span><span class="sxs-lookup"><span data-stu-id="a8955-111">Type</span></span>   |<span data-ttu-id="a8955-112">说明</span><span class="sxs-lookup"><span data-stu-id="a8955-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8955-113">name</span><span class="sxs-lookup"><span data-stu-id="a8955-113">name</span></span>|<span data-ttu-id="a8955-114">字符串</span><span class="sxs-lookup"><span data-stu-id="a8955-114">String</span></span>|<span data-ttu-id="a8955-115">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="a8955-115">The name of the notebook.</span></span>|
|<span data-ttu-id="a8955-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="a8955-116">lastAccessedTime</span></span>|<span data-ttu-id="a8955-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8955-117">DateTimeOffset</span></span>|<span data-ttu-id="a8955-p104">上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="a8955-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="a8955-122">links</span><span class="sxs-lookup"><span data-stu-id="a8955-122">links</span></span>|[<span data-ttu-id="a8955-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="a8955-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="a8955-124">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="a8955-124">Links for opening the notebook.</span></span> <span data-ttu-id="a8955-125">`oneNoteClientURL` 链接可以在 OneNote 客户端（如果已安装的话）中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="a8955-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="a8955-126">`oneNoteWebURL` 链接可以在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="a8955-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="a8955-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="a8955-127">sourceService</span></span>|<span data-ttu-id="a8955-128">String</span><span class="sxs-lookup"><span data-stu-id="a8955-128">String</span></span>|<span data-ttu-id="a8955-129">笔记本驻留的后端存储，可以是 `OneDriveForBusiness` 或 `OneDrive`。</span><span class="sxs-lookup"><span data-stu-id="a8955-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8955-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8955-130">JSON representation</span></span>

<span data-ttu-id="a8955-131">下面是此资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8955-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="a8955-132">方法</span><span class="sxs-lookup"><span data-stu-id="a8955-132">Methods</span></span>

| <span data-ttu-id="a8955-133">方法</span><span class="sxs-lookup"><span data-stu-id="a8955-133">Method</span></span>           | <span data-ttu-id="a8955-134">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8955-134">Return Type</span></span>    |<span data-ttu-id="a8955-135">说明</span><span class="sxs-lookup"><span data-stu-id="a8955-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8955-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="a8955-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="a8955-137">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8955-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="a8955-138">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="a8955-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
