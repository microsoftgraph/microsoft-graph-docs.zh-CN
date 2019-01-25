---
title: 过程资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521206"
---
# <a name="process-resource-type"></a><span data-ttu-id="9208b-104">过程资源类型</span><span class="sxs-lookup"><span data-stu-id="9208b-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9208b-105">包含有关与通知相关的过程的状态信息。</span><span class="sxs-lookup"><span data-stu-id="9208b-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="9208b-106">属性</span><span class="sxs-lookup"><span data-stu-id="9208b-106">Properties</span></span>

| <span data-ttu-id="9208b-107">属性</span><span class="sxs-lookup"><span data-stu-id="9208b-107">Property</span></span>   | <span data-ttu-id="9208b-108">类型</span><span class="sxs-lookup"><span data-stu-id="9208b-108">Type</span></span>|<span data-ttu-id="9208b-109">说明</span><span class="sxs-lookup"><span data-stu-id="9208b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9208b-110">accountName</span><span class="sxs-lookup"><span data-stu-id="9208b-110">accountName</span></span>|<span data-ttu-id="9208b-111">String</span><span class="sxs-lookup"><span data-stu-id="9208b-111">String</span></span>|<span data-ttu-id="9208b-112">用户帐户标识符 （下运行过程的用户帐户上下文） 的示例、 AccountName、 SID，等等。</span><span class="sxs-lookup"><span data-stu-id="9208b-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="9208b-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="9208b-113">commandLine</span></span>|<span data-ttu-id="9208b-114">String</span><span class="sxs-lookup"><span data-stu-id="9208b-114">String</span></span>|<span data-ttu-id="9208b-115">包括所有参数中的完整过程调用 commandline。</span><span class="sxs-lookup"><span data-stu-id="9208b-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="9208b-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9208b-116">createdDateTime</span></span>|<span data-ttu-id="9208b-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9208b-117">DateTimeOffset</span></span>|<span data-ttu-id="9208b-118">过程开始时间。</span><span class="sxs-lookup"><span data-stu-id="9208b-118">Time at which the process was started.</span></span> <span data-ttu-id="9208b-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9208b-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9208b-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="9208b-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9208b-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="9208b-121">fileHash</span></span>|[<span data-ttu-id="9208b-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="9208b-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="9208b-123">包含文件哈希 （加密和位置） 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="9208b-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="9208b-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="9208b-124">integrityLevel</span></span>|<span data-ttu-id="9208b-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="9208b-125">processIntegrityLevel</span></span>|<span data-ttu-id="9208b-126">过程的完整性级别。</span><span class="sxs-lookup"><span data-stu-id="9208b-126">The integrity level of the process.</span></span> <span data-ttu-id="9208b-127">可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="9208b-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="9208b-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="9208b-128">isElevated</span></span>|<span data-ttu-id="9208b-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="9208b-129">Boolean</span></span>|<span data-ttu-id="9208b-130">如果提升进程，则为 true。</span><span class="sxs-lookup"><span data-stu-id="9208b-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="9208b-131">name</span><span class="sxs-lookup"><span data-stu-id="9208b-131">name</span></span>|<span data-ttu-id="9208b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="9208b-132">String</span></span>|<span data-ttu-id="9208b-133">进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="9208b-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="9208b-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9208b-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="9208b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9208b-135">DateTimeOffset</span></span>|<span data-ttu-id="9208b-136">父进程已开始的日期时间。</span><span class="sxs-lookup"><span data-stu-id="9208b-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="9208b-137">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9208b-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9208b-138">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="9208b-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9208b-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="9208b-139">parentProcessId</span></span>|<span data-ttu-id="9208b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9208b-140">Int32</span></span>|<span data-ttu-id="9208b-141">进程 ID (PID) 的父进程。</span><span class="sxs-lookup"><span data-stu-id="9208b-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="9208b-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="9208b-142">parentProcessName</span></span>|<span data-ttu-id="9208b-143">String</span><span class="sxs-lookup"><span data-stu-id="9208b-143">String</span></span>|<span data-ttu-id="9208b-144">父流程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="9208b-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="9208b-145">路径</span><span class="sxs-lookup"><span data-stu-id="9208b-145">path</span></span>|<span data-ttu-id="9208b-146">String</span><span class="sxs-lookup"><span data-stu-id="9208b-146">String</span></span>|<span data-ttu-id="9208b-147">完整路径，包括文件名。</span><span class="sxs-lookup"><span data-stu-id="9208b-147">Full path, including filename.</span></span>|
|<span data-ttu-id="9208b-148">ProcessID</span><span class="sxs-lookup"><span data-stu-id="9208b-148">processId</span></span>|<span data-ttu-id="9208b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9208b-149">Int32</span></span>|<span data-ttu-id="9208b-150">进程 ID (PID) 的过程。</span><span class="sxs-lookup"><span data-stu-id="9208b-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9208b-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9208b-151">JSON representation</span></span>

<span data-ttu-id="9208b-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9208b-152">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/process.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
