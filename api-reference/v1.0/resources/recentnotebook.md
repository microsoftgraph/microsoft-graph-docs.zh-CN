# <a name="recentnotebook-resource-type"></a><span data-ttu-id="60785-101">recentNotebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="60785-101">recentNotebook resource type</span></span>

<span data-ttu-id="60785-102">最近访问过的 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="60785-102">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="60785-103">**recentNotebook** 类似于 [notebook](notebook.md)，不同之处在于属性较少。</span><span class="sxs-lookup"><span data-stu-id="60785-103">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="60785-104">属性</span><span class="sxs-lookup"><span data-stu-id="60785-104">Properties</span></span>
| <span data-ttu-id="60785-105">属性</span><span class="sxs-lookup"><span data-stu-id="60785-105">Property</span></span>     | <span data-ttu-id="60785-106">类型</span><span class="sxs-lookup"><span data-stu-id="60785-106">Type</span></span>   |<span data-ttu-id="60785-107">说明</span><span class="sxs-lookup"><span data-stu-id="60785-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60785-108">名称</span><span class="sxs-lookup"><span data-stu-id="60785-108">name</span></span>|<span data-ttu-id="60785-109">字符串</span><span class="sxs-lookup"><span data-stu-id="60785-109">String</span></span>|<span data-ttu-id="60785-110">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="60785-110">The name of the notebook.</span></span>|
|<span data-ttu-id="60785-111">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="60785-111">lastAccessedTime</span></span>|<span data-ttu-id="60785-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60785-112">DateTimeOffset</span></span>|<span data-ttu-id="60785-113">上次修改笔记本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="60785-113">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="60785-114">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="60785-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="60785-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="60785-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="60785-116">只读。</span><span class="sxs-lookup"><span data-stu-id="60785-116">Read-only.</span></span>|
|<span data-ttu-id="60785-117">links</span><span class="sxs-lookup"><span data-stu-id="60785-117">links</span></span>|[<span data-ttu-id="60785-118">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="60785-118">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="60785-119">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="60785-119">Links for opening the notebook.</span></span> <span data-ttu-id="60785-120">`oneNoteClientURL` 链接可以在 OneNote 客户端（如果已安装的话）中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="60785-120">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="60785-121">`oneNoteWebURL` 链接可以在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="60785-121">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="60785-122">sourceService</span><span class="sxs-lookup"><span data-stu-id="60785-122">sourceService</span></span>|<span data-ttu-id="60785-123">String</span><span class="sxs-lookup"><span data-stu-id="60785-123">String</span></span>|<span data-ttu-id="60785-124">笔记本驻留的后端存储，可以是 `OneDriveForBusiness` 或 `OneDrive`。</span><span class="sxs-lookup"><span data-stu-id="60785-124">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60785-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60785-125">JSON representation</span></span>

<span data-ttu-id="60785-126">下面是此资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60785-126">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="60785-127">方法</span><span class="sxs-lookup"><span data-stu-id="60785-127">Methods</span></span>

| <span data-ttu-id="60785-128">方法</span><span class="sxs-lookup"><span data-stu-id="60785-128">Method</span></span>           | <span data-ttu-id="60785-129">返回类型</span><span class="sxs-lookup"><span data-stu-id="60785-129">Return Type</span></span>    |<span data-ttu-id="60785-130">说明</span><span class="sxs-lookup"><span data-stu-id="60785-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60785-131">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="60785-131">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="60785-132">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60785-132">[Notebook](notebook.md) collection</span></span> | <span data-ttu-id="60785-133">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="60785-133">Get a collection of the most recently accessed notebooks for the user.</span></span> |
