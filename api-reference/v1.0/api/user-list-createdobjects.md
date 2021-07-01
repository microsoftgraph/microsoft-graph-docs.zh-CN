---
title: List createdObjects
description: 获取由用户创建的 directory 对象列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d615b23fb422c8ff4007eaa7a1324ce76fc4f474
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207012"
---
# <a name="list-createdobjects"></a><span data-ttu-id="e58a8-103">List createdObjects</span><span class="sxs-lookup"><span data-stu-id="e58a8-103">List createdObjects</span></span>

<span data-ttu-id="e58a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e58a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e58a8-105">获取由用户创建的 directory 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e58a8-105">Get a list of directory objects that were created by the user.</span></span> <span data-ttu-id="e58a8-106">此 API 仅返回那些由没有任何管理员角色的用户创建的目录对象;否则，它将返回一个空对象。</span><span class="sxs-lookup"><span data-stu-id="e58a8-106">This API returns only those directory objects that were created by a user who isn't in any administrator role; otherwise, it returns an empty object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e58a8-107">权限</span><span class="sxs-lookup"><span data-stu-id="e58a8-107">Permissions</span></span>
<span data-ttu-id="e58a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e58a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e58a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e58a8-110">Permission type</span></span>      | <span data-ttu-id="e58a8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e58a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e58a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e58a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e58a8-113">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e58a8-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e58a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e58a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e58a8-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e58a8-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e58a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e58a8-116">Application</span></span> | <span data-ttu-id="e58a8-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e58a8-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e58a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e58a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
GET /me/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e58a8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e58a8-119">Optional query parameters</span></span>
<span data-ttu-id="e58a8-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e58a8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e58a8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e58a8-121">Request headers</span></span>
| <span data-ttu-id="e58a8-122">标头</span><span class="sxs-lookup"><span data-stu-id="e58a8-122">Header</span></span>       | <span data-ttu-id="e58a8-123">值</span><span class="sxs-lookup"><span data-stu-id="e58a8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e58a8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e58a8-124">Authorization</span></span>  | <span data-ttu-id="e58a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e58a8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e58a8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e58a8-127">Content-Type</span></span>  | <span data-ttu-id="e58a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e58a8-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e58a8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e58a8-129">Request body</span></span>
<span data-ttu-id="e58a8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e58a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e58a8-131">响应</span><span class="sxs-lookup"><span data-stu-id="e58a8-131">Response</span></span>

<span data-ttu-id="e58a8-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e58a8-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e58a8-133">示例</span><span class="sxs-lookup"><span data-stu-id="e58a8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e58a8-134">请求</span><span class="sxs-lookup"><span data-stu-id="e58a8-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e58a8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e58a8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="e58a8-136">C#</span><span class="sxs-lookup"><span data-stu-id="e58a8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e58a8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e58a8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e58a8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e58a8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e58a8-139">Java</span><span class="sxs-lookup"><span data-stu-id="e58a8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e58a8-140">响应</span><span class="sxs-lookup"><span data-stu-id="e58a8-140">Response</span></span>
<span data-ttu-id="e58a8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e58a8-141">The following is an example of the response.</span></span> <span data-ttu-id="e58a8-142">在响应中，用户创建了Microsoft 365组、应用程序及其服务主体。</span><span class="sxs-lookup"><span data-stu-id="e58a8-142">From the response, the user created a Microsoft 365 group, an application, and it's service principal.</span></span>

><span data-ttu-id="e58a8-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e58a8-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "92f3d47b-86cc-4b90-953e-8ec7f83ef45f",
      "displayName": "Contoso volunteer roster",
      "groupTypes": [
        "Unified"
      ],
      "mail": "volunteers@contoso.com",
      "mailEnabled": true,
      "mailNickname": "volunteers"
    },
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "5847962e-c746-4707-a657-f80b5b71f429",
      "appId": "254e989a-1b8c-4f8c-84e8-9dea78e9d283",
      "displayName": "ConVol",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    },
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "ea6a54da-62be-4cdc-9860-3ed68a43d8f6",
      "accountEnabled": true,
      "appDisplayName": "ConVol",
      "appDescription": null,
      "appId": "254e989a-1b8c-4f8c-84e8-9dea78e9d283",
      "displayName": "ConVol",
      "servicePrincipalNames": [
        "254e989a-1b8c-4f8c-84e8-9dea78e9d283"
      ],
      "servicePrincipalType": "Application",
      "signInAudience": "AzureADMyOrg",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
