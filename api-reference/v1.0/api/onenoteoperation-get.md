---
title: 获得 onenoteOperation
description: '获取长时间运行的 OneNote 操作的状态。这适用于在响应中返回 **Operation-Location** 标头的操作，例如 `CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection`。   '
localization_priority: Normal
ms.openlocfilehash: c402c5d334ab3b1fb34b2991ffcdb94c89bd5da3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894325"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="4f383-104">获得 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="4f383-104">Get onenoteOperation</span></span>

<span data-ttu-id="4f383-p102">获取长时间运行的 OneNote 操作的状态。这适用于在响应中返回 **Operation-Location** 标头的操作，例如 `CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection`。</span><span class="sxs-lookup"><span data-stu-id="4f383-p102">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="4f383-107">可以轮询 Operation-Location 终结点，直到 `status` 属性返回 `completed` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="4f383-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="4f383-108">如果状态是 `completed`，则此 `resourceLocation` 属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="4f383-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="4f383-109">如果状态是 `failed`，错误和 `@api.diagnostics` 属性提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="4f383-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f383-110">权限</span><span class="sxs-lookup"><span data-stu-id="4f383-110">Permissions</span></span>
<span data-ttu-id="4f383-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f383-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f383-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f383-113">Permission type</span></span>      | <span data-ttu-id="4f383-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f383-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f383-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f383-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4f383-116">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f383-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f383-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f383-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f383-118">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f383-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4f383-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f383-119">Application</span></span> | <span data-ttu-id="4f383-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f383-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f383-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f383-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4f383-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4f383-122">Optional query parameters</span></span>
<span data-ttu-id="4f383-123">无。</span><span class="sxs-lookup"><span data-stu-id="4f383-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f383-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f383-124">Request headers</span></span>
| <span data-ttu-id="4f383-125">名称</span><span class="sxs-lookup"><span data-stu-id="4f383-125">Name</span></span>       | <span data-ttu-id="4f383-126">类型</span><span class="sxs-lookup"><span data-stu-id="4f383-126">Type</span></span> | <span data-ttu-id="4f383-127">说明</span><span class="sxs-lookup"><span data-stu-id="4f383-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f383-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f383-128">Authorization</span></span>  | <span data-ttu-id="4f383-129">string</span><span class="sxs-lookup"><span data-stu-id="4f383-129">string</span></span>  | <span data-ttu-id="4f383-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f383-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f383-132">Accept</span><span class="sxs-lookup"><span data-stu-id="4f383-132">Accept</span></span> | <span data-ttu-id="4f383-133">string</span><span class="sxs-lookup"><span data-stu-id="4f383-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4f383-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f383-134">Request body</span></span>
<span data-ttu-id="4f383-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f383-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f383-136">响应</span><span class="sxs-lookup"><span data-stu-id="4f383-136">Response</span></span>

<span data-ttu-id="4f383-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [onenoteOperation](../resources/onenoteoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f383-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f383-138">示例</span><span class="sxs-lookup"><span data-stu-id="4f383-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f383-139">请求</span><span class="sxs-lookup"><span data-stu-id="4f383-139">Request</span></span>
<span data-ttu-id="4f383-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f383-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="4f383-141">响应</span><span class="sxs-lookup"><span data-stu-id="4f383-141">Response</span></span>
<span data-ttu-id="4f383-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f383-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
