# <a name="recentnotebook-resource-type"></a><span data-ttu-id="71991-101">recentNotebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="71991-101">recentNotebook resource type</span></span>

<span data-ttu-id="71991-102">最近访问过的 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="71991-102">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="71991-103">**recentNotebook** 类似于 [notebook](notebook.md)，不同之处在于属性较少。</span><span class="sxs-lookup"><span data-stu-id="71991-103">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="71991-104">属性</span><span class="sxs-lookup"><span data-stu-id="71991-104">Properties</span></span>
| <span data-ttu-id="71991-105">属性</span><span class="sxs-lookup"><span data-stu-id="71991-105">Property</span></span>     | <span data-ttu-id="71991-106">类型</span><span class="sxs-lookup"><span data-stu-id="71991-106">Type</span></span>   |<span data-ttu-id="71991-107">说明</span><span class="sxs-lookup"><span data-stu-id="71991-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71991-108">displayName</span><span class="sxs-lookup"><span data-stu-id="71991-108">displayName</span></span>|<span data-ttu-id="71991-109">字符串</span><span class="sxs-lookup"><span data-stu-id="71991-109">String</span></span>|<span data-ttu-id="71991-110">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="71991-110">The name of the notebook.</span></span>|
|<span data-ttu-id="71991-111">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="71991-111">lastAccessedTime</span></span>|<span data-ttu-id="71991-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71991-112">DateTimeOffset</span></span>|<span data-ttu-id="71991-p102">上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="71991-p102">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="71991-117">links</span><span class="sxs-lookup"><span data-stu-id="71991-117">links</span></span>|[<span data-ttu-id="71991-118">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="71991-118">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="71991-119">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="71991-119">Links for opening the notebook.</span></span> <span data-ttu-id="71991-120">链接可以在 OneNote 客户端（如果已安装的话）中打开笔记本。`oneNoteClientURL`</span><span class="sxs-lookup"><span data-stu-id="71991-120">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="71991-121">链接可以在 OneNote Online 中打开笔记本。`oneNoteWebURL`</span><span class="sxs-lookup"><span data-stu-id="71991-121">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="71991-122">sourceService</span><span class="sxs-lookup"><span data-stu-id="71991-122">sourceService</span></span>|<span data-ttu-id="71991-123">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="71991-123">onenoteSourceService values</span></span>|<span data-ttu-id="71991-124">笔记本驻留的后端存储，可以是 `OneDriveForBusiness` 或 `OneDrive`。</span><span class="sxs-lookup"><span data-stu-id="71991-124">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71991-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71991-125">JSON representation</span></span>

<span data-ttu-id="71991-126">下面是此资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71991-126">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="71991-127">方法</span><span class="sxs-lookup"><span data-stu-id="71991-127">Methods</span></span>

| <span data-ttu-id="71991-128">方法</span><span class="sxs-lookup"><span data-stu-id="71991-128">Method</span></span>           | <span data-ttu-id="71991-129">返回类型</span><span class="sxs-lookup"><span data-stu-id="71991-129">Return Type</span></span>    |<span data-ttu-id="71991-130">说明</span><span class="sxs-lookup"><span data-stu-id="71991-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71991-131">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="71991-131">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="71991-132">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71991-132">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="71991-133">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="71991-133">Get a collection of the most recently accessed notebooks for the user.</span></span> |
