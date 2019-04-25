---
title: 进程资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563276"
---
# <a name="process-resource-type"></a><span data-ttu-id="514f7-104">进程资源类型</span><span class="sxs-lookup"><span data-stu-id="514f7-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="514f7-105">包含有关与警报相关的进程的状态信息。</span><span class="sxs-lookup"><span data-stu-id="514f7-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="514f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="514f7-106">Properties</span></span>

| <span data-ttu-id="514f7-107">属性</span><span class="sxs-lookup"><span data-stu-id="514f7-107">Property</span></span>   | <span data-ttu-id="514f7-108">类型</span><span class="sxs-lookup"><span data-stu-id="514f7-108">Type</span></span>|<span data-ttu-id="514f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="514f7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="514f7-110">帐户</span><span class="sxs-lookup"><span data-stu-id="514f7-110">accountName</span></span>|<span data-ttu-id="514f7-111">String</span><span class="sxs-lookup"><span data-stu-id="514f7-111">String</span></span>|<span data-ttu-id="514f7-112">用户帐户标识符 (进程在其下运行的用户帐户上下文) 例如, AccountName、SID 等。</span><span class="sxs-lookup"><span data-stu-id="514f7-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="514f7-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="514f7-113">commandLine</span></span>|<span data-ttu-id="514f7-114">String</span><span class="sxs-lookup"><span data-stu-id="514f7-114">String</span></span>|<span data-ttu-id="514f7-115">完整的过程调用命令行, 包括所有参数。</span><span class="sxs-lookup"><span data-stu-id="514f7-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="514f7-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="514f7-116">createdDateTime</span></span>|<span data-ttu-id="514f7-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="514f7-117">DateTimeOffset</span></span>|<span data-ttu-id="514f7-118">启动进程的时间。</span><span class="sxs-lookup"><span data-stu-id="514f7-118">Time at which the process was started.</span></span> <span data-ttu-id="514f7-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="514f7-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="514f7-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="514f7-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="514f7-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="514f7-121">fileHash</span></span>|[<span data-ttu-id="514f7-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="514f7-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="514f7-123">包含文件哈希 (加密和位置敏感) 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="514f7-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="514f7-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="514f7-124">integrityLevel</span></span>|<span data-ttu-id="514f7-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="514f7-125">processIntegrityLevel</span></span>|<span data-ttu-id="514f7-126">进程的完整性级别。</span><span class="sxs-lookup"><span data-stu-id="514f7-126">The integrity level of the process.</span></span> <span data-ttu-id="514f7-127">可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="514f7-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="514f7-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="514f7-128">isElevated</span></span>|<span data-ttu-id="514f7-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="514f7-129">Boolean</span></span>|<span data-ttu-id="514f7-130">如果进程已提升, 则为 True。</span><span class="sxs-lookup"><span data-stu-id="514f7-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="514f7-131">name</span><span class="sxs-lookup"><span data-stu-id="514f7-131">name</span></span>|<span data-ttu-id="514f7-132">String</span><span class="sxs-lookup"><span data-stu-id="514f7-132">String</span></span>|<span data-ttu-id="514f7-133">进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="514f7-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="514f7-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="514f7-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="514f7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="514f7-135">DateTimeOffset</span></span>|<span data-ttu-id="514f7-136">父进程已启动的日期时间。</span><span class="sxs-lookup"><span data-stu-id="514f7-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="514f7-137">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="514f7-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="514f7-138">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="514f7-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="514f7-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="514f7-139">parentProcessId</span></span>|<span data-ttu-id="514f7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="514f7-140">Int32</span></span>|<span data-ttu-id="514f7-141">父进程的进程 ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="514f7-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="514f7-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="514f7-142">parentProcessName</span></span>|<span data-ttu-id="514f7-143">String</span><span class="sxs-lookup"><span data-stu-id="514f7-143">String</span></span>|<span data-ttu-id="514f7-144">父进程的图像文件的名称。</span><span class="sxs-lookup"><span data-stu-id="514f7-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="514f7-145">路径</span><span class="sxs-lookup"><span data-stu-id="514f7-145">path</span></span>|<span data-ttu-id="514f7-146">字符串</span><span class="sxs-lookup"><span data-stu-id="514f7-146">String</span></span>|<span data-ttu-id="514f7-147">完整路径, 包括文件名。</span><span class="sxs-lookup"><span data-stu-id="514f7-147">Full path, including filename.</span></span>|
|<span data-ttu-id="514f7-148">processId</span><span class="sxs-lookup"><span data-stu-id="514f7-148">processId</span></span>|<span data-ttu-id="514f7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="514f7-149">Int32</span></span>|<span data-ttu-id="514f7-150">进程的进程 ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="514f7-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="514f7-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="514f7-151">JSON representation</span></span>

<span data-ttu-id="514f7-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="514f7-152">The following is a JSON representation of the resource.</span></span>

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
