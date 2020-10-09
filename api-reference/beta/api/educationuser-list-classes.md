---
title: 列出课程
description: '检索 class 对象的列表。 请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 55c55ebfd619e8dc6a1fd49b621578ae56b82360
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403288"
---
# <a name="list-classes"></a><span data-ttu-id="a9420-104">列出课程</span><span class="sxs-lookup"><span data-stu-id="a9420-104">List classes</span></span>

<span data-ttu-id="a9420-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9420-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9420-106">检索 educationClass 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="a9420-106">Retrieve a collection of educationClass resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9420-107">权限</span><span class="sxs-lookup"><span data-stu-id="a9420-107">Permissions</span></span>

<span data-ttu-id="a9420-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9420-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9420-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9420-110">Permission type</span></span>                        | <span data-ttu-id="a9420-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9420-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a9420-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9420-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9420-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a9420-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a9420-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9420-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9420-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9420-115">Not supported.</span></span>                              |
| <span data-ttu-id="a9420-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9420-116">Application</span></span>                            | <span data-ttu-id="a9420-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9420-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a9420-118">使用委派权限时，将仅返回身份验证用户为其成员的 educationClass 资源。</span><span class="sxs-lookup"><span data-stu-id="a9420-118">When delegated permissions are used, only educationClass resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="a9420-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9420-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/classes
GET /education/users/{id}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9420-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a9420-120">Optional query parameters</span></span>

<span data-ttu-id="a9420-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a9420-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9420-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9420-122">Request headers</span></span>

| <span data-ttu-id="a9420-123">标头</span><span class="sxs-lookup"><span data-stu-id="a9420-123">Header</span></span>        | <span data-ttu-id="a9420-124">值</span><span class="sxs-lookup"><span data-stu-id="a9420-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a9420-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9420-125">Authorization</span></span> | <span data-ttu-id="a9420-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9420-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9420-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9420-128">Request body</span></span>

<span data-ttu-id="a9420-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9420-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9420-130">响应</span><span class="sxs-lookup"><span data-stu-id="a9420-130">Response</span></span>

<span data-ttu-id="a9420-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a9420-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9420-132">示例</span><span class="sxs-lookup"><span data-stu-id="a9420-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a9420-133">请求</span><span class="sxs-lookup"><span data-stu-id="a9420-133">Request</span></span>

<span data-ttu-id="a9420-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a9420-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9420-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9420-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/classes
```

# <a name="c"></a>[<span data-ttu-id="a9420-136">C#</span><span class="sxs-lookup"><span data-stu-id="a9420-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9420-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9420-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9420-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9420-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9420-139">响应</span><span class="sxs-lookup"><span data-stu-id="a9420-139">Response</span></span>

<span data-ttu-id="a9420-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a9420-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a9420-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a9420-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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