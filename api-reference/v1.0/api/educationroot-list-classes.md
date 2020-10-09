---
title: 列出课程
description: '检索所有 class 对象的列表。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8f37a8e1b74999265e54afe6008d9b4275753a64
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401612"
---
# <a name="list-classes"></a><span data-ttu-id="73d20-103">列出课程</span><span class="sxs-lookup"><span data-stu-id="73d20-103">List classes</span></span>

<span data-ttu-id="73d20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d20-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73d20-105">检索所有 class 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="73d20-105">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="73d20-106">权限</span><span class="sxs-lookup"><span data-stu-id="73d20-106">Permissions</span></span>
<span data-ttu-id="73d20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73d20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d20-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73d20-109">Permission type</span></span>      | <span data-ttu-id="73d20-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73d20-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73d20-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73d20-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73d20-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="73d20-112">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="73d20-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73d20-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="73d20-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73d20-114">Not supported.</span></span>  |
|<span data-ttu-id="73d20-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73d20-115">Application</span></span> | <span data-ttu-id="73d20-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d20-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="73d20-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73d20-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73d20-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73d20-118">Optional query parameters</span></span>
<span data-ttu-id="73d20-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73d20-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73d20-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73d20-120">Request headers</span></span>
| <span data-ttu-id="73d20-121">标头</span><span class="sxs-lookup"><span data-stu-id="73d20-121">Header</span></span>       | <span data-ttu-id="73d20-122">值</span><span class="sxs-lookup"><span data-stu-id="73d20-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73d20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d20-123">Authorization</span></span>  | <span data-ttu-id="73d20-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73d20-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="73d20-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73d20-126">Request body</span></span>
<span data-ttu-id="73d20-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73d20-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="73d20-128">响应</span><span class="sxs-lookup"><span data-stu-id="73d20-128">Response</span></span>
<span data-ttu-id="73d20-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="73d20-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73d20-130">示例</span><span class="sxs-lookup"><span data-stu-id="73d20-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73d20-131">请求</span><span class="sxs-lookup"><span data-stu-id="73d20-131">Request</span></span>
<span data-ttu-id="73d20-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73d20-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73d20-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="73d20-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes
```
# <a name="c"></a>[<span data-ttu-id="73d20-134">C#</span><span class="sxs-lookup"><span data-stu-id="73d20-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73d20-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73d20-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73d20-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73d20-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73d20-137">Java</span><span class="sxs-lookup"><span data-stu-id="73d20-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="73d20-138">响应</span><span class="sxs-lookup"><span data-stu-id="73d20-138">Response</span></span>
<span data-ttu-id="73d20-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73d20-139">The following is an example of the response.</span></span> 

><span data-ttu-id="73d20-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73d20-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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