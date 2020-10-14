---
title: 列出附件
description: 获取附加到 Outlook 任务的附件对象的列表。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0f8e0b76f84cbacee562493937998ebfbc6423f6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459016"
---
# <a name="list-attachments-deprecated"></a><span data-ttu-id="b298b-103">列出附件 (弃用) </span><span class="sxs-lookup"><span data-stu-id="b298b-103">List attachments (deprecated)</span></span>

<span data-ttu-id="b298b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b298b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="b298b-105">获取附加到 Outlook 任务的 [附件](../resources/attachment.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b298b-105">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="b298b-106">权限</span><span class="sxs-lookup"><span data-stu-id="b298b-106">Permissions</span></span>

<span data-ttu-id="b298b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b298b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b298b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b298b-109">Permission type</span></span>      | <span data-ttu-id="b298b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b298b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b298b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b298b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b298b-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="b298b-112">Tasks.Read</span></span>    |
|<span data-ttu-id="b298b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b298b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b298b-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="b298b-114">Tasks.Read</span></span>    |
|<span data-ttu-id="b298b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b298b-115">Application</span></span> | <span data-ttu-id="b298b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b298b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b298b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b298b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b298b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b298b-118">Optional query parameters</span></span>

<span data-ttu-id="b298b-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b298b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b298b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b298b-120">Request headers</span></span>

| <span data-ttu-id="b298b-121">名称</span><span class="sxs-lookup"><span data-stu-id="b298b-121">Name</span></span>      |<span data-ttu-id="b298b-122">说明</span><span class="sxs-lookup"><span data-stu-id="b298b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b298b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b298b-123">Authorization</span></span>  | <span data-ttu-id="b298b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b298b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b298b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b298b-126">Request body</span></span>

<span data-ttu-id="b298b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b298b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b298b-128">响应</span><span class="sxs-lookup"><span data-stu-id="b298b-128">Response</span></span>

<span data-ttu-id="b298b-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [附件](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b298b-129">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b298b-130">示例</span><span class="sxs-lookup"><span data-stu-id="b298b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b298b-131">请求</span><span class="sxs-lookup"><span data-stu-id="b298b-131">Request</span></span>

<span data-ttu-id="b298b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b298b-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b298b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b298b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="b298b-134">C#</span><span class="sxs-lookup"><span data-stu-id="b298b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b298b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b298b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b298b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b298b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b298b-137">响应</span><span class="sxs-lookup"><span data-stu-id="b298b-137">Response</span></span>

<span data-ttu-id="b298b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b298b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
