---
title: 列出附件
description: 检索 attachment 对象列表。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e9b5a8537fc4e3a673a76573782dc70721229d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052409"
---
# <a name="list-attachments"></a><span data-ttu-id="1d276-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="1d276-103">List attachments</span></span>

<span data-ttu-id="1d276-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d276-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d276-105">检索 attachment 对象列表。</span><span class="sxs-lookup"><span data-stu-id="1d276-105">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d276-106">权限</span><span class="sxs-lookup"><span data-stu-id="1d276-106">Permissions</span></span>
<span data-ttu-id="1d276-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d276-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d276-109">Permission type</span></span>      | <span data-ttu-id="1d276-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d276-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d276-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d276-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d276-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d276-112">Mail.Read</span></span>    |
|<span data-ttu-id="1d276-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d276-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d276-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d276-114">Mail.Read</span></span>    |
|<span data-ttu-id="1d276-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d276-115">Application</span></span> | <span data-ttu-id="1d276-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d276-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d276-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d276-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d276-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1d276-118">Optional query parameters</span></span>
<span data-ttu-id="1d276-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1d276-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d276-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d276-120">Request headers</span></span>
| <span data-ttu-id="1d276-121">名称</span><span class="sxs-lookup"><span data-stu-id="1d276-121">Name</span></span>       | <span data-ttu-id="1d276-122">类型</span><span class="sxs-lookup"><span data-stu-id="1d276-122">Type</span></span> | <span data-ttu-id="1d276-123">说明</span><span class="sxs-lookup"><span data-stu-id="1d276-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1d276-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d276-124">Authorization</span></span>  | <span data-ttu-id="1d276-125">string</span><span class="sxs-lookup"><span data-stu-id="1d276-125">string</span></span>  | <span data-ttu-id="1d276-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d276-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d276-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d276-128">Request body</span></span>
<span data-ttu-id="1d276-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d276-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d276-130">响应</span><span class="sxs-lookup"><span data-stu-id="1d276-130">Response</span></span>

<span data-ttu-id="1d276-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d276-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d276-132">示例</span><span class="sxs-lookup"><span data-stu-id="1d276-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d276-133">请求</span><span class="sxs-lookup"><span data-stu-id="1d276-133">Request</span></span>
<span data-ttu-id="1d276-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d276-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d276-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d276-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="1d276-136">C#</span><span class="sxs-lookup"><span data-stu-id="1d276-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d276-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d276-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d276-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d276-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d276-139">Java</span><span class="sxs-lookup"><span data-stu-id="1d276-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/eventmessage-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1d276-140">响应</span><span class="sxs-lookup"><span data-stu-id="1d276-140">Response</span></span>
<span data-ttu-id="1d276-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1d276-141">Here is an example of the response.</span></span> <span data-ttu-id="1d276-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1d276-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "eventmessage_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
