---
title: 获取 educationClass
description: "  组管理员代表课程中的教师。 如果使用的是委派令牌，用户只会看到他们作为成员的课程。"
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1be350f85abc1aab70be667819fdcda433bf720c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36717967"
---
# <a name="get-educationclass"></a><span data-ttu-id="4a852-104">获取 educationClass</span><span class="sxs-lookup"><span data-stu-id="4a852-104">Get educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a852-105">从系统检索课程。</span><span class="sxs-lookup"><span data-stu-id="4a852-105">Retrieve a class from the system.</span></span> <span data-ttu-id="4a852-106">课程是带特殊属性的通用组，向系统表明该组是课程。</span><span class="sxs-lookup"><span data-stu-id="4a852-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="4a852-107">组成员表示学生；组管理员代表课程教师。</span><span class="sxs-lookup"><span data-stu-id="4a852-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="4a852-108">如果使用的是委派令牌，用户只会看到他们作为成员的课程。</span><span class="sxs-lookup"><span data-stu-id="4a852-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a852-109">权限</span><span class="sxs-lookup"><span data-stu-id="4a852-109">Permissions</span></span>
<span data-ttu-id="4a852-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a852-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a852-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a852-112">Permission type</span></span>      | <span data-ttu-id="4a852-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a852-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a852-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a852-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a852-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="4a852-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="4a852-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a852-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4a852-117">不支持</span><span class="sxs-lookup"><span data-stu-id="4a852-117">Not supported</span></span>  |
|<span data-ttu-id="4a852-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a852-118">Application</span></span> | <span data-ttu-id="4a852-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a852-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4a852-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a852-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a852-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a852-121">Optional query parameters</span></span>
<span data-ttu-id="4a852-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a852-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a852-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a852-123">Request headers</span></span>
| <span data-ttu-id="4a852-124">标头</span><span class="sxs-lookup"><span data-stu-id="4a852-124">Header</span></span>       | <span data-ttu-id="4a852-125">值</span><span class="sxs-lookup"><span data-stu-id="4a852-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a852-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a852-126">Authorization</span></span>  | <span data-ttu-id="4a852-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a852-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a852-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a852-129">Request body</span></span>
<span data-ttu-id="4a852-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a852-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4a852-131">响应</span><span class="sxs-lookup"><span data-stu-id="4a852-131">Response</span></span>
<span data-ttu-id="4a852-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a852-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a852-133">示例</span><span class="sxs-lookup"><span data-stu-id="4a852-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a852-134">请求</span><span class="sxs-lookup"><span data-stu-id="4a852-134">Request</span></span>
<span data-ttu-id="4a852-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a852-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4a852-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4a852-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11023
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a852-137">C#</span><span class="sxs-lookup"><span data-stu-id="4a852-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a852-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a852-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a852-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="4a852-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a852-140">响应</span><span class="sxs-lookup"><span data-stu-id="4a852-140">Response</span></span>
<span data-ttu-id="4a852-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4a852-141">The following is an example of the response.</span></span> 

><span data-ttu-id="4a852-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4a852-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
