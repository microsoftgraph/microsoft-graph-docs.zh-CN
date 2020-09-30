---
title: 列出 childFolder
description: 获取指定联系人文件夹下的子文件夹的集合。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 36fdbb323c455c0fb2ebeef19d9f0ce5680b47c1
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312916"
---
# <a name="list-childfolders"></a><span data-ttu-id="a4938-103">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="a4938-103">List childFolders</span></span>

<span data-ttu-id="a4938-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4938-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4938-105">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="a4938-105">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4938-106">权限</span><span class="sxs-lookup"><span data-stu-id="a4938-106">Permissions</span></span>
<span data-ttu-id="a4938-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4938-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4938-109">Permission type</span></span>      | <span data-ttu-id="a4938-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4938-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4938-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4938-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4938-112">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4938-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a4938-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4938-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4938-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4938-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a4938-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4938-115">Application</span></span> | <span data-ttu-id="a4938-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4938-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4938-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4938-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4938-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4938-118">Optional query parameters</span></span>
<span data-ttu-id="a4938-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4938-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a4938-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4938-120">Request headers</span></span>
| <span data-ttu-id="a4938-121">名称</span><span class="sxs-lookup"><span data-stu-id="a4938-121">Name</span></span>       | <span data-ttu-id="a4938-122">类型</span><span class="sxs-lookup"><span data-stu-id="a4938-122">Type</span></span> | <span data-ttu-id="a4938-123">说明</span><span class="sxs-lookup"><span data-stu-id="a4938-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4938-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4938-124">Authorization</span></span>  | <span data-ttu-id="a4938-125">string</span><span class="sxs-lookup"><span data-stu-id="a4938-125">string</span></span>  | <span data-ttu-id="a4938-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4938-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4938-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4938-128">Request body</span></span>
<span data-ttu-id="a4938-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4938-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4938-130">响应</span><span class="sxs-lookup"><span data-stu-id="a4938-130">Response</span></span>

<span data-ttu-id="a4938-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a4938-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a4938-132">示例</span><span class="sxs-lookup"><span data-stu-id="a4938-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4938-133">请求</span><span class="sxs-lookup"><span data-stu-id="a4938-133">Request</span></span>
<span data-ttu-id="a4938-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4938-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4938-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4938-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="a4938-136">C#</span><span class="sxs-lookup"><span data-stu-id="a4938-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4938-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4938-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4938-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4938-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a4938-139">响应</span><span class="sxs-lookup"><span data-stu-id="a4938-139">Response</span></span>
<span data-ttu-id="a4938-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4938-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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