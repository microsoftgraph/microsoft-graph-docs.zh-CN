---
title: 列出 educationUser 的课程
description: '检索 class 对象的列表。 请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6530d0fd060381a0e2f3281f23cad60f98b2dfef
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475428"
---
# <a name="list-classes-of-an-educationuser"></a><span data-ttu-id="07d14-104">列出 educationUser 的课程</span><span class="sxs-lookup"><span data-stu-id="07d14-104">List classes of an educationUser</span></span>

<span data-ttu-id="07d14-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07d14-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07d14-106">获取 [educationUser](../resources/educationclass.md) 是其中一个成员的 [educationClass](../resources/educationuser.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="07d14-106">Get the [educationClass](../resources/educationclass.md) resources an [educationUser](../resources/educationuser.md) is a member of.</span></span>

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="07d14-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="07d14-107">Permissions</span></span>
<span data-ttu-id="07d14-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07d14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="07d14-110">Permission type</span></span>      | <span data-ttu-id="07d14-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07d14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07d14-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="07d14-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="07d14-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="07d14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07d14-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="07d14-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="07d14-115">Not supported.</span></span>  |
|<span data-ttu-id="07d14-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="07d14-116">Application</span></span> | <span data-ttu-id="07d14-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d14-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

> [!NOTE]
> <span data-ttu-id="07d14-118">请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。</span><span class="sxs-lookup"><span data-stu-id="07d14-118">Note that if the delegated token is used, members can only see information about their own classes.</span></span>

## <a name="http-request"></a><span data-ttu-id="07d14-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07d14-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07d14-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="07d14-120">Optional query parameters</span></span>
<span data-ttu-id="07d14-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="07d14-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07d14-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="07d14-122">Request headers</span></span>
| <span data-ttu-id="07d14-123">标头</span><span class="sxs-lookup"><span data-stu-id="07d14-123">Header</span></span>       | <span data-ttu-id="07d14-124">值</span><span class="sxs-lookup"><span data-stu-id="07d14-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07d14-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07d14-125">Authorization</span></span>  | <span data-ttu-id="07d14-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07d14-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07d14-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="07d14-128">Request body</span></span>
<span data-ttu-id="07d14-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="07d14-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="07d14-130">响应</span><span class="sxs-lookup"><span data-stu-id="07d14-130">Response</span></span>
<span data-ttu-id="07d14-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="07d14-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07d14-132">示例</span><span class="sxs-lookup"><span data-stu-id="07d14-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07d14-133">请求</span><span class="sxs-lookup"><span data-stu-id="07d14-133">Request</span></span>
<span data-ttu-id="07d14-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07d14-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07d14-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="07d14-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/classes
```
# <a name="c"></a>[<span data-ttu-id="07d14-136">C#</span><span class="sxs-lookup"><span data-stu-id="07d14-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07d14-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07d14-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07d14-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07d14-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07d14-139">Java</span><span class="sxs-lookup"><span data-stu-id="07d14-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07d14-140">响应</span><span class="sxs-lookup"><span data-stu-id="07d14-140">Response</span></span>
<span data-ttu-id="07d14-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07d14-141">The following is an example of the response.</span></span> 

><span data-ttu-id="07d14-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="07d14-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
