---
title: List contactFolders
description: 获取登录用户的邮箱中的所有联系人文件夹。
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f59362e627dc4b23be75f70b84e9824dd7f9ce16
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459506"
---
# <a name="list-contactfolders"></a><span data-ttu-id="12cf8-103">List contactFolders</span><span class="sxs-lookup"><span data-stu-id="12cf8-103">List contactFolders</span></span>

<span data-ttu-id="12cf8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12cf8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12cf8-105">获取登录用户的邮箱中的所有联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="12cf8-105">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="12cf8-106">权限</span><span class="sxs-lookup"><span data-stu-id="12cf8-106">Permissions</span></span>
<span data-ttu-id="12cf8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12cf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12cf8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12cf8-109">Permission type</span></span>      | <span data-ttu-id="12cf8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12cf8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12cf8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12cf8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12cf8-112">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12cf8-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="12cf8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12cf8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12cf8-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12cf8-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="12cf8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="12cf8-115">Application</span></span> | <span data-ttu-id="12cf8-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12cf8-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="12cf8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12cf8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12cf8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="12cf8-118">Optional query parameters</span></span>
<span data-ttu-id="12cf8-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="12cf8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="12cf8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12cf8-120">Request headers</span></span>
| <span data-ttu-id="12cf8-121">标头</span><span class="sxs-lookup"><span data-stu-id="12cf8-121">Header</span></span>       | <span data-ttu-id="12cf8-122">值</span><span class="sxs-lookup"><span data-stu-id="12cf8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12cf8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12cf8-123">Authorization</span></span>  | <span data-ttu-id="12cf8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12cf8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12cf8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12cf8-126">Content-Type</span></span>   | <span data-ttu-id="12cf8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12cf8-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12cf8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="12cf8-128">Request body</span></span>
<span data-ttu-id="12cf8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12cf8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12cf8-130">响应</span><span class="sxs-lookup"><span data-stu-id="12cf8-130">Response</span></span>

<span data-ttu-id="12cf8-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="12cf8-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12cf8-132">示例</span><span class="sxs-lookup"><span data-stu-id="12cf8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12cf8-133">请求</span><span class="sxs-lookup"><span data-stu-id="12cf8-133">Request</span></span>
<span data-ttu-id="12cf8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12cf8-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12cf8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="12cf8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="12cf8-136">C#</span><span class="sxs-lookup"><span data-stu-id="12cf8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12cf8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12cf8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12cf8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12cf8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="12cf8-139">响应</span><span class="sxs-lookup"><span data-stu-id="12cf8-139">Response</span></span>
<span data-ttu-id="12cf8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12cf8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
