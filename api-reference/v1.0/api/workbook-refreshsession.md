---
title: 刷新会话
description: '使用此 API 刷新现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5e4aaad295abc4ce83b8669f3d4053edafb1ad5d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575838"
---
# <a name="refresh-session"></a><span data-ttu-id="5ed47-103">刷新会话</span><span class="sxs-lookup"><span data-stu-id="5ed47-103">Refresh Session</span></span>

<span data-ttu-id="5ed47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ed47-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ed47-105">使用此 API 刷新现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="5ed47-105">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5ed47-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ed47-106">Permissions</span></span>
<span data-ttu-id="5ed47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ed47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ed47-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ed47-109">Permission type</span></span>      | <span data-ttu-id="5ed47-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ed47-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ed47-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ed47-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ed47-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ed47-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ed47-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ed47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ed47-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ed47-114">Not supported.</span></span>    |
|<span data-ttu-id="5ed47-115">Application</span><span class="sxs-lookup"><span data-stu-id="5ed47-115">Application</span></span> | <span data-ttu-id="5ed47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ed47-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ed47-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ed47-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/refreshSession
POST /me/drive/root:/{item-path}:/workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="5ed47-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ed47-118">Request headers</span></span>
| <span data-ttu-id="5ed47-119">名称</span><span class="sxs-lookup"><span data-stu-id="5ed47-119">Name</span></span>       | <span data-ttu-id="5ed47-120">说明</span><span class="sxs-lookup"><span data-stu-id="5ed47-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ed47-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ed47-121">Authorization</span></span>  | <span data-ttu-id="5ed47-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ed47-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ed47-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="5ed47-124">workbook-session-id</span></span> | <span data-ttu-id="5ed47-125">要刷新的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="5ed47-125">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ed47-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ed47-126">Request body</span></span>
<span data-ttu-id="5ed47-127">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ed47-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="5ed47-128">响应</span><span class="sxs-lookup"><span data-stu-id="5ed47-128">Response</span></span>

<span data-ttu-id="5ed47-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5ed47-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5ed47-130">示例</span><span class="sxs-lookup"><span data-stu-id="5ed47-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ed47-131">请求</span><span class="sxs-lookup"><span data-stu-id="5ed47-131">Request</span></span>
<span data-ttu-id="5ed47-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ed47-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ed47-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ed47-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="c"></a>[<span data-ttu-id="5ed47-134">C#</span><span class="sxs-lookup"><span data-stu-id="5ed47-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ed47-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ed47-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ed47-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ed47-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ed47-137">Java</span><span class="sxs-lookup"><span data-stu-id="5ed47-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/refresh-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5ed47-138">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="5ed47-138">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="5ed47-139">响应</span><span class="sxs-lookup"><span data-stu-id="5ed47-139">Response</span></span>
<span data-ttu-id="5ed47-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ed47-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
  ]
}-->

