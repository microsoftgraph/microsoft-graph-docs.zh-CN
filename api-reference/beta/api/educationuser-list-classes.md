---
title: 列出课程
description: '检索 class 对象的列表。 请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8a3ddcbca26354b10326155afa6530ce4b9a6278
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415867"
---
# <a name="list-classes"></a><span data-ttu-id="0c0de-104">列出课程</span><span class="sxs-lookup"><span data-stu-id="0c0de-104">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c0de-105">检索 class 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0c0de-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="0c0de-106">请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。</span><span class="sxs-lookup"><span data-stu-id="0c0de-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="0c0de-107">权限</span><span class="sxs-lookup"><span data-stu-id="0c0de-107">Permissions</span></span>
<span data-ttu-id="0c0de-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c0de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c0de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c0de-110">Permission type</span></span>      | <span data-ttu-id="0c0de-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c0de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c0de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c0de-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c0de-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="0c0de-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="0c0de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c0de-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c0de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c0de-115">Not supported.</span></span>  |
|<span data-ttu-id="0c0de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c0de-116">Application</span></span> | <span data-ttu-id="0c0de-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0de-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c0de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c0de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0c0de-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0c0de-119">Optional query parameters</span></span>
<span data-ttu-id="0c0de-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0c0de-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c0de-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c0de-121">Request headers</span></span>
| <span data-ttu-id="0c0de-122">标头</span><span class="sxs-lookup"><span data-stu-id="0c0de-122">Header</span></span>       | <span data-ttu-id="0c0de-123">值</span><span class="sxs-lookup"><span data-stu-id="0c0de-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c0de-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c0de-124">Authorization</span></span>  | <span data-ttu-id="0c0de-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c0de-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c0de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c0de-127">Request body</span></span>
<span data-ttu-id="0c0de-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c0de-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0c0de-129">响应</span><span class="sxs-lookup"><span data-stu-id="0c0de-129">Response</span></span>
<span data-ttu-id="0c0de-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0c0de-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c0de-131">示例</span><span class="sxs-lookup"><span data-stu-id="0c0de-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c0de-132">请求</span><span class="sxs-lookup"><span data-stu-id="0c0de-132">Request</span></span>
<span data-ttu-id="0c0de-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c0de-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c0de-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0c0de-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c0de-135">C#</span><span class="sxs-lookup"><span data-stu-id="0c0de-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c0de-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c0de-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c0de-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="0c0de-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0c0de-138">响应</span><span class="sxs-lookup"><span data-stu-id="0c0de-138">Response</span></span>
<span data-ttu-id="0c0de-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0c0de-139">The following is an example of the response.</span></span> 

><span data-ttu-id="0c0de-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0c0de-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
