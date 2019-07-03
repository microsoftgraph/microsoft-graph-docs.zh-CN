---
title: 获取 outlookTaskGroup
description: 获取指定的 Outlook 任务组的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7d5db2094f73e9390810b224332653d135e9a3d8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447255"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="e7395-103">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="e7395-103">Get outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7395-104">获取指定的 Outlook 任务组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7395-104">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7395-105">权限</span><span class="sxs-lookup"><span data-stu-id="e7395-105">Permissions</span></span>
<span data-ttu-id="e7395-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7395-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7395-108">Permission type</span></span>      | <span data-ttu-id="e7395-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7395-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7395-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7395-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7395-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e7395-111">Tasks.Read</span></span>    |
|<span data-ttu-id="e7395-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7395-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7395-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e7395-113">Tasks.Read</span></span>    |
|<span data-ttu-id="e7395-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7395-114">Application</span></span> | <span data-ttu-id="e7395-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7395-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7395-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7395-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7395-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e7395-117">Optional query parameters</span></span>
<span data-ttu-id="e7395-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e7395-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7395-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7395-119">Request headers</span></span>
| <span data-ttu-id="e7395-120">名称</span><span class="sxs-lookup"><span data-stu-id="e7395-120">Name</span></span>      |<span data-ttu-id="e7395-121">说明</span><span class="sxs-lookup"><span data-stu-id="e7395-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7395-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7395-122">Authorization</span></span>  | <span data-ttu-id="e7395-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7395-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7395-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7395-125">Request body</span></span>
<span data-ttu-id="e7395-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e7395-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7395-127">响应</span><span class="sxs-lookup"><span data-stu-id="e7395-127">Response</span></span>

<span data-ttu-id="e7395-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7395-128">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7395-129">示例</span><span class="sxs-lookup"><span data-stu-id="e7395-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7395-130">请求</span><span class="sxs-lookup"><span data-stu-id="e7395-130">Request</span></span>
<span data-ttu-id="e7395-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7395-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e7395-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e7395-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7395-133">C#</span><span class="sxs-lookup"><span data-stu-id="e7395-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7395-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7395-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7395-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="e7395-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7395-136">响应</span><span class="sxs-lookup"><span data-stu-id="e7395-136">Response</span></span>
<span data-ttu-id="e7395-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7395-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
