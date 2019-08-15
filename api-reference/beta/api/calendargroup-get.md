---
title: 获取 calendarGroup
description: 检索 calendargroup 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f2e6a98c0cdb194caa3c47e7ea6623e1721d5f19
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419067"
---
# <a name="get-calendargroup"></a><span data-ttu-id="72877-103">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="72877-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72877-104">检索 calendargroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72877-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72877-105">权限</span><span class="sxs-lookup"><span data-stu-id="72877-105">Permissions</span></span>

<span data-ttu-id="72877-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72877-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="72877-108">Permission type</span></span>                        | <span data-ttu-id="72877-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72877-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="72877-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72877-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="72877-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72877-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="72877-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72877-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72877-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72877-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="72877-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="72877-114">Application</span></span>                            | <span data-ttu-id="72877-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72877-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="72877-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72877-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="72877-117">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="72877-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72877-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72877-118">Optional query parameters</span></span>

<span data-ttu-id="72877-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72877-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72877-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="72877-120">Request headers</span></span>

| <span data-ttu-id="72877-121">名称</span><span class="sxs-lookup"><span data-stu-id="72877-121">Name</span></span>          | <span data-ttu-id="72877-122">类型</span><span class="sxs-lookup"><span data-stu-id="72877-122">Type</span></span>   | <span data-ttu-id="72877-123">说明</span><span class="sxs-lookup"><span data-stu-id="72877-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="72877-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72877-124">Authorization</span></span> | <span data-ttu-id="72877-125">string</span><span class="sxs-lookup"><span data-stu-id="72877-125">string</span></span> | <span data-ttu-id="72877-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72877-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72877-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="72877-128">Request body</span></span>

<span data-ttu-id="72877-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72877-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72877-130">响应</span><span class="sxs-lookup"><span data-stu-id="72877-130">Response</span></span>

<span data-ttu-id="72877-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72877-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72877-132">示例</span><span class="sxs-lookup"><span data-stu-id="72877-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="72877-133">请求</span><span class="sxs-lookup"><span data-stu-id="72877-133">Request</span></span>

<span data-ttu-id="72877-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72877-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72877-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="72877-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72877-136">C#</span><span class="sxs-lookup"><span data-stu-id="72877-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72877-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72877-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72877-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="72877-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72877-139">响应</span><span class="sxs-lookup"><span data-stu-id="72877-139">Response</span></span>

<span data-ttu-id="72877-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72877-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
