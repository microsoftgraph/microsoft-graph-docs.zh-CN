---
title: 获取组
description: 检索Microsoft 365 **educationClass** 对应的组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6439e460bcd1e32780540de4bce3f36d432c75a0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035566"
---
# <a name="get-group"></a><span data-ttu-id="e0be5-103">获取组</span><span class="sxs-lookup"><span data-stu-id="e0be5-103">Get group</span></span>

<span data-ttu-id="e0be5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0be5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0be5-105">检索Microsoft 365 **educationClass** 对应的组。</span><span class="sxs-lookup"><span data-stu-id="e0be5-105">Retrieve the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="e0be5-106">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="e0be5-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="e0be5-107">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="e0be5-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0be5-108">权限</span><span class="sxs-lookup"><span data-stu-id="e0be5-108">Permissions</span></span>
<span data-ttu-id="e0be5-109">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="e0be5-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="e0be5-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0be5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0be5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0be5-111">Permission type</span></span>      | <span data-ttu-id="e0be5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0be5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0be5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0be5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e0be5-114">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0be5-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="e0be5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0be5-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e0be5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0be5-116">Not supported.</span></span>  |
|<span data-ttu-id="e0be5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0be5-117">Application</span></span> | <span data-ttu-id="e0be5-118">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0be5-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e0be5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0be5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="e0be5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0be5-120">Request headers</span></span>
| <span data-ttu-id="e0be5-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0be5-121">Header</span></span>       | <span data-ttu-id="e0be5-122">值</span><span class="sxs-lookup"><span data-stu-id="e0be5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0be5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0be5-123">Authorization</span></span>  | <span data-ttu-id="e0be5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0be5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0be5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0be5-126">Request body</span></span>
<span data-ttu-id="e0be5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0be5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e0be5-128">响应</span><span class="sxs-lookup"><span data-stu-id="e0be5-128">Response</span></span>
<span data-ttu-id="e0be5-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0be5-129">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0be5-130">示例</span><span class="sxs-lookup"><span data-stu-id="e0be5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0be5-131">请求</span><span class="sxs-lookup"><span data-stu-id="e0be5-131">Request</span></span>
<span data-ttu-id="e0be5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0be5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0be5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0be5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
# <a name="c"></a>[<span data-ttu-id="e0be5-134">C#</span><span class="sxs-lookup"><span data-stu-id="e0be5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0be5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0be5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0be5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0be5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0be5-137">Java</span><span class="sxs-lookup"><span data-stu-id="e0be5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0be5-138">响应</span><span class="sxs-lookup"><span data-stu-id="e0be5-138">Response</span></span>
<span data-ttu-id="e0be5-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0be5-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e0be5-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0be5-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
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

