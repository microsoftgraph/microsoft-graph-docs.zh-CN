---
title: 列出 directoryRoleTemplates
description: 检索 directoryroletemplate 对象的列表。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3750e5d036601089d226d64a5e219c1c70fb9cf0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436695"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="14985-103">列出 directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="14985-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="14985-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14985-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14985-105">检索 directoryroletemplate 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="14985-105">Retrieve a list of directoryroletemplate objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="14985-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="14985-106">Permissions</span></span>
<span data-ttu-id="14985-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14985-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14985-109">Permission type</span></span>      | <span data-ttu-id="14985-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14985-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14985-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14985-111">Delegated (work or school account)</span></span> | <span data-ttu-id="14985-112">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14985-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14985-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14985-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14985-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14985-114">Not supported.</span></span>    |
|<span data-ttu-id="14985-115">Application</span><span class="sxs-lookup"><span data-stu-id="14985-115">Application</span></span> | <span data-ttu-id="14985-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14985-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14985-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14985-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14985-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14985-118">Optional query parameters</span></span>
<span data-ttu-id="14985-119">此方法 **不** 支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="14985-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14985-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14985-120">Request headers</span></span>
| <span data-ttu-id="14985-121">名称</span><span class="sxs-lookup"><span data-stu-id="14985-121">Name</span></span>       | <span data-ttu-id="14985-122">类型</span><span class="sxs-lookup"><span data-stu-id="14985-122">Type</span></span> | <span data-ttu-id="14985-123">说明</span><span class="sxs-lookup"><span data-stu-id="14985-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14985-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14985-124">Authorization</span></span>  | <span data-ttu-id="14985-125">string</span><span class="sxs-lookup"><span data-stu-id="14985-125">string</span></span>  | <span data-ttu-id="14985-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14985-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14985-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="14985-128">Request body</span></span>
<span data-ttu-id="14985-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14985-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14985-130">响应</span><span class="sxs-lookup"><span data-stu-id="14985-130">Response</span></span>

<span data-ttu-id="14985-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRoleTemplate](../resources/directoryroletemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="14985-131">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14985-132">示例</span><span class="sxs-lookup"><span data-stu-id="14985-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14985-133">请求</span><span class="sxs-lookup"><span data-stu-id="14985-133">Request</span></span>
<span data-ttu-id="14985-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14985-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14985-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="14985-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```
# <a name="c"></a>[<span data-ttu-id="14985-136">C#</span><span class="sxs-lookup"><span data-stu-id="14985-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14985-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14985-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14985-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14985-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14985-139">Java</span><span class="sxs-lookup"><span data-stu-id="14985-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="14985-140">响应</span><span class="sxs-lookup"><span data-stu-id="14985-140">Response</span></span>
<span data-ttu-id="14985-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14985-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 139

{
  "value": [
    {
      "description": "description-value",
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
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
