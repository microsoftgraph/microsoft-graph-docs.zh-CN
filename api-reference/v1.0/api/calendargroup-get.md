---
title: 获取 calendarGroup
description: 检索 calendargroup 对象的属性和关系。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 772e4d0001fe96a41ea3cbcda495c5029825e123
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406154"
---
# <a name="get-calendargroup"></a><span data-ttu-id="3f840-103">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="3f840-103">Get calendarGroup</span></span>

<span data-ttu-id="3f840-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f840-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f840-105">检索 calendargroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f840-105">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f840-106">权限</span><span class="sxs-lookup"><span data-stu-id="3f840-106">Permissions</span></span>

<span data-ttu-id="3f840-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f840-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f840-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f840-109">Permission type</span></span>                        | <span data-ttu-id="3f840-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f840-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3f840-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f840-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f840-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3f840-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="3f840-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f840-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f840-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3f840-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="3f840-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f840-115">Application</span></span>                            | <span data-ttu-id="3f840-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3f840-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="3f840-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f840-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3f840-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3f840-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3f840-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3f840-119">Optional query parameters</span></span>

<span data-ttu-id="3f840-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3f840-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f840-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f840-121">Request headers</span></span>

| <span data-ttu-id="3f840-122">名称</span><span class="sxs-lookup"><span data-stu-id="3f840-122">Name</span></span>          | <span data-ttu-id="3f840-123">类型</span><span class="sxs-lookup"><span data-stu-id="3f840-123">Type</span></span>   | <span data-ttu-id="3f840-124">说明</span><span class="sxs-lookup"><span data-stu-id="3f840-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="3f840-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f840-125">Authorization</span></span> | <span data-ttu-id="3f840-126">string</span><span class="sxs-lookup"><span data-stu-id="3f840-126">string</span></span> | <span data-ttu-id="3f840-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f840-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f840-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f840-129">Request body</span></span>

<span data-ttu-id="3f840-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f840-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f840-131">响应</span><span class="sxs-lookup"><span data-stu-id="3f840-131">Response</span></span>

<span data-ttu-id="3f840-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f840-132">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f840-133">示例</span><span class="sxs-lookup"><span data-stu-id="3f840-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3f840-134">请求</span><span class="sxs-lookup"><span data-stu-id="3f840-134">Request</span></span>

<span data-ttu-id="3f840-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f840-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f840-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f840-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="3f840-137">C#</span><span class="sxs-lookup"><span data-stu-id="3f840-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f840-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f840-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f840-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f840-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f840-140">Java</span><span class="sxs-lookup"><span data-stu-id="3f840-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f840-141">响应</span><span class="sxs-lookup"><span data-stu-id="3f840-141">Response</span></span>

<span data-ttu-id="3f840-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f840-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->