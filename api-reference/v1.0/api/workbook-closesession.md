---
title: 关闭会话
description: '使用此 API 关闭现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4c348690e0fbe8942ddea31102adc02c08707036
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600714"
---
# <a name="close-session"></a><span data-ttu-id="88fc2-103">关闭会话</span><span class="sxs-lookup"><span data-stu-id="88fc2-103">Close Session</span></span>

<span data-ttu-id="88fc2-104">使用此 API 关闭现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="88fc2-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="88fc2-105">权限</span><span class="sxs-lookup"><span data-stu-id="88fc2-105">Permissions</span></span>
<span data-ttu-id="88fc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88fc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88fc2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="88fc2-108">Permission type</span></span>      | <span data-ttu-id="88fc2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88fc2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88fc2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88fc2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88fc2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88fc2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="88fc2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88fc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88fc2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="88fc2-113">Not supported.</span></span>    |
|<span data-ttu-id="88fc2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="88fc2-114">Application</span></span> | <span data-ttu-id="88fc2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="88fc2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88fc2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88fc2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="88fc2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="88fc2-117">Request headers</span></span>
| <span data-ttu-id="88fc2-118">名称</span><span class="sxs-lookup"><span data-stu-id="88fc2-118">Name</span></span>       | <span data-ttu-id="88fc2-119">说明</span><span class="sxs-lookup"><span data-stu-id="88fc2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="88fc2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="88fc2-120">Authorization</span></span>  | <span data-ttu-id="88fc2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88fc2-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="88fc2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="88fc2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="88fc2-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="88fc2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="88fc2-126">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="88fc2-126">workbook-session-id</span></span> | <span data-ttu-id="88fc2-127">要关闭的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="88fc2-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="88fc2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="88fc2-128">Request body</span></span>
<span data-ttu-id="88fc2-129">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="88fc2-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="88fc2-130">响应</span><span class="sxs-lookup"><span data-stu-id="88fc2-130">Response</span></span>

<span data-ttu-id="88fc2-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="88fc2-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88fc2-132">示例</span><span class="sxs-lookup"><span data-stu-id="88fc2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88fc2-133">请求</span><span class="sxs-lookup"><span data-stu-id="88fc2-133">Request</span></span>
<span data-ttu-id="88fc2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88fc2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="88fc2-135">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="88fc2-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="88fc2-136">响应</span><span class="sxs-lookup"><span data-stu-id="88fc2-136">Response</span></span>
<span data-ttu-id="88fc2-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88fc2-137">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="88fc2-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="88fc2-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="88fc2-139">语言</span><span class="sxs-lookup"><span data-stu-id="88fc2-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/close_excel_session-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88fc2-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="88fc2-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/close_excel_session-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
