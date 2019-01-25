---
title: 列出附件
description: 检索 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 06c36179bcf5c79b287f6107c6c62d2a7dee89d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529675"
---
# <a name="list-attachments"></a><span data-ttu-id="23f1b-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="23f1b-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f1b-104">检索 attachment 对象列表。</span><span class="sxs-lookup"><span data-stu-id="23f1b-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="23f1b-105">权限</span><span class="sxs-lookup"><span data-stu-id="23f1b-105">Permissions</span></span>
<span data-ttu-id="23f1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23f1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23f1b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="23f1b-108">Permission type</span></span>      | <span data-ttu-id="23f1b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23f1b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f1b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23f1b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23f1b-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="23f1b-111">Mail.Read</span></span>    |
|<span data-ttu-id="23f1b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23f1b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f1b-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="23f1b-113">Mail.Read</span></span>    |
|<span data-ttu-id="23f1b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="23f1b-114">Application</span></span> | <span data-ttu-id="23f1b-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="23f1b-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="23f1b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23f1b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23f1b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23f1b-117">Optional query parameters</span></span>
<span data-ttu-id="23f1b-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23f1b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23f1b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="23f1b-119">Request headers</span></span>
| <span data-ttu-id="23f1b-120">名称</span><span class="sxs-lookup"><span data-stu-id="23f1b-120">Name</span></span>       | <span data-ttu-id="23f1b-121">类型</span><span class="sxs-lookup"><span data-stu-id="23f1b-121">Type</span></span> | <span data-ttu-id="23f1b-122">说明</span><span class="sxs-lookup"><span data-stu-id="23f1b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23f1b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23f1b-123">Authorization</span></span>  | <span data-ttu-id="23f1b-124">string</span><span class="sxs-lookup"><span data-stu-id="23f1b-124">string</span></span>  | <span data-ttu-id="23f1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23f1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23f1b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="23f1b-127">Request body</span></span>
<span data-ttu-id="23f1b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23f1b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23f1b-129">响应</span><span class="sxs-lookup"><span data-stu-id="23f1b-129">Response</span></span>

<span data-ttu-id="23f1b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="23f1b-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23f1b-131">示例</span><span class="sxs-lookup"><span data-stu-id="23f1b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23f1b-132">请求</span><span class="sxs-lookup"><span data-stu-id="23f1b-132">Request</span></span>
<span data-ttu-id="23f1b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23f1b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="23f1b-134">响应</span><span class="sxs-lookup"><span data-stu-id="23f1b-134">Response</span></span>
<span data-ttu-id="23f1b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23f1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
