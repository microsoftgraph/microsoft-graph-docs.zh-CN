---
title: 创建 unifiedRoleAssignment
description: 创建新的 unifiedRoleAssignment 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 672eac457659c3af05f0a3e1fc92ec0fe283746e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454515"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="09ab7-103">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="09ab7-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="09ab7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="09ab7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ab7-105">创建新的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="09ab7-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09ab7-106">权限</span><span class="sxs-lookup"><span data-stu-id="09ab7-106">Permissions</span></span>

<span data-ttu-id="09ab7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09ab7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09ab7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09ab7-109">Permission type</span></span>                        | <span data-ttu-id="09ab7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09ab7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09ab7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09ab7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09ab7-112">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="09ab7-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="09ab7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09ab7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ab7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="09ab7-114">Not supported.</span></span> |
| <span data-ttu-id="09ab7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09ab7-115">Application</span></span>                            | <span data-ttu-id="09ab7-116">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="09ab7-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="09ab7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09ab7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="09ab7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09ab7-118">Request headers</span></span>

| <span data-ttu-id="09ab7-119">名称</span><span class="sxs-lookup"><span data-stu-id="09ab7-119">Name</span></span>          | <span data-ttu-id="09ab7-120">说明</span><span class="sxs-lookup"><span data-stu-id="09ab7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="09ab7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ab7-121">Authorization</span></span> | <span data-ttu-id="09ab7-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="09ab7-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="09ab7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="09ab7-123">Request body</span></span>

<span data-ttu-id="09ab7-124">在请求正文中，提供[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09ab7-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="09ab7-125">响应</span><span class="sxs-lookup"><span data-stu-id="09ab7-125">Response</span></span>

<span data-ttu-id="09ab7-126">如果成功，此方法在`201 Created`响应正文中返回响应代码和新的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="09ab7-126">If successful, this method returns `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09ab7-127">示例</span><span class="sxs-lookup"><span data-stu-id="09ab7-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="09ab7-128">请求</span><span class="sxs-lookup"><span data-stu-id="09ab7-128">Request</span></span>

<span data-ttu-id="09ab7-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09ab7-129">The following is an example of the request.</span></span> <span data-ttu-id="09ab7-130">请注意，使用 roleTemplateId 进行 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="09ab7-130">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="09ab7-131">roleDefinitionId 可以是服务范围的模板 Id，也可以是特定于目录的 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="09ab7-131">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>

# <a name="http"></a>[<span data-ttu-id="09ab7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="09ab7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "principalId":"a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "roleDefinitionId":"b0f54661-2d74-4c50-afa3-1ec803f12efe",
    "resourceScope":"/"
}
```
# <a name="c"></a>[<span data-ttu-id="09ab7-133">C#</span><span class="sxs-lookup"><span data-stu-id="09ab7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09ab7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09ab7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09ab7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09ab7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09ab7-136">响应</span><span class="sxs-lookup"><span data-stu-id="09ab7-136">Response</span></span>

<span data-ttu-id="09ab7-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09ab7-137">The following is an example of the response.</span></span>

> <span data-ttu-id="09ab7-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09ab7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "resourceScope": "/",
    "roleDefinitionId": "b0f54661-2d74-4c50-afa3-1ec803f12efe"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
