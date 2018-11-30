---
title: 列出附件
description: 检索 attachment 对象列表。
ms.openlocfilehash: c9540db402a39cf8bf8f35318d06e7e699e9c7f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011030"
---
# <a name="list-attachments"></a><span data-ttu-id="0eda6-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="0eda6-103">List attachments</span></span>

<span data-ttu-id="0eda6-104">检索 attachment 对象列表。</span><span class="sxs-lookup"><span data-stu-id="0eda6-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0eda6-105">权限</span><span class="sxs-lookup"><span data-stu-id="0eda6-105">Permissions</span></span>
<span data-ttu-id="0eda6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0eda6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eda6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0eda6-108">Permission type</span></span>      | <span data-ttu-id="0eda6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0eda6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eda6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0eda6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0eda6-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0eda6-111">Mail.Read</span></span>    |
|<span data-ttu-id="0eda6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0eda6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eda6-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0eda6-113">Mail.Read</span></span>    |
|<span data-ttu-id="0eda6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0eda6-114">Application</span></span> | <span data-ttu-id="0eda6-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0eda6-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eda6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0eda6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0eda6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0eda6-117">Optional query parameters</span></span>
<span data-ttu-id="0eda6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0eda6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eda6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0eda6-119">Request headers</span></span>
| <span data-ttu-id="0eda6-120">名称</span><span class="sxs-lookup"><span data-stu-id="0eda6-120">Name</span></span>       | <span data-ttu-id="0eda6-121">类型</span><span class="sxs-lookup"><span data-stu-id="0eda6-121">Type</span></span> | <span data-ttu-id="0eda6-122">说明</span><span class="sxs-lookup"><span data-stu-id="0eda6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0eda6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eda6-123">Authorization</span></span>  | <span data-ttu-id="0eda6-124">string</span><span class="sxs-lookup"><span data-stu-id="0eda6-124">string</span></span>  | <span data-ttu-id="0eda6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0eda6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eda6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0eda6-127">Request body</span></span>
<span data-ttu-id="0eda6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0eda6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eda6-129">响应</span><span class="sxs-lookup"><span data-stu-id="0eda6-129">Response</span></span>

<span data-ttu-id="0eda6-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0eda6-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0eda6-131">示例</span><span class="sxs-lookup"><span data-stu-id="0eda6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0eda6-132">请求</span><span class="sxs-lookup"><span data-stu-id="0eda6-132">Request</span></span>
<span data-ttu-id="0eda6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0eda6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="0eda6-134">响应</span><span class="sxs-lookup"><span data-stu-id="0eda6-134">Response</span></span>
<span data-ttu-id="0eda6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0eda6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
