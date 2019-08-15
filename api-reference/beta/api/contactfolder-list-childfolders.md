---
title: 列出 childFolder
description: 获取指定联系人文件夹下的子文件夹的集合。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fb64378700743134dc791c8272515c920dbf1318
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417961"
---
# <a name="list-childfolders"></a><span data-ttu-id="2b1c1-103">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="2b1c1-103">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b1c1-104">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b1c1-105">权限</span><span class="sxs-lookup"><span data-stu-id="2b1c1-105">Permissions</span></span>
<span data-ttu-id="2b1c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b1c1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b1c1-108">Permission type</span></span>      | <span data-ttu-id="2b1c1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b1c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b1c1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b1c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b1c1-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b1c1-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2b1c1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b1c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b1c1-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b1c1-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2b1c1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b1c1-114">Application</span></span> | <span data-ttu-id="2b1c1-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b1c1-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b1c1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b1c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b1c1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2b1c1-117">Optional query parameters</span></span>
<span data-ttu-id="2b1c1-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2b1c1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b1c1-119">Request headers</span></span>
| <span data-ttu-id="2b1c1-120">名称</span><span class="sxs-lookup"><span data-stu-id="2b1c1-120">Name</span></span>       | <span data-ttu-id="2b1c1-121">类型</span><span class="sxs-lookup"><span data-stu-id="2b1c1-121">Type</span></span> | <span data-ttu-id="2b1c1-122">说明</span><span class="sxs-lookup"><span data-stu-id="2b1c1-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b1c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b1c1-123">Authorization</span></span>  | <span data-ttu-id="2b1c1-124">string</span><span class="sxs-lookup"><span data-stu-id="2b1c1-124">string</span></span>  | <span data-ttu-id="2b1c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b1c1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b1c1-127">Request body</span></span>
<span data-ttu-id="2b1c1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b1c1-129">响应</span><span class="sxs-lookup"><span data-stu-id="2b1c1-129">Response</span></span>

<span data-ttu-id="2b1c1-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b1c1-131">示例</span><span class="sxs-lookup"><span data-stu-id="2b1c1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b1c1-132">请求</span><span class="sxs-lookup"><span data-stu-id="2b1c1-132">Request</span></span>
<span data-ttu-id="2b1c1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2b1c1-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2b1c1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b1c1-135">C#</span><span class="sxs-lookup"><span data-stu-id="2b1c1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b1c1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b1c1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b1c1-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="2b1c1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b1c1-138">响应</span><span class="sxs-lookup"><span data-stu-id="2b1c1-138">Response</span></span>
<span data-ttu-id="2b1c1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b1c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
