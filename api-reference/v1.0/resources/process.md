---
title: 过程资源类型
description: 包含有关与通知相关的过程的状态信息。
localization_priority: Normal
ms.openlocfilehash: 0b4207c1780dfd6327ceb67e837f793341e609ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864419"
---
# <a name="process-resource-type"></a><span data-ttu-id="215fc-103">过程资源类型</span><span class="sxs-lookup"><span data-stu-id="215fc-103">process resource type</span></span>

<span data-ttu-id="215fc-104">包含有关与通知相关的过程的状态信息。</span><span class="sxs-lookup"><span data-stu-id="215fc-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="215fc-105">属性</span><span class="sxs-lookup"><span data-stu-id="215fc-105">Properties</span></span>

| <span data-ttu-id="215fc-106">属性</span><span class="sxs-lookup"><span data-stu-id="215fc-106">Property</span></span>   | <span data-ttu-id="215fc-107">类型</span><span class="sxs-lookup"><span data-stu-id="215fc-107">Type</span></span>|<span data-ttu-id="215fc-108">Description</span><span class="sxs-lookup"><span data-stu-id="215fc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="215fc-109">accountName</span><span class="sxs-lookup"><span data-stu-id="215fc-109">accountName</span></span>|<span data-ttu-id="215fc-110">字符串</span><span class="sxs-lookup"><span data-stu-id="215fc-110">String</span></span>|<span data-ttu-id="215fc-111">用户帐户标识符 （下运行过程的用户帐户上下文） 的示例、 AccountName、 SID，等等。</span><span class="sxs-lookup"><span data-stu-id="215fc-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="215fc-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="215fc-112">commandLine</span></span>|<span data-ttu-id="215fc-113">String</span><span class="sxs-lookup"><span data-stu-id="215fc-113">String</span></span>|<span data-ttu-id="215fc-114">包括所有参数中的完整过程调用 commandline。</span><span class="sxs-lookup"><span data-stu-id="215fc-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="215fc-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="215fc-115">createdDateTime</span></span>|<span data-ttu-id="215fc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="215fc-116">DateTimeOffset</span></span>|<span data-ttu-id="215fc-117">过程开始时间。</span><span class="sxs-lookup"><span data-stu-id="215fc-117">Time at which the process was started.</span></span> <span data-ttu-id="215fc-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="215fc-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="215fc-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="215fc-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="215fc-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="215fc-120">fileHash</span></span>|[<span data-ttu-id="215fc-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="215fc-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="215fc-122">包含文件哈希 （加密和位置） 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="215fc-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="215fc-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="215fc-123">integrityLevel</span></span>|<span data-ttu-id="215fc-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="215fc-124">processIntegrityLevel</span></span>|<span data-ttu-id="215fc-125">过程的完整性级别。</span><span class="sxs-lookup"><span data-stu-id="215fc-125">The integrity level of the process.</span></span> <span data-ttu-id="215fc-126">可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="215fc-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="215fc-127">isElevated</span><span class="sxs-lookup"><span data-stu-id="215fc-127">isElevated</span></span>|<span data-ttu-id="215fc-128">布尔</span><span class="sxs-lookup"><span data-stu-id="215fc-128">Boolean</span></span>|<span data-ttu-id="215fc-129">如果提升进程，则为 true。</span><span class="sxs-lookup"><span data-stu-id="215fc-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="215fc-130">name</span><span class="sxs-lookup"><span data-stu-id="215fc-130">name</span></span>|<span data-ttu-id="215fc-131">字符串</span><span class="sxs-lookup"><span data-stu-id="215fc-131">String</span></span>|<span data-ttu-id="215fc-132">进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="215fc-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="215fc-133">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="215fc-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="215fc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="215fc-134">DateTimeOffset</span></span>|<span data-ttu-id="215fc-135">父进程已开始的日期时间。</span><span class="sxs-lookup"><span data-stu-id="215fc-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="215fc-136">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="215fc-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="215fc-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="215fc-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="215fc-138">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="215fc-138">parentProcessId</span></span>|<span data-ttu-id="215fc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="215fc-139">Int32</span></span>|<span data-ttu-id="215fc-140">进程 ID (PID) 的父进程。</span><span class="sxs-lookup"><span data-stu-id="215fc-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="215fc-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="215fc-141">parentProcessName</span></span>|<span data-ttu-id="215fc-142">字符串</span><span class="sxs-lookup"><span data-stu-id="215fc-142">String</span></span>|<span data-ttu-id="215fc-143">父流程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="215fc-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="215fc-144">路径</span><span class="sxs-lookup"><span data-stu-id="215fc-144">path</span></span>|<span data-ttu-id="215fc-145">字符串</span><span class="sxs-lookup"><span data-stu-id="215fc-145">String</span></span>|<span data-ttu-id="215fc-146">完整路径，包括文件名。</span><span class="sxs-lookup"><span data-stu-id="215fc-146">Full path, including filename.</span></span>|
|<span data-ttu-id="215fc-147">processId</span><span class="sxs-lookup"><span data-stu-id="215fc-147">processId</span></span>|<span data-ttu-id="215fc-148">Int32</span><span class="sxs-lookup"><span data-stu-id="215fc-148">Int32</span></span>|<span data-ttu-id="215fc-149">进程 ID (PID) 的过程。</span><span class="sxs-lookup"><span data-stu-id="215fc-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="215fc-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="215fc-150">JSON representation</span></span>

<span data-ttu-id="215fc-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="215fc-151">The following is a JSON representation of the resource.</span></span>

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
