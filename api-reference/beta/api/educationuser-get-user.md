---
title: 获取用户
description: 检索与此 **educationUser** 对应的简单目录 **user**。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ef2337c17cbed1ff397bb4ff5e49c04bd0e4685c
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006749"
---
# <a name="get-user"></a><span data-ttu-id="7a2ff-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="7a2ff-103">Get user</span></span>

<span data-ttu-id="7a2ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a2ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a2ff-105">检索与此 **educationUser** 对应的简单目录 **user**。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-105">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

> [!NOTE]
> <span data-ttu-id="7a2ff-106">如果使用委派的令牌，则成员只能查看有关其自己的帐户的信息。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-106">If the delegated token is used, members can only see information about their own account.</span></span> <span data-ttu-id="7a2ff-107">在这种情况下，使用 `beta/education/me/users` 资源。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-107">Use the `beta/education/me/users` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a2ff-108">权限</span><span class="sxs-lookup"><span data-stu-id="7a2ff-108">Permissions</span></span>

<span data-ttu-id="7a2ff-109">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="7a2ff-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a2ff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a2ff-111">Permission type</span></span>                        | <span data-ttu-id="7a2ff-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a2ff-112">Permissions (from least to most privileged)</span></span>                                                               |
| :------------------------------------- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7a2ff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a2ff-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a2ff-114">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All 或 User.Read</span><span class="sxs-lookup"><span data-stu-id="7a2ff-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span> |
| <span data-ttu-id="7a2ff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a2ff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a2ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-116">Not supported.</span></span>                                                                                            |
| <span data-ttu-id="7a2ff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a2ff-117">Application</span></span>                            | <span data-ttu-id="7a2ff-118">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a2ff-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="7a2ff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a2ff-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/user
GET /education/users/{id}/user
```

## <a name="request-headers"></a><span data-ttu-id="7a2ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a2ff-120">Request headers</span></span>

| <span data-ttu-id="7a2ff-121">标头</span><span class="sxs-lookup"><span data-stu-id="7a2ff-121">Header</span></span>        | <span data-ttu-id="7a2ff-122">值</span><span class="sxs-lookup"><span data-stu-id="7a2ff-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7a2ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a2ff-123">Authorization</span></span> | <span data-ttu-id="7a2ff-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a2ff-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a2ff-126">Request body</span></span>

<span data-ttu-id="7a2ff-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a2ff-128">响应</span><span class="sxs-lookup"><span data-stu-id="7a2ff-128">Response</span></span>

<span data-ttu-id="7a2ff-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-129">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a2ff-130">示例</span><span class="sxs-lookup"><span data-stu-id="7a2ff-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7a2ff-131">请求</span><span class="sxs-lookup"><span data-stu-id="7a2ff-131">Request</span></span>

<span data-ttu-id="7a2ff-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a2ff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a2ff-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/user
```

# <a name="c"></a>[<span data-ttu-id="7a2ff-134">C#</span><span class="sxs-lookup"><span data-stu-id="7a2ff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a2ff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a2ff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a2ff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a2ff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a2ff-137">响应</span><span class="sxs-lookup"><span data-stu-id="7a2ff-137">Response</span></span>

<span data-ttu-id="7a2ff-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-138">The following is an example of the response.</span></span>

> <span data-ttu-id="7a2ff-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7a2ff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
