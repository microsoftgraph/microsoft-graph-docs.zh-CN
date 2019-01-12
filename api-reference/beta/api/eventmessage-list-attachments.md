---
title: 列出附件
description: 检索 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5b54e26acbb08b7960693b3e5a1e531fc4c20708
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951346"
---
# <a name="list-attachments"></a><span data-ttu-id="d8d6f-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="d8d6f-103">List attachments</span></span>

> <span data-ttu-id="d8d6f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8d6f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8d6f-106">检索 attachment 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-106">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8d6f-107">权限</span><span class="sxs-lookup"><span data-stu-id="d8d6f-107">Permissions</span></span>
<span data-ttu-id="d8d6f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8d6f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8d6f-110">Permission type</span></span>      | <span data-ttu-id="d8d6f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8d6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8d6f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8d6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8d6f-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d8d6f-113">Mail.Read</span></span>    |
|<span data-ttu-id="d8d6f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8d6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8d6f-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d8d6f-115">Mail.Read</span></span>    |
|<span data-ttu-id="d8d6f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8d6f-116">Application</span></span> | <span data-ttu-id="d8d6f-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d8d6f-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8d6f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8d6f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8d6f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d8d6f-119">Optional query parameters</span></span>
<span data-ttu-id="d8d6f-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8d6f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8d6f-121">Request headers</span></span>
| <span data-ttu-id="d8d6f-122">名称</span><span class="sxs-lookup"><span data-stu-id="d8d6f-122">Name</span></span>       | <span data-ttu-id="d8d6f-123">类型</span><span class="sxs-lookup"><span data-stu-id="d8d6f-123">Type</span></span> | <span data-ttu-id="d8d6f-124">说明</span><span class="sxs-lookup"><span data-stu-id="d8d6f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8d6f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8d6f-125">Authorization</span></span>  | <span data-ttu-id="d8d6f-126">string</span><span class="sxs-lookup"><span data-stu-id="d8d6f-126">string</span></span>  | <span data-ttu-id="d8d6f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8d6f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8d6f-129">Request body</span></span>
<span data-ttu-id="d8d6f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8d6f-131">响应</span><span class="sxs-lookup"><span data-stu-id="d8d6f-131">Response</span></span>

<span data-ttu-id="d8d6f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8d6f-133">示例</span><span class="sxs-lookup"><span data-stu-id="d8d6f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8d6f-134">请求</span><span class="sxs-lookup"><span data-stu-id="d8d6f-134">Request</span></span>
<span data-ttu-id="d8d6f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="d8d6f-136">响应</span><span class="sxs-lookup"><span data-stu-id="d8d6f-136">Response</span></span>
<span data-ttu-id="d8d6f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8d6f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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
