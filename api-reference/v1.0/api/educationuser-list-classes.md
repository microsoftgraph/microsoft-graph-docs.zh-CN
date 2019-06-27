---
title: 列出课程
description: '检索 class 对象的列表。 请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4cc312917f93a4f3eaf2fe8ae0541645de349149
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275997"
---
# <a name="list-classes"></a><span data-ttu-id="9212c-104">列出课程</span><span class="sxs-lookup"><span data-stu-id="9212c-104">List classes</span></span>

<span data-ttu-id="9212c-105">检索 class 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9212c-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="9212c-106">请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。</span><span class="sxs-lookup"><span data-stu-id="9212c-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="9212c-107">权限</span><span class="sxs-lookup"><span data-stu-id="9212c-107">Permissions</span></span>
<span data-ttu-id="9212c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9212c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9212c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9212c-110">Permission type</span></span>      | <span data-ttu-id="9212c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9212c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9212c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9212c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9212c-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="9212c-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="9212c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9212c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9212c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9212c-115">Not supported.</span></span>  |
|<span data-ttu-id="9212c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9212c-116">Application</span></span> | <span data-ttu-id="9212c-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9212c-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9212c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9212c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9212c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9212c-119">Optional query parameters</span></span>
<span data-ttu-id="9212c-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9212c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9212c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9212c-121">Request headers</span></span>
| <span data-ttu-id="9212c-122">标头</span><span class="sxs-lookup"><span data-stu-id="9212c-122">Header</span></span>       | <span data-ttu-id="9212c-123">值</span><span class="sxs-lookup"><span data-stu-id="9212c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9212c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9212c-124">Authorization</span></span>  | <span data-ttu-id="9212c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9212c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9212c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9212c-127">Request body</span></span>
<span data-ttu-id="9212c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9212c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9212c-129">响应</span><span class="sxs-lookup"><span data-stu-id="9212c-129">Response</span></span>
<span data-ttu-id="9212c-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="9212c-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9212c-131">示例</span><span class="sxs-lookup"><span data-stu-id="9212c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9212c-132">请求</span><span class="sxs-lookup"><span data-stu-id="9212c-132">Request</span></span>
<span data-ttu-id="9212c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9212c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="9212c-134">响应</span><span class="sxs-lookup"><span data-stu-id="9212c-134">Response</span></span>
<span data-ttu-id="9212c-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9212c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9212c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9212c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9212c-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9212c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9212c-139">C#</span><span class="sxs-lookup"><span data-stu-id="9212c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_classes-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9212c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="9212c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_classes-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9212c-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="9212c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_classes-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationuser-list-classes.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationuser-list-classes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationuser-list-classes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
