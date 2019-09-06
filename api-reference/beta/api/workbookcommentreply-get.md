---
title: 获取 workbookCommentReply
description: 检索 workbookcommentreply 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 282e650e3eb927b011187607b33b827400e3c6dd
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775837"
---
# <a name="get-workbookcommentreply"></a><span data-ttu-id="93e5a-103">获取 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="93e5a-103">Get workbookCommentReply</span></span>

<span data-ttu-id="93e5a-104">检索[workbookCommentReply](../resources/workbookcommentreply.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93e5a-104">Retrieve the properties and relationships of [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="93e5a-105">权限</span><span class="sxs-lookup"><span data-stu-id="93e5a-105">Permissions</span></span>

<span data-ttu-id="93e5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93e5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93e5a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="93e5a-108">Permission type</span></span>                        | <span data-ttu-id="93e5a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93e5a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="93e5a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93e5a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="93e5a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93e5a-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="93e5a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93e5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93e5a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="93e5a-113">Not supported.</span></span> |
| <span data-ttu-id="93e5a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="93e5a-114">Application</span></span>                            | <span data-ttu-id="93e5a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="93e5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93e5a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93e5a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /comments/{id}/replies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93e5a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="93e5a-117">Request headers</span></span>

| <span data-ttu-id="93e5a-118">名称</span><span class="sxs-lookup"><span data-stu-id="93e5a-118">Name</span></span>      |<span data-ttu-id="93e5a-119">说明</span><span class="sxs-lookup"><span data-stu-id="93e5a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93e5a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="93e5a-120">Authorization</span></span> | <span data-ttu-id="93e5a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93e5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93e5a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="93e5a-123">Request body</span></span>

<span data-ttu-id="93e5a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93e5a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93e5a-125">响应</span><span class="sxs-lookup"><span data-stu-id="93e5a-125">Response</span></span>

<span data-ttu-id="93e5a-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[workbookCommentReply](../resources/workbookcommentreply.md)对象。</span><span class="sxs-lookup"><span data-stu-id="93e5a-126">If successful, this method returns a `200 OK` response code and the requested [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93e5a-127">示例</span><span class="sxs-lookup"><span data-stu-id="93e5a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93e5a-128">请求</span><span class="sxs-lookup"><span data-stu-id="93e5a-128">Request</span></span>

<span data-ttu-id="93e5a-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="93e5a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/comments/{id}/replies/{id}
```

### <a name="response"></a><span data-ttu-id="93e5a-130">响应</span><span class="sxs-lookup"><span data-stu-id="93e5a-130">Response</span></span>

<span data-ttu-id="93e5a-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="93e5a-131">The following is an example of the response.</span></span>

> <span data-ttu-id="93e5a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="93e5a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is text of comment.",
  "contentType": "Plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
