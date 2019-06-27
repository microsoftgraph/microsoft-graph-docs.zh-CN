---
title: 获取 educationClass
description: "  组管理员代表课程中的教师。 如果使用的是委派令牌，用户只会看到他们作为成员的课程。"
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 242e03802d4fdcddb6b00fc5dff3878a1d5721b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259813"
---
# <a name="get-educationclass"></a><span data-ttu-id="ce369-104">获取 educationClass</span><span class="sxs-lookup"><span data-stu-id="ce369-104">Get educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce369-105">从系统检索课程。</span><span class="sxs-lookup"><span data-stu-id="ce369-105">Retrieve a class from the system.</span></span> <span data-ttu-id="ce369-106">课程是带特殊属性的通用组，向系统表明该组是课程。</span><span class="sxs-lookup"><span data-stu-id="ce369-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="ce369-107">组成员表示学生；组管理员代表课程教师。</span><span class="sxs-lookup"><span data-stu-id="ce369-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="ce369-108">如果使用的是委派令牌，用户只会看到他们作为成员的课程。</span><span class="sxs-lookup"><span data-stu-id="ce369-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce369-109">权限</span><span class="sxs-lookup"><span data-stu-id="ce369-109">Permissions</span></span>
<span data-ttu-id="ce369-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce369-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce369-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce369-112">Permission type</span></span>      | <span data-ttu-id="ce369-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce369-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce369-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce369-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="ce369-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ce369-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="ce369-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce369-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ce369-117">不支持</span><span class="sxs-lookup"><span data-stu-id="ce369-117">Not supported</span></span>  |
|<span data-ttu-id="ce369-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce369-118">Application</span></span> | <span data-ttu-id="ce369-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce369-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ce369-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce369-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce369-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce369-121">Optional query parameters</span></span>
<span data-ttu-id="ce369-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ce369-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce369-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce369-123">Request headers</span></span>
| <span data-ttu-id="ce369-124">标头</span><span class="sxs-lookup"><span data-stu-id="ce369-124">Header</span></span>       | <span data-ttu-id="ce369-125">值</span><span class="sxs-lookup"><span data-stu-id="ce369-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce369-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce369-126">Authorization</span></span>  | <span data-ttu-id="ce369-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce369-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce369-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce369-129">Request body</span></span>
<span data-ttu-id="ce369-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce369-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ce369-131">响应</span><span class="sxs-lookup"><span data-stu-id="ce369-131">Response</span></span>
<span data-ttu-id="ce369-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce369-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce369-133">示例</span><span class="sxs-lookup"><span data-stu-id="ce369-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce369-134">请求</span><span class="sxs-lookup"><span data-stu-id="ce369-134">Request</span></span>
<span data-ttu-id="ce369-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce369-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023
```
##### <a name="response"></a><span data-ttu-id="ce369-136">响应</span><span class="sxs-lookup"><span data-stu-id="ce369-136">Response</span></span>
<span data-ttu-id="ce369-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce369-137">The following is an example of the response.</span></span> 

><span data-ttu-id="ce369-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ce369-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce369-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ce369-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce369-141">C#</span><span class="sxs-lookup"><span data-stu-id="ce369-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationclass-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce369-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce369-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationclass-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce369-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="ce369-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_educationclass-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationclass-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationclass-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationclass-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
