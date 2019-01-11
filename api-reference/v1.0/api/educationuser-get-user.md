---
title: 获取用户
description: 检索与此 **educationUser** 对应的简单目录 **user**。
localization_priority: Normal
ms.openlocfilehash: ae2cdfa5aed7dadf7e61c275e65c646196f4667d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836853"
---
# <a name="get-user"></a><span data-ttu-id="edeee-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="edeee-103">Get user</span></span>

<span data-ttu-id="edeee-104">检索与此 **educationUser** 对应的简单目录 **user**。</span><span class="sxs-lookup"><span data-stu-id="edeee-104">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="edeee-105">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="edeee-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="edeee-106">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="edeee-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="edeee-107">权限</span><span class="sxs-lookup"><span data-stu-id="edeee-107">Permissions</span></span>
<span data-ttu-id="edeee-108">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="edeee-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="edeee-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edeee-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edeee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="edeee-110">Permission type</span></span>      | <span data-ttu-id="edeee-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edeee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edeee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edeee-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="edeee-113">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All 或 User.Read</span><span class="sxs-lookup"><span data-stu-id="edeee-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="edeee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edeee-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="edeee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="edeee-115">Not supported.</span></span>  |
|<span data-ttu-id="edeee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="edeee-116">Application</span></span> | <span data-ttu-id="edeee-117">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="edeee-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="edeee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edeee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="edeee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="edeee-119">Request headers</span></span>
| <span data-ttu-id="edeee-120">标头</span><span class="sxs-lookup"><span data-stu-id="edeee-120">Header</span></span>       | <span data-ttu-id="edeee-121">值</span><span class="sxs-lookup"><span data-stu-id="edeee-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="edeee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="edeee-122">Authorization</span></span>  | <span data-ttu-id="edeee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edeee-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="edeee-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="edeee-125">Request body</span></span>
<span data-ttu-id="edeee-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="edeee-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="edeee-127">响应</span><span class="sxs-lookup"><span data-stu-id="edeee-127">Response</span></span>
<span data-ttu-id="edeee-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edeee-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="edeee-129">示例</span><span class="sxs-lookup"><span data-stu-id="edeee-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edeee-130">请求</span><span class="sxs-lookup"><span data-stu-id="edeee-130">Request</span></span>
<span data-ttu-id="edeee-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="edeee-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/user
```
##### <a name="response"></a><span data-ttu-id="edeee-132">响应</span><span class="sxs-lookup"><span data-stu-id="edeee-132">Response</span></span>
<span data-ttu-id="edeee-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="edeee-133">The following is an example of the response.</span></span> 

><span data-ttu-id="edeee-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="edeee-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
