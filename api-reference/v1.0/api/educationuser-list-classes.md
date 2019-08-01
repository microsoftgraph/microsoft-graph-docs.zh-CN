---
title: 列出课程
description: '检索 class 对象的列表。 请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00ba036c3fd28d253842839537e52fd66d792e29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006764"
---
# <a name="list-classes"></a><span data-ttu-id="c25db-104">列出课程</span><span class="sxs-lookup"><span data-stu-id="c25db-104">List classes</span></span>

<span data-ttu-id="c25db-105">检索 class 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c25db-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="c25db-106">请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。</span><span class="sxs-lookup"><span data-stu-id="c25db-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="c25db-107">权限</span><span class="sxs-lookup"><span data-stu-id="c25db-107">Permissions</span></span>
<span data-ttu-id="c25db-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c25db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c25db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c25db-110">Permission type</span></span>      | <span data-ttu-id="c25db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c25db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c25db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c25db-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c25db-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c25db-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c25db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c25db-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c25db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c25db-115">Not supported.</span></span>  |
|<span data-ttu-id="c25db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c25db-116">Application</span></span> | <span data-ttu-id="c25db-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c25db-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c25db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c25db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c25db-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c25db-119">Optional query parameters</span></span>
<span data-ttu-id="c25db-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c25db-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c25db-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c25db-121">Request headers</span></span>
| <span data-ttu-id="c25db-122">标头</span><span class="sxs-lookup"><span data-stu-id="c25db-122">Header</span></span>       | <span data-ttu-id="c25db-123">值</span><span class="sxs-lookup"><span data-stu-id="c25db-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c25db-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c25db-124">Authorization</span></span>  | <span data-ttu-id="c25db-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c25db-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c25db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c25db-127">Request body</span></span>
<span data-ttu-id="c25db-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c25db-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c25db-129">响应</span><span class="sxs-lookup"><span data-stu-id="c25db-129">Response</span></span>
<span data-ttu-id="c25db-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c25db-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c25db-131">示例</span><span class="sxs-lookup"><span data-stu-id="c25db-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c25db-132">请求</span><span class="sxs-lookup"><span data-stu-id="c25db-132">Request</span></span>
<span data-ttu-id="c25db-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c25db-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c25db-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c25db-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c25db-135">C#</span><span class="sxs-lookup"><span data-stu-id="c25db-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c25db-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c25db-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c25db-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="c25db-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c25db-138">Java</span><span class="sxs-lookup"><span data-stu-id="c25db-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c25db-139">响应</span><span class="sxs-lookup"><span data-stu-id="c25db-139">Response</span></span>
<span data-ttu-id="c25db-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c25db-140">The following is an example of the response.</span></span> 

><span data-ttu-id="c25db-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c25db-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
