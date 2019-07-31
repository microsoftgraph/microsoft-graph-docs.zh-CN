---
title: 创建 synchronizationJob
description: 使用默认同步架构创建新的同步作业。 作业将在禁用状态中创建。 启动同步的呼叫启动作业。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7a766012070d0dae3851a4822408393aea16b694
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977829"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="65576-105">创建 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="65576-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65576-106">使用默认同步架构创建新的同步作业。</span><span class="sxs-lookup"><span data-stu-id="65576-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="65576-107">作业将在禁用状态中创建。</span><span class="sxs-lookup"><span data-stu-id="65576-107">The job is created in a disabled state.</span></span> <span data-ttu-id="65576-108">启动同步的呼叫[启动作业](synchronization-synchronizationjob-start.md)。</span><span class="sxs-lookup"><span data-stu-id="65576-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="65576-109">权限</span><span class="sxs-lookup"><span data-stu-id="65576-109">Permissions</span></span>
<span data-ttu-id="65576-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65576-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65576-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="65576-112">Permission type</span></span>                        | <span data-ttu-id="65576-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65576-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="65576-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65576-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="65576-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65576-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="65576-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65576-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="65576-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="65576-117">Not supported.</span></span>|
|<span data-ttu-id="65576-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="65576-118">Application</span></span>                            |<span data-ttu-id="65576-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="65576-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="65576-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65576-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="65576-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="65576-121">Request headers</span></span>

| <span data-ttu-id="65576-122">名称</span><span class="sxs-lookup"><span data-stu-id="65576-122">Name</span></span>           | <span data-ttu-id="65576-123">类型</span><span class="sxs-lookup"><span data-stu-id="65576-123">Type</span></span>    | <span data-ttu-id="65576-124">说明</span><span class="sxs-lookup"><span data-stu-id="65576-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="65576-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="65576-125">Authorization</span></span>  | <span data-ttu-id="65576-126">string</span><span class="sxs-lookup"><span data-stu-id="65576-126">string</span></span>  | <span data-ttu-id="65576-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65576-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65576-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="65576-129">Request body</span></span>

<span data-ttu-id="65576-130">在请求正文中, 提供要创建的[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65576-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="65576-131">唯一的必需属性是`templateId`。</span><span class="sxs-lookup"><span data-stu-id="65576-131">The only required property is `templateId`.</span></span> <span data-ttu-id="65576-132">`templateId`属性必须与为此应用程序/服务主体创建的一个模板相匹配。</span><span class="sxs-lookup"><span data-stu-id="65576-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="65576-133">若要查找可用模板, 请使用[列表模板](synchronization-synchronizationtemplate-list.md)。</span><span class="sxs-lookup"><span data-stu-id="65576-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="65576-134">响应</span><span class="sxs-lookup"><span data-stu-id="65576-134">Response</span></span>

<span data-ttu-id="65576-135">如果成功, 则在`201 Created`响应正文中返回响应代码和[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="65576-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65576-136">示例</span><span class="sxs-lookup"><span data-stu-id="65576-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="65576-137">请求</span><span class="sxs-lookup"><span data-stu-id="65576-137">Request</span></span>
<span data-ttu-id="65576-138">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="65576-138">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="65576-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="65576-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65576-140">C#</span><span class="sxs-lookup"><span data-stu-id="65576-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65576-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="65576-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65576-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="65576-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65576-143">Java</span><span class="sxs-lookup"><span data-stu-id="65576-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationjob-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65576-144">响应</span><span class="sxs-lookup"><span data-stu-id="65576-144">Response</span></span>
<span data-ttu-id="65576-145">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="65576-145">The following is an example of a response.</span></span> 

><span data-ttu-id="65576-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="65576-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
