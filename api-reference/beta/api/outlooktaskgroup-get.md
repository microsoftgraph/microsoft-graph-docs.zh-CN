---
title: 获取 outlookTaskGroup
description: 获取指定的 Outlook 任务组的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5840189cba9e340c9562315c5fbfcd3d76b7d416
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596207"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="80077-103">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="80077-103">Get outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80077-104">获取指定的 Outlook 任务组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80077-104">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="80077-105">权限</span><span class="sxs-lookup"><span data-stu-id="80077-105">Permissions</span></span>
<span data-ttu-id="80077-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80077-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="80077-108">Permission type</span></span>      | <span data-ttu-id="80077-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80077-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80077-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80077-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80077-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="80077-111">Tasks.Read</span></span>    |
|<span data-ttu-id="80077-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80077-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80077-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="80077-113">Tasks.Read</span></span>    |
|<span data-ttu-id="80077-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="80077-114">Application</span></span> | <span data-ttu-id="80077-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80077-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80077-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80077-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="80077-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80077-117">Optional query parameters</span></span>
<span data-ttu-id="80077-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80077-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80077-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="80077-119">Request headers</span></span>
| <span data-ttu-id="80077-120">名称</span><span class="sxs-lookup"><span data-stu-id="80077-120">Name</span></span>      |<span data-ttu-id="80077-121">说明</span><span class="sxs-lookup"><span data-stu-id="80077-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="80077-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80077-122">Authorization</span></span>  | <span data-ttu-id="80077-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80077-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80077-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80077-125">Request body</span></span>
<span data-ttu-id="80077-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80077-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80077-127">响应</span><span class="sxs-lookup"><span data-stu-id="80077-127">Response</span></span>

<span data-ttu-id="80077-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80077-128">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80077-129">示例</span><span class="sxs-lookup"><span data-stu-id="80077-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80077-130">请求</span><span class="sxs-lookup"><span data-stu-id="80077-130">Request</span></span>
<span data-ttu-id="80077-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80077-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
##### <a name="response"></a><span data-ttu-id="80077-132">响应</span><span class="sxs-lookup"><span data-stu-id="80077-132">Response</span></span>
<span data-ttu-id="80077-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80077-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="80077-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="80077-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="80077-137">语言</span><span class="sxs-lookup"><span data-stu-id="80077-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_outlooktaskgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80077-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="80077-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_outlooktaskgroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlooktaskgroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskgroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
