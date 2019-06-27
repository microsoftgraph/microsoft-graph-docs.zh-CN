---
title: 处理长时间运行的操作（测试）
description: 本文会介绍处理长时间运行的操作。
localization_priority: Normal
author: daspek
ms.openlocfilehash: 0403dd8e099a5f21f3b1da7cf74859b664eefa43
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277768"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="f1b43-103">处理长时间运行的操作 (beta)</span><span class="sxs-lookup"><span data-stu-id="f1b43-103">Working with long running actions (beta)</span></span>


<span data-ttu-id="f1b43-104">某些 API 响应完成所需的时间不确定。</span><span class="sxs-lookup"><span data-stu-id="f1b43-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="f1b43-105">Microsoft Graph 可能会使用长时间运行操作模式，而不是等待操作完成之后再返回响应。</span><span class="sxs-lookup"><span data-stu-id="f1b43-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="f1b43-106">此模式可让应用等待轮询长时间运行操作的状态更新，而无需任何等待操作完成的请求。</span><span class="sxs-lookup"><span data-stu-id="f1b43-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="f1b43-107">常规模式包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="f1b43-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="f1b43-108">应用请求通过 API 执行长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="f1b43-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="f1b43-109">API 接受操作，并返回 `202 Accepted` 响应以及 API URL 的 Location 头，以便检索操作状态报告。</span><span class="sxs-lookup"><span data-stu-id="f1b43-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="f1b43-110">应用请求获取操作状态报告 URL，然后收到包含长时间运行的操作进度的 [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 响应。</span><span class="sxs-lookup"><span data-stu-id="f1b43-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="f1b43-111">长时间运行的操作完成。</span><span class="sxs-lookup"><span data-stu-id="f1b43-111">The long running action completes.</span></span> 
4. <span data-ttu-id="f1b43-112">应用再次请求获取操作状态报告 URL ，然后收到显示操作已完成状态的 [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 响应。</span><span class="sxs-lookup"><span data-stu-id="f1b43-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="f1b43-113">初始操作请求</span><span class="sxs-lookup"><span data-stu-id="f1b43-113">Initial action request</span></span>

<span data-ttu-id="f1b43-114">让我们来逐步完成 [DriveItem 复制](/graph/api/driveitem-copy?view=graph-rest-beta)示例方案。</span><span class="sxs-lookup"><span data-stu-id="f1b43-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="f1b43-115">在此方案中，应用请求复制包含大量数据的文件夹。</span><span class="sxs-lookup"><span data-stu-id="f1b43-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="f1b43-116">因为数据量较大，所以此请求可能需要几秒钟才能完成。</span><span class="sxs-lookup"><span data-stu-id="f1b43-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>

<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```

<span data-ttu-id="f1b43-117">API 予以响应，指明已接受此操作，并返回用于检索长时间运行的操作的状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="f1b43-117">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1b43-118">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f1b43-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1b43-119">C#</span><span class="sxs-lookup"><span data-stu-id="f1b43-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1b43-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1b43-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1b43-121">目标-C</span><span class="sxs-lookup"><span data-stu-id="f1b43-121">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="f1b43-122">**注意：** 返回的位置 URL 可能不在 Microsoft Graph API 终结点上。</span><span class="sxs-lookup"><span data-stu-id="f1b43-122">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="f1b43-123">在很多情况下，请求到此结束，因为复制操作的完成无需应用执行其他任何工作。</span><span class="sxs-lookup"><span data-stu-id="f1b43-123">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="f1b43-124">不过，如果应用需要显示复制操作的状态，或确保其正确完成，可以使用监视器 URL。</span><span class="sxs-lookup"><span data-stu-id="f1b43-124">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="f1b43-125">通过监视器 URL 检索状态报告</span><span class="sxs-lookup"><span data-stu-id="f1b43-125">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="f1b43-p105">为了检查复制操作的状态，应用会请求获取上一响应中返回的 URL。 *注意：* 此请求无需验证，因为这是原始调用方专属的短期 URL。</span><span class="sxs-lookup"><span data-stu-id="f1b43-p105">To check on the status of the copy action, the app makes a request to the URL provided in the previous response. *Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="f1b43-128">服务响应返回的信息指明长时间运行的操作仍在进行中：</span><span class="sxs-lookup"><span data-stu-id="f1b43-128">The service responses with information that the long running action is still in progress:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

<span data-ttu-id="f1b43-p106">此信息可用于向用户提供复制操作的最新进度。 应用可以继续轮询监视器 URL，以请求获取状态更新并跟踪操作进度。</span><span class="sxs-lookup"><span data-stu-id="f1b43-p106">This information can be used to provide an update to the user about the progress of the copy action. The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="f1b43-131">通过监视器 URL 检索已完成状态报告</span><span class="sxs-lookup"><span data-stu-id="f1b43-131">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="f1b43-p107">几秒钟后，复制操作完成。 当应用向监视器 URL 发出请求时，响应返回的是重定向到操作的最终结果。</span><span class="sxs-lookup"><span data-stu-id="f1b43-p107">After a few seconds the copy operation has completed. This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="f1b43-134">完成操作后，监视器服务的响应将返回结果的 resourceId。</span><span class="sxs-lookup"><span data-stu-id="f1b43-134">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="f1b43-135">检索已完成的操作的结果</span><span class="sxs-lookup"><span data-stu-id="f1b43-135">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="f1b43-136">完成作业后，监视器 URL 返回结果的 resourceId，在此例中为原始项的新副本。</span><span class="sxs-lookup"><span data-stu-id="f1b43-136">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="f1b43-137">可以使用 resourceId 处理此新项，例如：</span><span class="sxs-lookup"><span data-stu-id="f1b43-137">You can address this new item using the resourceId, for example:</span></span>

<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1b43-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f1b43-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1b43-139">C#</span><span class="sxs-lookup"><span data-stu-id="f1b43-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1b43-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1b43-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1b43-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="f1b43-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="supported-resources"></a><span data-ttu-id="f1b43-142">支持的资源</span><span class="sxs-lookup"><span data-stu-id="f1b43-142">Supported resources</span></span>

<span data-ttu-id="f1b43-143">以下 API 方法支持长时间运行的操作</span><span class="sxs-lookup"><span data-stu-id="f1b43-143">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="f1b43-144">**资源**</span><span class="sxs-lookup"><span data-stu-id="f1b43-144">**Resource**</span></span> | <span data-ttu-id="f1b43-145">**API**</span><span class="sxs-lookup"><span data-stu-id="f1b43-145">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="f1b43-146">DriveItem</span><span class="sxs-lookup"><span data-stu-id="f1b43-146">DriveItem</span></span> | [<span data-ttu-id="f1b43-147">Copy</span><span class="sxs-lookup"><span data-stu-id="f1b43-147">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="f1b43-148">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1b43-148">Prerequisites</span></span>

<span data-ttu-id="f1b43-149">查询长时间运行的操作的状态也需要执行长时间运行的操作所需的相同[权限](./permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f1b43-149">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
