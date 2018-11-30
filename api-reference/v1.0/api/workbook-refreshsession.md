---
title: 刷新会话
description: '使用此 API 刷新现有的工作簿会话。 '
ms.openlocfilehash: d3504646f4fcacfd71e18c3fc6a83e4835397703
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008257"
---
# <a name="refresh-session"></a><span data-ttu-id="4b92e-103">刷新会话</span><span class="sxs-lookup"><span data-stu-id="4b92e-103">Refresh Session</span></span>

<span data-ttu-id="4b92e-104">使用此 API 刷新现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="4b92e-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4b92e-105">权限</span><span class="sxs-lookup"><span data-stu-id="4b92e-105">Permissions</span></span>
<span data-ttu-id="4b92e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b92e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b92e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b92e-108">Permission type</span></span>      | <span data-ttu-id="4b92e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b92e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b92e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b92e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b92e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b92e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b92e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b92e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b92e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b92e-113">Not supported.</span></span>    |
|<span data-ttu-id="4b92e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b92e-114">Application</span></span> | <span data-ttu-id="4b92e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b92e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b92e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b92e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="4b92e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b92e-117">Request headers</span></span>
| <span data-ttu-id="4b92e-118">名称</span><span class="sxs-lookup"><span data-stu-id="4b92e-118">Name</span></span>       | <span data-ttu-id="4b92e-119">说明</span><span class="sxs-lookup"><span data-stu-id="4b92e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b92e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b92e-120">Authorization</span></span>  | <span data-ttu-id="4b92e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b92e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b92e-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="4b92e-123">workbook-session-id</span></span> | <span data-ttu-id="4b92e-124">要刷新的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="4b92e-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b92e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b92e-125">Request body</span></span>
<span data-ttu-id="4b92e-126">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b92e-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="4b92e-127">响应</span><span class="sxs-lookup"><span data-stu-id="4b92e-127">Response</span></span>

<span data-ttu-id="4b92e-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4b92e-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b92e-129">示例</span><span class="sxs-lookup"><span data-stu-id="4b92e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b92e-130">请求</span><span class="sxs-lookup"><span data-stu-id="4b92e-130">Request</span></span>
<span data-ttu-id="4b92e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b92e-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="4b92e-132">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="4b92e-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="4b92e-133">响应</span><span class="sxs-lookup"><span data-stu-id="4b92e-133">Response</span></span>
<span data-ttu-id="4b92e-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4b92e-134">Here is an example of the response.</span></span> 

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
    "Warning: refresh_excel_session//api-reference/v1.0/api/workbook-refreshsession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
