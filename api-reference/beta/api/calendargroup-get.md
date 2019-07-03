---
title: 获取 calendarGroup
description: 检索 calendargroup 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d7dcb00497c6824678f77c87ab7836c77736748f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438879"
---
# <a name="get-calendargroup"></a><span data-ttu-id="8305c-103">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="8305c-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8305c-104">检索 calendargroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8305c-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8305c-105">权限</span><span class="sxs-lookup"><span data-stu-id="8305c-105">Permissions</span></span>

<span data-ttu-id="8305c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8305c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8305c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8305c-108">Permission type</span></span>                        | <span data-ttu-id="8305c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8305c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8305c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8305c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8305c-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8305c-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="8305c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8305c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8305c-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8305c-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="8305c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8305c-114">Application</span></span>                            | <span data-ttu-id="8305c-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8305c-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="8305c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8305c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="8305c-117">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="8305c-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8305c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8305c-118">Optional query parameters</span></span>

<span data-ttu-id="8305c-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8305c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8305c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8305c-120">Request headers</span></span>

| <span data-ttu-id="8305c-121">名称</span><span class="sxs-lookup"><span data-stu-id="8305c-121">Name</span></span>          | <span data-ttu-id="8305c-122">类型</span><span class="sxs-lookup"><span data-stu-id="8305c-122">Type</span></span>   | <span data-ttu-id="8305c-123">说明</span><span class="sxs-lookup"><span data-stu-id="8305c-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="8305c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8305c-124">Authorization</span></span> | <span data-ttu-id="8305c-125">string</span><span class="sxs-lookup"><span data-stu-id="8305c-125">string</span></span> | <span data-ttu-id="8305c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8305c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8305c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8305c-128">Request body</span></span>

<span data-ttu-id="8305c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8305c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8305c-130">响应</span><span class="sxs-lookup"><span data-stu-id="8305c-130">Response</span></span>

<span data-ttu-id="8305c-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8305c-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8305c-132">示例</span><span class="sxs-lookup"><span data-stu-id="8305c-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8305c-133">请求</span><span class="sxs-lookup"><span data-stu-id="8305c-133">Request</span></span>

<span data-ttu-id="8305c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8305c-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8305c-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8305c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8305c-136">C#</span><span class="sxs-lookup"><span data-stu-id="8305c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8305c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8305c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8305c-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="8305c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8305c-139">响应</span><span class="sxs-lookup"><span data-stu-id="8305c-139">Response</span></span>

<span data-ttu-id="8305c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8305c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
