---
title: 获取 unifiedRoleAssignment
description: 检索 unifiedRoleAssignment 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 43cf52fde2719f44ac03c6c31444d135e925e460
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452062"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="aa689-103">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="aa689-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="aa689-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="aa689-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa689-105">检索[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa689-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa689-106">权限</span><span class="sxs-lookup"><span data-stu-id="aa689-106">Permissions</span></span>

<span data-ttu-id="aa689-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa689-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa689-109">Permission type</span></span>      | <span data-ttu-id="aa689-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa689-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa689-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa689-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa689-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="aa689-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa689-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa689-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa689-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa689-114">Not supported.</span></span>    |
|<span data-ttu-id="aa689-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa689-115">Application</span></span> | <span data-ttu-id="aa689-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="aa689-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa689-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa689-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa689-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aa689-118">Optional query parameters</span></span>

<span data-ttu-id="aa689-119">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aa689-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="aa689-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="aa689-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa689-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa689-121">Request headers</span></span>

| <span data-ttu-id="aa689-122">名称</span><span class="sxs-lookup"><span data-stu-id="aa689-122">Name</span></span>      |<span data-ttu-id="aa689-123">说明</span><span class="sxs-lookup"><span data-stu-id="aa689-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa689-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa689-124">Authorization</span></span> | <span data-ttu-id="aa689-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="aa689-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa689-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa689-126">Request body</span></span>

<span data-ttu-id="aa689-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa689-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa689-128">响应</span><span class="sxs-lookup"><span data-stu-id="aa689-128">Response</span></span>

<span data-ttu-id="aa689-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aa689-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa689-130">示例</span><span class="sxs-lookup"><span data-stu-id="aa689-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa689-131">请求</span><span class="sxs-lookup"><span data-stu-id="aa689-131">Request</span></span>

<span data-ttu-id="aa689-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa689-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa689-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa689-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="aa689-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa689-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa689-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa689-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa689-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa689-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa689-137">响应</span><span class="sxs-lookup"><span data-stu-id="aa689-137">Response</span></span>

<span data-ttu-id="aa689-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa689-138">The following is an example of the response.</span></span>

> <span data-ttu-id="aa689-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aa689-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "resourceScope": "/",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
