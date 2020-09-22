---
title: 进程资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: a024cfbabcff4357427ae6a814da00af83eae304
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070490"
---
# <a name="process-resource-type"></a><span data-ttu-id="7a054-104">进程资源类型</span><span class="sxs-lookup"><span data-stu-id="7a054-104">process resource type</span></span>

<span data-ttu-id="7a054-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a054-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a054-106">包含有关与警报相关的进程的状态信息。</span><span class="sxs-lookup"><span data-stu-id="7a054-106">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="7a054-107">属性</span><span class="sxs-lookup"><span data-stu-id="7a054-107">Properties</span></span>

| <span data-ttu-id="7a054-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a054-108">Property</span></span>   | <span data-ttu-id="7a054-109">类型</span><span class="sxs-lookup"><span data-stu-id="7a054-109">Type</span></span>|<span data-ttu-id="7a054-110">说明</span><span class="sxs-lookup"><span data-stu-id="7a054-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a054-111">帐户</span><span class="sxs-lookup"><span data-stu-id="7a054-111">accountName</span></span>|<span data-ttu-id="7a054-112">String</span><span class="sxs-lookup"><span data-stu-id="7a054-112">String</span></span>|<span data-ttu-id="7a054-113">用户帐户标识符 (的用户帐户上下文。该进程在) 下运行，例如，AccountName、SID 等。</span><span class="sxs-lookup"><span data-stu-id="7a054-113">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="7a054-114">commandLine</span><span class="sxs-lookup"><span data-stu-id="7a054-114">commandLine</span></span>|<span data-ttu-id="7a054-115">String</span><span class="sxs-lookup"><span data-stu-id="7a054-115">String</span></span>|<span data-ttu-id="7a054-116">完整的过程调用命令行，包括所有参数。</span><span class="sxs-lookup"><span data-stu-id="7a054-116">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="7a054-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a054-117">createdDateTime</span></span>|<span data-ttu-id="7a054-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a054-118">DateTimeOffset</span></span>|<span data-ttu-id="7a054-119">启动进程的时间。</span><span class="sxs-lookup"><span data-stu-id="7a054-119">Time at which the process was started.</span></span> <span data-ttu-id="7a054-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7a054-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7a054-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7a054-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7a054-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="7a054-122">fileHash</span></span>|[<span data-ttu-id="7a054-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="7a054-123">fileHash</span></span>](filehash.md)|<span data-ttu-id="7a054-124">包含 (加密和位置敏感) 的文件哈希的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="7a054-124">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="7a054-125">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="7a054-125">integrityLevel</span></span>|<span data-ttu-id="7a054-126">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="7a054-126">processIntegrityLevel</span></span>|<span data-ttu-id="7a054-127">进程的完整性级别。</span><span class="sxs-lookup"><span data-stu-id="7a054-127">The integrity level of the process.</span></span> <span data-ttu-id="7a054-128">可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="7a054-128">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="7a054-129">isElevated</span><span class="sxs-lookup"><span data-stu-id="7a054-129">isElevated</span></span>|<span data-ttu-id="7a054-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a054-130">Boolean</span></span>|<span data-ttu-id="7a054-131">如果进程已提升，则为 True。</span><span class="sxs-lookup"><span data-stu-id="7a054-131">True if the process is elevated.</span></span>|
|<span data-ttu-id="7a054-132">名称</span><span class="sxs-lookup"><span data-stu-id="7a054-132">name</span></span>|<span data-ttu-id="7a054-133">String</span><span class="sxs-lookup"><span data-stu-id="7a054-133">String</span></span>|<span data-ttu-id="7a054-134">进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="7a054-134">The name of the process' Image file.</span></span>|
|<span data-ttu-id="7a054-135">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a054-135">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="7a054-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a054-136">DateTimeOffset</span></span>|<span data-ttu-id="7a054-137">父进程已启动的日期时间。</span><span class="sxs-lookup"><span data-stu-id="7a054-137">DateTime at which the parent process was started.</span></span> <span data-ttu-id="7a054-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7a054-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7a054-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7a054-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7a054-140">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="7a054-140">parentProcessId</span></span>|<span data-ttu-id="7a054-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7a054-141">Int32</span></span>|<span data-ttu-id="7a054-142">父进程 (PID) 的进程 ID。</span><span class="sxs-lookup"><span data-stu-id="7a054-142">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="7a054-143">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="7a054-143">parentProcessName</span></span>|<span data-ttu-id="7a054-144">String</span><span class="sxs-lookup"><span data-stu-id="7a054-144">String</span></span>|<span data-ttu-id="7a054-145">父进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="7a054-145">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="7a054-146">路径</span><span class="sxs-lookup"><span data-stu-id="7a054-146">path</span></span>|<span data-ttu-id="7a054-147">String</span><span class="sxs-lookup"><span data-stu-id="7a054-147">String</span></span>|<span data-ttu-id="7a054-148">完整路径，包括文件名。</span><span class="sxs-lookup"><span data-stu-id="7a054-148">Full path, including filename.</span></span>|
|<span data-ttu-id="7a054-149">processId</span><span class="sxs-lookup"><span data-stu-id="7a054-149">processId</span></span>|<span data-ttu-id="7a054-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7a054-150">Int32</span></span>|<span data-ttu-id="7a054-151">进程的进程 ID (PID) 。</span><span class="sxs-lookup"><span data-stu-id="7a054-151">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a054-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a054-152">JSON representation</span></span>

<span data-ttu-id="7a054-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a054-153">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


