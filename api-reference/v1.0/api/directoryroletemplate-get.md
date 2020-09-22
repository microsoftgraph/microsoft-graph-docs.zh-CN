---
title: 获取 directoryRoleTemplate
description: 检索 directoryroletemplate 对象的属性和关系。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6c377c6e364de5225e39c93f0b9faa6119af641a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052325"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="4cb19-103">获取 directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="4cb19-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="4cb19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cb19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cb19-105">检索 directoryroletemplate 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4cb19-105">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cb19-106">权限</span><span class="sxs-lookup"><span data-stu-id="4cb19-106">Permissions</span></span>
<span data-ttu-id="4cb19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cb19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb19-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cb19-109">Permission type</span></span>      | <span data-ttu-id="4cb19-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cb19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cb19-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cb19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4cb19-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="4cb19-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4cb19-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cb19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb19-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cb19-114">Not supported.</span></span>    |
|<span data-ttu-id="4cb19-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4cb19-115">Application</span></span> | <span data-ttu-id="4cb19-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="4cb19-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cb19-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cb19-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4cb19-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4cb19-118">Optional query parameters</span></span>
<span data-ttu-id="4cb19-119">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="4cb19-119">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cb19-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cb19-120">Request headers</span></span>
| <span data-ttu-id="4cb19-121">名称</span><span class="sxs-lookup"><span data-stu-id="4cb19-121">Name</span></span>       | <span data-ttu-id="4cb19-122">类型</span><span class="sxs-lookup"><span data-stu-id="4cb19-122">Type</span></span> | <span data-ttu-id="4cb19-123">说明</span><span class="sxs-lookup"><span data-stu-id="4cb19-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4cb19-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cb19-124">Authorization</span></span>  | <span data-ttu-id="4cb19-125">string</span><span class="sxs-lookup"><span data-stu-id="4cb19-125">string</span></span>  | <span data-ttu-id="4cb19-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4cb19-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cb19-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cb19-128">Request body</span></span>
<span data-ttu-id="4cb19-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4cb19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cb19-130">响应</span><span class="sxs-lookup"><span data-stu-id="4cb19-130">Response</span></span>

<span data-ttu-id="4cb19-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRoleTemplate](../resources/directoryroletemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4cb19-131">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4cb19-132">示例</span><span class="sxs-lookup"><span data-stu-id="4cb19-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cb19-133">请求</span><span class="sxs-lookup"><span data-stu-id="4cb19-133">Request</span></span>
<span data-ttu-id="4cb19-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4cb19-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4cb19-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cb19-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="4cb19-136">C#</span><span class="sxs-lookup"><span data-stu-id="4cb19-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cb19-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cb19-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cb19-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cb19-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4cb19-139">Java</span><span class="sxs-lookup"><span data-stu-id="4cb19-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4cb19-140">响应</span><span class="sxs-lookup"><span data-stu-id="4cb19-140">Response</span></span>
<span data-ttu-id="4cb19-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4cb19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

