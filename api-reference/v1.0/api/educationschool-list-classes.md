---
title: 列出 educationSchool 的班级
description: 检索学校所拥有的课程列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cbd644e5994f8039a29c16f0463445d92500a865
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232030"
---
# <a name="list-classes-of-an-educationschool"></a><span data-ttu-id="6f72a-103">列出 educationSchool 的班级</span><span class="sxs-lookup"><span data-stu-id="6f72a-103">List classes of an educationSchool</span></span>

<span data-ttu-id="6f72a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f72a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f72a-105">获取[educationSchool](../resources/educationschool.md)所拥有的[educationClass](../resources/educationclass.md)资源。</span><span class="sxs-lookup"><span data-stu-id="6f72a-105">Get the [educationClass](../resources/educationclass.md) resources owned by an [educationSchool](../resources/educationschool.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f72a-106">权限</span><span class="sxs-lookup"><span data-stu-id="6f72a-106">Permissions</span></span>

<span data-ttu-id="6f72a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f72a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f72a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f72a-109">Permission type</span></span>                        | <span data-ttu-id="6f72a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f72a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6f72a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f72a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f72a-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="6f72a-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="6f72a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f72a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f72a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f72a-114">Not supported.</span></span>                              |
| <span data-ttu-id="6f72a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f72a-115">Application</span></span>                            | <span data-ttu-id="6f72a-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f72a-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f72a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f72a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/{educationSchoolId}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f72a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6f72a-118">Optional query parameters</span></span>

<span data-ttu-id="6f72a-119">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="6f72a-119">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="6f72a-120">您还可以使用 和 `$filter` `$count` `$search` 查询参数来限制响应。</span><span class="sxs-lookup"><span data-stu-id="6f72a-120">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span>

<span data-ttu-id="6f72a-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="6f72a-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6f72a-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="6f72a-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="6f72a-123">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6f72a-123">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f72a-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f72a-124">Request headers</span></span>
| <span data-ttu-id="6f72a-125">标头</span><span class="sxs-lookup"><span data-stu-id="6f72a-125">Header</span></span>       | <span data-ttu-id="6f72a-126">值</span><span class="sxs-lookup"><span data-stu-id="6f72a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6f72a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f72a-127">Authorization</span></span>  | <span data-ttu-id="6f72a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f72a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f72a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f72a-130">Request body</span></span>
<span data-ttu-id="6f72a-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f72a-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6f72a-132">响应</span><span class="sxs-lookup"><span data-stu-id="6f72a-132">Response</span></span>
<span data-ttu-id="6f72a-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="6f72a-133">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f72a-134">示例</span><span class="sxs-lookup"><span data-stu-id="6f72a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f72a-135">请求</span><span class="sxs-lookup"><span data-stu-id="6f72a-135">Request</span></span>
<span data-ttu-id="6f72a-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f72a-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f72a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f72a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
# <a name="c"></a>[<span data-ttu-id="6f72a-138">C#</span><span class="sxs-lookup"><span data-stu-id="6f72a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f72a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f72a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f72a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f72a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f72a-141">Java</span><span class="sxs-lookup"><span data-stu-id="6f72a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6f72a-142">响应</span><span class="sxs-lookup"><span data-stu-id="6f72a-142">Response</span></span>
<span data-ttu-id="6f72a-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f72a-143">The following is an example of the response.</span></span> 

><span data-ttu-id="6f72a-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6f72a-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
