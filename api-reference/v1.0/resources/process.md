# <a name="process-resource-type"></a><span data-ttu-id="ae688-101">进程资源类型</span><span class="sxs-lookup"><span data-stu-id="ae688-101">process resource type</span></span>

<span data-ttu-id="ae688-102">包含有关与通知相关的进程的有状态信息。</span><span class="sxs-lookup"><span data-stu-id="ae688-102">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="ae688-103">属性</span><span class="sxs-lookup"><span data-stu-id="ae688-103">Properties</span></span>

| <span data-ttu-id="ae688-104">属性</span><span class="sxs-lookup"><span data-stu-id="ae688-104">Property</span></span>   | <span data-ttu-id="ae688-105">类型</span><span class="sxs-lookup"><span data-stu-id="ae688-105">Type</span></span>|<span data-ttu-id="ae688-106">说明</span><span class="sxs-lookup"><span data-stu-id="ae688-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae688-107">accountName</span><span class="sxs-lookup"><span data-stu-id="ae688-107">accountName</span></span>|<span data-ttu-id="ae688-108">字符串</span><span class="sxs-lookup"><span data-stu-id="ae688-108">String</span></span>|<span data-ttu-id="ae688-109">用户帐户标识符 （运行进程的用户帐户上下文），例如 AccountName、SID 等等。</span><span class="sxs-lookup"><span data-stu-id="ae688-109">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="ae688-110">commandLine</span><span class="sxs-lookup"><span data-stu-id="ae688-110">commandLine</span></span>|<span data-ttu-id="ae688-111">字符串</span><span class="sxs-lookup"><span data-stu-id="ae688-111">String</span></span>|<span data-ttu-id="ae688-112">包括所有参数中的完整过程调用命令行。</span><span class="sxs-lookup"><span data-stu-id="ae688-112">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="ae688-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae688-113">createdDateTime</span></span>|<span data-ttu-id="ae688-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae688-114">DateTimeOffset</span></span>|<span data-ttu-id="ae688-115">进程开始的时间。</span><span class="sxs-lookup"><span data-stu-id="ae688-115">Time at which the process was started.</span></span> <span data-ttu-id="ae688-116">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ae688-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae688-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="ae688-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ae688-118">fileHash</span><span class="sxs-lookup"><span data-stu-id="ae688-118">fileHash</span></span>|[<span data-ttu-id="ae688-119">fileHash</span><span class="sxs-lookup"><span data-stu-id="ae688-119">fileHash</span></span>](filehash.md)|<span data-ttu-id="ae688-120">包含文件哈希 （加密和位置敏感）的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="ae688-120">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="ae688-121">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="ae688-121">integrityLevel</span></span>|<span data-ttu-id="ae688-122">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="ae688-122">processIntegrityLevel</span></span>|<span data-ttu-id="ae688-123">过程的完整性级别。</span><span class="sxs-lookup"><span data-stu-id="ae688-123">The integrity level of the process.</span></span> <span data-ttu-id="ae688-124">可能的值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="ae688-124">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="ae688-125">isElevated</span><span class="sxs-lookup"><span data-stu-id="ae688-125">isElevated</span></span>|<span data-ttu-id="ae688-126">布尔</span><span class="sxs-lookup"><span data-stu-id="ae688-126">Boolean</span></span>|<span data-ttu-id="ae688-127">如果提升进程，则为 true。</span><span class="sxs-lookup"><span data-stu-id="ae688-127">True if the process is elevated.</span></span>|
|<span data-ttu-id="ae688-128">name</span><span class="sxs-lookup"><span data-stu-id="ae688-128">name</span></span>|<span data-ttu-id="ae688-129">字符串</span><span class="sxs-lookup"><span data-stu-id="ae688-129">String</span></span>|<span data-ttu-id="ae688-130">进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ae688-130">The name of the process' Image file.</span></span>|
|<span data-ttu-id="ae688-131">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae688-131">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="ae688-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae688-132">DateTimeOffset</span></span>|<span data-ttu-id="ae688-133">父进程开始的日期时间。</span><span class="sxs-lookup"><span data-stu-id="ae688-133">DateTime at which the parent process was started.</span></span> <span data-ttu-id="ae688-134">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ae688-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae688-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="ae688-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ae688-136">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="ae688-136">parentProcessId</span></span>|<span data-ttu-id="ae688-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ae688-137">Int32</span></span>|<span data-ttu-id="ae688-138">父进程的进程 ID (PID) 。</span><span class="sxs-lookup"><span data-stu-id="ae688-138">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="ae688-139">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="ae688-139">parentProcessName</span></span>|<span data-ttu-id="ae688-140">字符串</span><span class="sxs-lookup"><span data-stu-id="ae688-140">String</span></span>|<span data-ttu-id="ae688-141">父进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ae688-141">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="ae688-142">path</span><span class="sxs-lookup"><span data-stu-id="ae688-142">path</span></span>|<span data-ttu-id="ae688-143">字符串</span><span class="sxs-lookup"><span data-stu-id="ae688-143">String</span></span>|<span data-ttu-id="ae688-144">完整路径，包括文件名。</span><span class="sxs-lookup"><span data-stu-id="ae688-144">Full path, including filename.</span></span>|
|<span data-ttu-id="ae688-145">processId</span><span class="sxs-lookup"><span data-stu-id="ae688-145">processId</span></span>|<span data-ttu-id="ae688-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ae688-146">Int32</span></span>|<span data-ttu-id="ae688-147">进程的进程 ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="ae688-147">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae688-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae688-148">JSON representation</span></span>

<span data-ttu-id="ae688-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae688-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->