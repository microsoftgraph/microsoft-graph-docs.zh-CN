---
title: 获得 onenoteOperation
description: '获取长时间运行的 OneNote 操作的状态。这适用于在响应中返回 **Operation-Location** 标头的操作，例如 `CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection`。   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7974d12e0130fb61da6ee20afe35c3d0dd0e6575
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913777"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="c12a6-104">获得 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="c12a6-104">Get onenoteOperation</span></span>

> <span data-ttu-id="c12a6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c12a6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c12a6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c12a6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c12a6-p103">获取长时间运行的 OneNote 操作的状态。这适用于在响应中返回 **Operation-Location** 标头的操作，例如 `CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection`。</span><span class="sxs-lookup"><span data-stu-id="c12a6-p103">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="c12a6-109">可以轮询 Operation-Location 终结点，直到 `status` 属性返回 `completed` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="c12a6-109">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="c12a6-110">如果状态是 `completed`，则此 `resourceLocation` 属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="c12a6-110">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="c12a6-111">如果状态是 `failed`，错误和 `@api.diagnostics` 属性提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="c12a6-111">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="c12a6-112">权限</span><span class="sxs-lookup"><span data-stu-id="c12a6-112">Permissions</span></span>
<span data-ttu-id="c12a6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c12a6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c12a6-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="c12a6-115">Permission type</span></span>      | <span data-ttu-id="c12a6-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c12a6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c12a6-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c12a6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c12a6-118">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c12a6-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c12a6-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c12a6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c12a6-120">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c12a6-120">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c12a6-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="c12a6-121">Application</span></span> | <span data-ttu-id="c12a6-122">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c12a6-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c12a6-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c12a6-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c12a6-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c12a6-124">Optional query parameters</span></span>
<span data-ttu-id="c12a6-125">无。</span><span class="sxs-lookup"><span data-stu-id="c12a6-125">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c12a6-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c12a6-126">Request headers</span></span>
| <span data-ttu-id="c12a6-127">名称</span><span class="sxs-lookup"><span data-stu-id="c12a6-127">Name</span></span>       | <span data-ttu-id="c12a6-128">类型</span><span class="sxs-lookup"><span data-stu-id="c12a6-128">Type</span></span> | <span data-ttu-id="c12a6-129">说明</span><span class="sxs-lookup"><span data-stu-id="c12a6-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c12a6-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c12a6-130">Authorization</span></span>  | <span data-ttu-id="c12a6-131">string</span><span class="sxs-lookup"><span data-stu-id="c12a6-131">string</span></span>  | <span data-ttu-id="c12a6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c12a6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c12a6-134">Accept</span><span class="sxs-lookup"><span data-stu-id="c12a6-134">Accept</span></span> | <span data-ttu-id="c12a6-135">string</span><span class="sxs-lookup"><span data-stu-id="c12a6-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c12a6-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="c12a6-136">Request body</span></span>
<span data-ttu-id="c12a6-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c12a6-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c12a6-138">响应</span><span class="sxs-lookup"><span data-stu-id="c12a6-138">Response</span></span>

<span data-ttu-id="c12a6-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [onenoteOperation](../resources/onenoteoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c12a6-139">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c12a6-140">示例</span><span class="sxs-lookup"><span data-stu-id="c12a6-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c12a6-141">请求</span><span class="sxs-lookup"><span data-stu-id="c12a6-141">Request</span></span>
<span data-ttu-id="c12a6-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c12a6-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="c12a6-143">响应</span><span class="sxs-lookup"><span data-stu-id="c12a6-143">Response</span></span>
<span data-ttu-id="c12a6-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c12a6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
