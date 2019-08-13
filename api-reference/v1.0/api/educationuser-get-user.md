---
title: 获取用户
description: 检索与此 **educationUser** 对应的简单目录 **user**。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8f88f63aa3babcf52aeb08df524a517252715b06
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331217"
---
# <a name="get-user"></a><span data-ttu-id="1bfa3-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="1bfa3-103">Get user</span></span>

<span data-ttu-id="1bfa3-104">检索与此 **educationUser** 对应的简单目录 **user**。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-104">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="1bfa3-105">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="1bfa3-106">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bfa3-107">权限</span><span class="sxs-lookup"><span data-stu-id="1bfa3-107">Permissions</span></span>
<span data-ttu-id="1bfa3-108">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="1bfa3-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bfa3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bfa3-110">Permission type</span></span>      | <span data-ttu-id="1bfa3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bfa3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bfa3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bfa3-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="1bfa3-113">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All 或 User.Read</span><span class="sxs-lookup"><span data-stu-id="1bfa3-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="1bfa3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bfa3-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1bfa3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-115">Not supported.</span></span>  |
|<span data-ttu-id="1bfa3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bfa3-116">Application</span></span> | <span data-ttu-id="1bfa3-117">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bfa3-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="1bfa3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bfa3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="1bfa3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bfa3-119">Request headers</span></span>
| <span data-ttu-id="1bfa3-120">标头</span><span class="sxs-lookup"><span data-stu-id="1bfa3-120">Header</span></span>       | <span data-ttu-id="1bfa3-121">值</span><span class="sxs-lookup"><span data-stu-id="1bfa3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bfa3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bfa3-122">Authorization</span></span>  | <span data-ttu-id="1bfa3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bfa3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bfa3-125">Request body</span></span>
<span data-ttu-id="1bfa3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1bfa3-127">响应</span><span class="sxs-lookup"><span data-stu-id="1bfa3-127">Response</span></span>
<span data-ttu-id="1bfa3-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bfa3-129">示例</span><span class="sxs-lookup"><span data-stu-id="1bfa3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bfa3-130">请求</span><span class="sxs-lookup"><span data-stu-id="1bfa3-130">Request</span></span>
<span data-ttu-id="1bfa3-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1bfa3-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1bfa3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/user
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bfa3-133">C#</span><span class="sxs-lookup"><span data-stu-id="1bfa3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bfa3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bfa3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bfa3-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="1bfa3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1bfa3-136">Java</span><span class="sxs-lookup"><span data-stu-id="1bfa3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1bfa3-137">响应</span><span class="sxs-lookup"><span data-stu-id="1bfa3-137">Response</span></span>
<span data-ttu-id="1bfa3-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-138">The following is an example of the response.</span></span> 

><span data-ttu-id="1bfa3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1bfa3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
