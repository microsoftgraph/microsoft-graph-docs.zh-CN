---
title: 过程资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 36acd6ed0f6e2cee5095d445de3ba4ff024a024a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869466"
---
# <a name="process-resource-type"></a><span data-ttu-id="05634-104">过程资源类型</span><span class="sxs-lookup"><span data-stu-id="05634-104">process resource type</span></span>

 > <span data-ttu-id="05634-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="05634-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05634-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="05634-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05634-107">包含有关与通知相关的过程的状态信息。</span><span class="sxs-lookup"><span data-stu-id="05634-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="05634-108">属性</span><span class="sxs-lookup"><span data-stu-id="05634-108">Properties</span></span>

| <span data-ttu-id="05634-109">属性</span><span class="sxs-lookup"><span data-stu-id="05634-109">Property</span></span>   | <span data-ttu-id="05634-110">类型</span><span class="sxs-lookup"><span data-stu-id="05634-110">Type</span></span>|<span data-ttu-id="05634-111">Description</span><span class="sxs-lookup"><span data-stu-id="05634-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05634-112">accountName</span><span class="sxs-lookup"><span data-stu-id="05634-112">accountName</span></span>|<span data-ttu-id="05634-113">字符串</span><span class="sxs-lookup"><span data-stu-id="05634-113">String</span></span>|<span data-ttu-id="05634-114">用户帐户标识符 （下运行过程的用户帐户上下文） 的示例、 AccountName、 SID，等等。</span><span class="sxs-lookup"><span data-stu-id="05634-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="05634-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="05634-115">commandLine</span></span>|<span data-ttu-id="05634-116">String</span><span class="sxs-lookup"><span data-stu-id="05634-116">String</span></span>|<span data-ttu-id="05634-117">包括所有参数中的完整过程调用 commandline。</span><span class="sxs-lookup"><span data-stu-id="05634-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="05634-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05634-118">createdDateTime</span></span>|<span data-ttu-id="05634-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05634-119">DateTimeOffset</span></span>|<span data-ttu-id="05634-120">过程开始时间。</span><span class="sxs-lookup"><span data-stu-id="05634-120">Time at which the process was started.</span></span> <span data-ttu-id="05634-121">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="05634-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="05634-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="05634-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="05634-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="05634-123">fileHash</span></span>|[<span data-ttu-id="05634-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="05634-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="05634-125">包含文件哈希 （加密和位置） 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="05634-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="05634-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="05634-126">integrityLevel</span></span>|<span data-ttu-id="05634-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="05634-127">processIntegrityLevel</span></span>|<span data-ttu-id="05634-128">过程的完整性级别。</span><span class="sxs-lookup"><span data-stu-id="05634-128">The integrity level of the process.</span></span> <span data-ttu-id="05634-129">可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="05634-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="05634-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="05634-130">isElevated</span></span>|<span data-ttu-id="05634-131">布尔</span><span class="sxs-lookup"><span data-stu-id="05634-131">Boolean</span></span>|<span data-ttu-id="05634-132">如果提升进程，则为 true。</span><span class="sxs-lookup"><span data-stu-id="05634-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="05634-133">name</span><span class="sxs-lookup"><span data-stu-id="05634-133">name</span></span>|<span data-ttu-id="05634-134">字符串</span><span class="sxs-lookup"><span data-stu-id="05634-134">String</span></span>|<span data-ttu-id="05634-135">进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="05634-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="05634-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="05634-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="05634-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05634-137">DateTimeOffset</span></span>|<span data-ttu-id="05634-138">父进程已开始的日期时间。</span><span class="sxs-lookup"><span data-stu-id="05634-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="05634-139">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="05634-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="05634-140">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="05634-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="05634-141">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="05634-141">parentProcessId</span></span>|<span data-ttu-id="05634-142">Int32</span><span class="sxs-lookup"><span data-stu-id="05634-142">Int32</span></span>|<span data-ttu-id="05634-143">进程 ID (PID) 的父进程。</span><span class="sxs-lookup"><span data-stu-id="05634-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="05634-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="05634-144">parentProcessName</span></span>|<span data-ttu-id="05634-145">字符串</span><span class="sxs-lookup"><span data-stu-id="05634-145">String</span></span>|<span data-ttu-id="05634-146">父流程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="05634-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="05634-147">路径</span><span class="sxs-lookup"><span data-stu-id="05634-147">path</span></span>|<span data-ttu-id="05634-148">字符串</span><span class="sxs-lookup"><span data-stu-id="05634-148">String</span></span>|<span data-ttu-id="05634-149">完整路径，包括文件名。</span><span class="sxs-lookup"><span data-stu-id="05634-149">Full path, including filename.</span></span>|
|<span data-ttu-id="05634-150">processId</span><span class="sxs-lookup"><span data-stu-id="05634-150">processId</span></span>|<span data-ttu-id="05634-151">Int32</span><span class="sxs-lookup"><span data-stu-id="05634-151">Int32</span></span>|<span data-ttu-id="05634-152">进程 ID (PID) 的过程。</span><span class="sxs-lookup"><span data-stu-id="05634-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05634-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05634-153">JSON representation</span></span>

<span data-ttu-id="05634-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05634-154">The following is a JSON representation of the resource.</span></span>

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
