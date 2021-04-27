---
title: 获取 educationClass
description: "  组管理员表示班级中的教师。 如果使用的是委派令牌，用户只会看到他们作为成员的课程。"
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f5d6dba45d267b85e8edf6d2831338c7aa79084c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044009"
---
# <a name="get-educationclass"></a><span data-ttu-id="30499-104">获取 educationClass</span><span class="sxs-lookup"><span data-stu-id="30499-104">Get educationClass</span></span>

<span data-ttu-id="30499-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30499-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30499-106">从系统检索课程。</span><span class="sxs-lookup"><span data-stu-id="30499-106">Retrieve a class from the system.</span></span> <span data-ttu-id="30499-107">课程是带特殊属性的通用组，向系统表明该组是课程。</span><span class="sxs-lookup"><span data-stu-id="30499-107">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="30499-108">组成员表示学生；组管理员代表课程教师。</span><span class="sxs-lookup"><span data-stu-id="30499-108">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="30499-109">如果使用的是委派令牌，用户只会看到他们作为成员的课程。</span><span class="sxs-lookup"><span data-stu-id="30499-109">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="30499-110">权限</span><span class="sxs-lookup"><span data-stu-id="30499-110">Permissions</span></span>
<span data-ttu-id="30499-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30499-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30499-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="30499-113">Permission type</span></span>      | <span data-ttu-id="30499-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30499-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30499-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30499-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="30499-116">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="30499-116">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="30499-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30499-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="30499-118">不支持</span><span class="sxs-lookup"><span data-stu-id="30499-118">Not supported</span></span>  |
|<span data-ttu-id="30499-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="30499-119">Application</span></span> | <span data-ttu-id="30499-120">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30499-120">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="30499-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30499-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30499-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="30499-122">Optional query parameters</span></span>
<span data-ttu-id="30499-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="30499-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30499-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="30499-124">Request headers</span></span>
| <span data-ttu-id="30499-125">标头</span><span class="sxs-lookup"><span data-stu-id="30499-125">Header</span></span>       | <span data-ttu-id="30499-126">值</span><span class="sxs-lookup"><span data-stu-id="30499-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="30499-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="30499-127">Authorization</span></span>  | <span data-ttu-id="30499-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30499-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30499-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="30499-130">Request body</span></span>
<span data-ttu-id="30499-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30499-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="30499-132">响应</span><span class="sxs-lookup"><span data-stu-id="30499-132">Response</span></span>
<span data-ttu-id="30499-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30499-133">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30499-134">示例</span><span class="sxs-lookup"><span data-stu-id="30499-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30499-135">请求</span><span class="sxs-lookup"><span data-stu-id="30499-135">Request</span></span>
<span data-ttu-id="30499-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30499-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="30499-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="30499-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11023
```
# <a name="c"></a>[<span data-ttu-id="30499-138">C#</span><span class="sxs-lookup"><span data-stu-id="30499-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30499-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30499-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30499-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30499-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30499-141">Java</span><span class="sxs-lookup"><span data-stu-id="30499-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30499-142">响应</span><span class="sxs-lookup"><span data-stu-id="30499-142">Response</span></span>
<span data-ttu-id="30499-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="30499-143">The following is an example of the response.</span></span> 

><span data-ttu-id="30499-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="30499-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
