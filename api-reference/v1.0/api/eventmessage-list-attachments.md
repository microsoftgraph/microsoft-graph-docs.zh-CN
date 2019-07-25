---
title: 列出附件
description: 检索 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6207a185284e0f86a6b45ebc7311522c3241541a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888221"
---
# <a name="list-attachments"></a><span data-ttu-id="3a1e5-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="3a1e5-103">List attachments</span></span>

<span data-ttu-id="3a1e5-104">检索 attachment 对象列表。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a1e5-105">权限</span><span class="sxs-lookup"><span data-stu-id="3a1e5-105">Permissions</span></span>
<span data-ttu-id="3a1e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a1e5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a1e5-108">Permission type</span></span>      | <span data-ttu-id="3a1e5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a1e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a1e5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a1e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a1e5-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a1e5-111">Mail.Read</span></span>    |
|<span data-ttu-id="3a1e5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a1e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a1e5-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a1e5-113">Mail.Read</span></span>    |
|<span data-ttu-id="3a1e5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a1e5-114">Application</span></span> | <span data-ttu-id="3a1e5-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a1e5-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a1e5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a1e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a1e5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3a1e5-117">Optional query parameters</span></span>
<span data-ttu-id="3a1e5-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a1e5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a1e5-119">Request headers</span></span>
| <span data-ttu-id="3a1e5-120">名称</span><span class="sxs-lookup"><span data-stu-id="3a1e5-120">Name</span></span>       | <span data-ttu-id="3a1e5-121">类型</span><span class="sxs-lookup"><span data-stu-id="3a1e5-121">Type</span></span> | <span data-ttu-id="3a1e5-122">说明</span><span class="sxs-lookup"><span data-stu-id="3a1e5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3a1e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a1e5-123">Authorization</span></span>  | <span data-ttu-id="3a1e5-124">string</span><span class="sxs-lookup"><span data-stu-id="3a1e5-124">string</span></span>  | <span data-ttu-id="3a1e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a1e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a1e5-127">Request body</span></span>
<span data-ttu-id="3a1e5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a1e5-129">响应</span><span class="sxs-lookup"><span data-stu-id="3a1e5-129">Response</span></span>

<span data-ttu-id="3a1e5-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a1e5-131">示例</span><span class="sxs-lookup"><span data-stu-id="3a1e5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a1e5-132">请求</span><span class="sxs-lookup"><span data-stu-id="3a1e5-132">Request</span></span>
<span data-ttu-id="3a1e5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3a1e5-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3a1e5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a1e5-135">C#</span><span class="sxs-lookup"><span data-stu-id="3a1e5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a1e5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a1e5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a1e5-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="3a1e5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3a1e5-138">Java</span><span class="sxs-lookup"><span data-stu-id="3a1e5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/eventmessage-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3a1e5-139">响应</span><span class="sxs-lookup"><span data-stu-id="3a1e5-139">Response</span></span>
<span data-ttu-id="3a1e5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a1e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
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
      "contentBytes": "base64-contentBytes-value",
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
