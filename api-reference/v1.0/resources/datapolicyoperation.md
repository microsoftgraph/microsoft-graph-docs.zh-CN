# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="0db25-101">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="0db25-101">dataPolicyOperation resource type</span></span>

<span data-ttu-id="0db25-102">代表提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="0db25-102">Represents a submitted data policy operation.</span></span> <span data-ttu-id="0db25-103">它包含跟踪操作的状态所需的信息。</span><span class="sxs-lookup"><span data-stu-id="0db25-103">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="0db25-104">例如，公司管理员可以提交数据策略操作请求员工的公司数据导出，然后更高版本跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="0db25-104">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="0db25-105">方法</span><span class="sxs-lookup"><span data-stu-id="0db25-105">Methods</span></span>

| <span data-ttu-id="0db25-106">方法</span><span class="sxs-lookup"><span data-stu-id="0db25-106">Method</span></span>           | <span data-ttu-id="0db25-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="0db25-107">Return Type</span></span>    |<span data-ttu-id="0db25-108">说明</span><span class="sxs-lookup"><span data-stu-id="0db25-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0db25-109">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0db25-109">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="0db25-110">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0db25-110">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="0db25-111">检索**dataPolicyOperation**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0db25-111">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="0db25-112">导出个人数据</span><span class="sxs-lookup"><span data-stu-id="0db25-112">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="0db25-113">无</span><span class="sxs-lookup"><span data-stu-id="0db25-113">None</span></span> |<span data-ttu-id="0db25-114">提交数据策略操作请求，以便以后可以使用[获取 dataPolicyOperation](../api/datapolicyoperation-get.md)读取的组织用户的数据导出</span><span class="sxs-lookup"><span data-stu-id="0db25-114">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="0db25-115">属性</span><span class="sxs-lookup"><span data-stu-id="0db25-115">Properties</span></span>

> <span data-ttu-id="0db25-116">**注意：** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="0db25-116">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="0db25-117">属性</span><span class="sxs-lookup"><span data-stu-id="0db25-117">Property</span></span>     | <span data-ttu-id="0db25-118">类型</span><span class="sxs-lookup"><span data-stu-id="0db25-118">Type</span></span>   |<span data-ttu-id="0db25-119">说明</span><span class="sxs-lookup"><span data-stu-id="0db25-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0db25-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0db25-120">completedDateTime</span></span>|<span data-ttu-id="0db25-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db25-121">DateTimeOffset</span></span>|<span data-ttu-id="0db25-122">表示此数据策略操作的请求完成时，在 UTC 时间中，使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="0db25-122">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0db25-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0db25-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0db25-124">在操作完成前，则为 null。</span><span class="sxs-lookup"><span data-stu-id="0db25-124">Null until the operation completes.</span></span>|
|<span data-ttu-id="0db25-125">id</span><span class="sxs-lookup"><span data-stu-id="0db25-125">id</span></span>|<span data-ttu-id="0db25-126">String</span><span class="sxs-lookup"><span data-stu-id="0db25-126">String</span></span>| <span data-ttu-id="0db25-127">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="0db25-127">Unique key for this operation.</span></span> |
|<span data-ttu-id="0db25-128">状态</span><span class="sxs-lookup"><span data-stu-id="0db25-128">status</span></span>|<span data-ttu-id="0db25-129">string</span><span class="sxs-lookup"><span data-stu-id="0db25-129">string</span></span>| <span data-ttu-id="0db25-130">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0db25-130">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0db25-131">storageLocation</span><span class="sxs-lookup"><span data-stu-id="0db25-131">storageLocation</span></span>|<span data-ttu-id="0db25-132">String</span><span class="sxs-lookup"><span data-stu-id="0db25-132">String</span></span>|<span data-ttu-id="0db25-133">到要从中导出数据的导出请求的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="0db25-133">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="0db25-134">userId</span><span class="sxs-lookup"><span data-stu-id="0db25-134">userId</span></span>|<span data-ttu-id="0db25-135">String</span><span class="sxs-lookup"><span data-stu-id="0db25-135">String</span></span>|<span data-ttu-id="0db25-136">在其执行操作的用户 id。</span><span class="sxs-lookup"><span data-stu-id="0db25-136">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="0db25-137">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="0db25-137">submittedDateTime</span></span>|<span data-ttu-id="0db25-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db25-138">DateTimeOffset</span></span>|<span data-ttu-id="0db25-139">表示此数据操作的请求已提交时，在 UTC 时间中，使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="0db25-139">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0db25-140">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0db25-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0db25-141">进度</span><span class="sxs-lookup"><span data-stu-id="0db25-141">progress</span></span>|<span data-ttu-id="0db25-142">String</span><span class="sxs-lookup"><span data-stu-id="0db25-142">String</span></span>|<span data-ttu-id="0db25-143">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="0db25-143">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0db25-144">关系</span><span class="sxs-lookup"><span data-stu-id="0db25-144">Relationships</span></span>
<span data-ttu-id="0db25-145">无。</span><span class="sxs-lookup"><span data-stu-id="0db25-145">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0db25-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0db25-146">JSON representation</span></span>

<span data-ttu-id="0db25-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0db25-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
