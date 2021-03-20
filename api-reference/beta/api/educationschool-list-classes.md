---
title: 列出 educationClasses
description: 检索学校所拥有的课程列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5c02a27b1177e85cc00e96005faa5eb4ee3fc4d8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951332"
---
# <a name="list-educationclasses"></a><span data-ttu-id="440c0-103">列出 educationClasses</span><span class="sxs-lookup"><span data-stu-id="440c0-103">List educationClasses</span></span>

<span data-ttu-id="440c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="440c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="440c0-105">检索学校所拥有的课程列表。</span><span class="sxs-lookup"><span data-stu-id="440c0-105">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="440c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="440c0-106">Permissions</span></span>
<span data-ttu-id="440c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="440c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="440c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="440c0-109">Permission type</span></span>      | <span data-ttu-id="440c0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="440c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="440c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="440c0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="440c0-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="440c0-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="440c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="440c0-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="440c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="440c0-114">Not supported.</span></span>  |
|<span data-ttu-id="440c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="440c0-115">Application</span></span> | <span data-ttu-id="440c0-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="440c0-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="440c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="440c0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="440c0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="440c0-118">Optional query parameters</span></span>
<span data-ttu-id="440c0-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="440c0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="440c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="440c0-120">Request headers</span></span>
| <span data-ttu-id="440c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="440c0-121">Header</span></span>       | <span data-ttu-id="440c0-122">值</span><span class="sxs-lookup"><span data-stu-id="440c0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="440c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="440c0-123">Authorization</span></span>  | <span data-ttu-id="440c0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="440c0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="440c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="440c0-126">Request body</span></span>
<span data-ttu-id="440c0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="440c0-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="440c0-128">响应</span><span class="sxs-lookup"><span data-stu-id="440c0-128">Response</span></span>
<span data-ttu-id="440c0-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="440c0-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="440c0-130">示例</span><span class="sxs-lookup"><span data-stu-id="440c0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="440c0-131">请求</span><span class="sxs-lookup"><span data-stu-id="440c0-131">Request</span></span>
<span data-ttu-id="440c0-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="440c0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="440c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="440c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
# <a name="c"></a>[<span data-ttu-id="440c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="440c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="440c0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="440c0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="440c0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="440c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="440c0-137">Java</span><span class="sxs-lookup"><span data-stu-id="440c0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="440c0-138">响应</span><span class="sxs-lookup"><span data-stu-id="440c0-138">Response</span></span>
<span data-ttu-id="440c0-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="440c0-139">The following is an example of the response.</span></span> 

><span data-ttu-id="440c0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="440c0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
