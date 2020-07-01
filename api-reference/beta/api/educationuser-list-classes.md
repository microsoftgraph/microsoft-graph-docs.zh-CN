---
title: 列出课程
description: '检索 class 对象的列表。 请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e00aa154ece87b8e1488559d98f98b88c8952581
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006768"
---
# <a name="list-classes"></a><span data-ttu-id="a4a61-104">列出课程</span><span class="sxs-lookup"><span data-stu-id="a4a61-104">List classes</span></span>

<span data-ttu-id="a4a61-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4a61-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4a61-106">检索 educationClass 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="a4a61-106">Retrieve a collection of educationClass resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4a61-107">权限</span><span class="sxs-lookup"><span data-stu-id="a4a61-107">Permissions</span></span>

<span data-ttu-id="a4a61-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a4a61-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a4a61-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4a61-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4a61-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4a61-110">Permission type</span></span>                        | <span data-ttu-id="a4a61-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4a61-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a4a61-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4a61-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4a61-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a4a61-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a4a61-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4a61-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4a61-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4a61-115">Not supported.</span></span>                              |
| <span data-ttu-id="a4a61-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4a61-116">Application</span></span>                            | <span data-ttu-id="a4a61-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a61-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a4a61-118">使用委派权限时，将仅返回身份验证用户为其成员的 educationClass 资源。</span><span class="sxs-lookup"><span data-stu-id="a4a61-118">When delegated permissions are used, only educationClass resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="a4a61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4a61-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/classes
GET /education/users/{id}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4a61-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4a61-120">Optional query parameters</span></span>

<span data-ttu-id="a4a61-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4a61-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4a61-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4a61-122">Request headers</span></span>

| <span data-ttu-id="a4a61-123">标头</span><span class="sxs-lookup"><span data-stu-id="a4a61-123">Header</span></span>        | <span data-ttu-id="a4a61-124">值</span><span class="sxs-lookup"><span data-stu-id="a4a61-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a4a61-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a61-125">Authorization</span></span> | <span data-ttu-id="a4a61-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a4a61-126">Bearer {token}.</span></span> <span data-ttu-id="a4a61-127">Required.</span><span class="sxs-lookup"><span data-stu-id="a4a61-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4a61-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4a61-128">Request body</span></span>

<span data-ttu-id="a4a61-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4a61-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4a61-130">响应</span><span class="sxs-lookup"><span data-stu-id="a4a61-130">Response</span></span>

<span data-ttu-id="a4a61-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a4a61-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a61-132">示例</span><span class="sxs-lookup"><span data-stu-id="a4a61-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a4a61-133">请求</span><span class="sxs-lookup"><span data-stu-id="a4a61-133">Request</span></span>

<span data-ttu-id="a4a61-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a4a61-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4a61-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4a61-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/classes
```

# <a name="c"></a>[<span data-ttu-id="a4a61-136">C#</span><span class="sxs-lookup"><span data-stu-id="a4a61-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4a61-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4a61-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4a61-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4a61-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a4a61-139">响应</span><span class="sxs-lookup"><span data-stu-id="a4a61-139">Response</span></span>

<span data-ttu-id="a4a61-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a4a61-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a4a61-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="a4a61-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a4a61-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a4a61-142">All the properties will be returned from an actual call.</span></span>

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
