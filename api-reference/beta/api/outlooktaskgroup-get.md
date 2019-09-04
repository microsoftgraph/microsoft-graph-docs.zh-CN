---
title: 获取 outlookTaskGroup
description: 获取指定的 Outlook 任务组的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2ea03923ceffa9e99b58b2729c00ceb904e049b5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725883"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="a94a7-103">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a94a7-103">Get outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a94a7-104">获取指定的 Outlook 任务组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a94a7-104">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="a94a7-105">权限</span><span class="sxs-lookup"><span data-stu-id="a94a7-105">Permissions</span></span>
<span data-ttu-id="a94a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a94a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a94a7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a94a7-108">Permission type</span></span>      | <span data-ttu-id="a94a7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a94a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a94a7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a94a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a94a7-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a94a7-111">Tasks.Read</span></span>    |
|<span data-ttu-id="a94a7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a94a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a94a7-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a94a7-113">Tasks.Read</span></span>    |
|<span data-ttu-id="a94a7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a94a7-114">Application</span></span> | <span data-ttu-id="a94a7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a94a7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a94a7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a94a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a94a7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a94a7-117">Optional query parameters</span></span>
<span data-ttu-id="a94a7-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a94a7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a94a7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a94a7-119">Request headers</span></span>
| <span data-ttu-id="a94a7-120">名称</span><span class="sxs-lookup"><span data-stu-id="a94a7-120">Name</span></span>      |<span data-ttu-id="a94a7-121">说明</span><span class="sxs-lookup"><span data-stu-id="a94a7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a94a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a94a7-122">Authorization</span></span>  | <span data-ttu-id="a94a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a94a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a94a7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a94a7-125">Request body</span></span>
<span data-ttu-id="a94a7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a94a7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a94a7-127">响应</span><span class="sxs-lookup"><span data-stu-id="a94a7-127">Response</span></span>

<span data-ttu-id="a94a7-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a94a7-128">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a94a7-129">示例</span><span class="sxs-lookup"><span data-stu-id="a94a7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a94a7-130">请求</span><span class="sxs-lookup"><span data-stu-id="a94a7-130">Request</span></span>
<span data-ttu-id="a94a7-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a94a7-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a94a7-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a94a7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a94a7-133">C#</span><span class="sxs-lookup"><span data-stu-id="a94a7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a94a7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a94a7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a94a7-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="a94a7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a94a7-136">响应</span><span class="sxs-lookup"><span data-stu-id="a94a7-136">Response</span></span>
<span data-ttu-id="a94a7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a94a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
