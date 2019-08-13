---
title: 获取组
description: 检索与此 **educationClass** 对应的 Office 365 **group**。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dd0cc9f78a9686354b560a0296c545d19a3c0dc3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370457"
---
# <a name="get-group"></a><span data-ttu-id="784e7-103">获取组</span><span class="sxs-lookup"><span data-stu-id="784e7-103">Get group</span></span>

<span data-ttu-id="784e7-104">检索与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="784e7-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="784e7-105">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="784e7-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="784e7-106">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="784e7-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="784e7-107">权限</span><span class="sxs-lookup"><span data-stu-id="784e7-107">Permissions</span></span>
<span data-ttu-id="784e7-108">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="784e7-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="784e7-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="784e7-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="784e7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="784e7-110">Permission type</span></span>      | <span data-ttu-id="784e7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="784e7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="784e7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="784e7-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="784e7-113">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="784e7-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="784e7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="784e7-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="784e7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="784e7-115">Not supported.</span></span>  |
|<span data-ttu-id="784e7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="784e7-116">Application</span></span> | <span data-ttu-id="784e7-117">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="784e7-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="784e7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="784e7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="784e7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="784e7-119">Request headers</span></span>
| <span data-ttu-id="784e7-120">标头</span><span class="sxs-lookup"><span data-stu-id="784e7-120">Header</span></span>       | <span data-ttu-id="784e7-121">值</span><span class="sxs-lookup"><span data-stu-id="784e7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="784e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="784e7-122">Authorization</span></span>  | <span data-ttu-id="784e7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="784e7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="784e7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="784e7-125">Request body</span></span>
<span data-ttu-id="784e7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="784e7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="784e7-127">响应</span><span class="sxs-lookup"><span data-stu-id="784e7-127">Response</span></span>
<span data-ttu-id="784e7-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="784e7-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="784e7-129">示例</span><span class="sxs-lookup"><span data-stu-id="784e7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="784e7-130">请求</span><span class="sxs-lookup"><span data-stu-id="784e7-130">Request</span></span>
<span data-ttu-id="784e7-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="784e7-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="784e7-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="784e7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="784e7-133">C#</span><span class="sxs-lookup"><span data-stu-id="784e7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="784e7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="784e7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="784e7-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="784e7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="784e7-136">Java</span><span class="sxs-lookup"><span data-stu-id="784e7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="784e7-137">响应</span><span class="sxs-lookup"><span data-stu-id="784e7-137">Response</span></span>
<span data-ttu-id="784e7-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="784e7-138">The following is an example of the response.</span></span> 

><span data-ttu-id="784e7-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="784e7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
