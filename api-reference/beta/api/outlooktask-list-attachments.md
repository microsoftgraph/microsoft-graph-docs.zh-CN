---
title: 列出附件
description: 获取附件对象附加到 Outlook 任务的列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9d330f0a86b99bbd667ff1f32a5b5fc549dfc7f2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526905"
---
# <a name="list-attachments"></a><span data-ttu-id="9fe68-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="9fe68-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fe68-104">获取[附件](../resources/attachment.md)对象附加到 Outlook 任务的列表。</span><span class="sxs-lookup"><span data-stu-id="9fe68-104">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fe68-105">权限</span><span class="sxs-lookup"><span data-stu-id="9fe68-105">Permissions</span></span>

<span data-ttu-id="9fe68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fe68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fe68-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fe68-108">Permission type</span></span>      | <span data-ttu-id="9fe68-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fe68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fe68-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fe68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9fe68-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="9fe68-111">Tasks.Read</span></span>    |
|<span data-ttu-id="9fe68-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fe68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fe68-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="9fe68-113">Tasks.Read</span></span>    |
|<span data-ttu-id="9fe68-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fe68-114">Application</span></span> | <span data-ttu-id="9fe68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fe68-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fe68-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fe68-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fe68-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9fe68-117">Optional query parameters</span></span>

<span data-ttu-id="9fe68-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9fe68-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fe68-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fe68-119">Request headers</span></span>

| <span data-ttu-id="9fe68-120">名称</span><span class="sxs-lookup"><span data-stu-id="9fe68-120">Name</span></span>      |<span data-ttu-id="9fe68-121">说明</span><span class="sxs-lookup"><span data-stu-id="9fe68-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9fe68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fe68-122">Authorization</span></span>  | <span data-ttu-id="9fe68-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fe68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fe68-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fe68-125">Request body</span></span>

<span data-ttu-id="9fe68-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9fe68-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fe68-127">响应</span><span class="sxs-lookup"><span data-stu-id="9fe68-127">Response</span></span>

<span data-ttu-id="9fe68-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[attachment](../resources/attachment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="9fe68-128">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fe68-129">示例</span><span class="sxs-lookup"><span data-stu-id="9fe68-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fe68-130">请求</span><span class="sxs-lookup"><span data-stu-id="9fe68-130">Request</span></span>

<span data-ttu-id="9fe68-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fe68-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="9fe68-132">响应</span><span class="sxs-lookup"><span data-stu-id="9fe68-132">Response</span></span>

<span data-ttu-id="9fe68-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fe68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
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
    "Error: /api-reference/beta/api/outlooktask-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
