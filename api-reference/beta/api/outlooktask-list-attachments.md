---
title: 列出附件
description: 获取附加到 Outlook 任务的附件对象的列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 38da8bcbd0601bbca201b157db3d49d7016e2de3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988718"
---
# <a name="list-attachments"></a><span data-ttu-id="c85b5-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="c85b5-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c85b5-104">获取附加到 Outlook 任务的[附件](../resources/attachment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c85b5-104">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="c85b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="c85b5-105">Permissions</span></span>

<span data-ttu-id="c85b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c85b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c85b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c85b5-108">Permission type</span></span>      | <span data-ttu-id="c85b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c85b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c85b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c85b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c85b5-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c85b5-111">Tasks.Read</span></span>    |
|<span data-ttu-id="c85b5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c85b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c85b5-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c85b5-113">Tasks.Read</span></span>    |
|<span data-ttu-id="c85b5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c85b5-114">Application</span></span> | <span data-ttu-id="c85b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c85b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c85b5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c85b5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c85b5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c85b5-117">Optional query parameters</span></span>

<span data-ttu-id="c85b5-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c85b5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c85b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c85b5-119">Request headers</span></span>

| <span data-ttu-id="c85b5-120">名称</span><span class="sxs-lookup"><span data-stu-id="c85b5-120">Name</span></span>      |<span data-ttu-id="c85b5-121">说明</span><span class="sxs-lookup"><span data-stu-id="c85b5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c85b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c85b5-122">Authorization</span></span>  | <span data-ttu-id="c85b5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c85b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c85b5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c85b5-125">Request body</span></span>

<span data-ttu-id="c85b5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c85b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c85b5-127">响应</span><span class="sxs-lookup"><span data-stu-id="c85b5-127">Response</span></span>

<span data-ttu-id="c85b5-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[附件](../resources/attachment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c85b5-128">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c85b5-129">示例</span><span class="sxs-lookup"><span data-stu-id="c85b5-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c85b5-130">请求</span><span class="sxs-lookup"><span data-stu-id="c85b5-130">Request</span></span>

<span data-ttu-id="c85b5-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c85b5-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c85b5-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c85b5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c85b5-133">C#</span><span class="sxs-lookup"><span data-stu-id="c85b5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c85b5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="c85b5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c85b5-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="c85b5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c85b5-136">Java</span><span class="sxs-lookup"><span data-stu-id="c85b5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlook-task-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c85b5-137">响应</span><span class="sxs-lookup"><span data-stu-id="c85b5-137">Response</span></span>

<span data-ttu-id="c85b5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c85b5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
