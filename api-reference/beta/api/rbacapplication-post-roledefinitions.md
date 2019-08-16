---
title: 创建 unifiedRoleDefinition
description: 创建新的 unifiedRoleDefinition 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 803f21d56a6d02a64013a711cf5419996eb73de8
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437711"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="ef4d2-103">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ef4d2-103">Create unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef4d2-104">创建新的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-104">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef4d2-105">权限</span><span class="sxs-lookup"><span data-stu-id="ef4d2-105">Permissions</span></span>

<span data-ttu-id="ef4d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef4d2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef4d2-108">Permission type</span></span>                        | <span data-ttu-id="ef4d2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef4d2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ef4d2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef4d2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef4d2-111">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="ef4d2-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="ef4d2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef4d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef4d2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-113">Not supported.</span></span> |
| <span data-ttu-id="ef4d2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef4d2-114">Application</span></span>                            | <span data-ttu-id="ef4d2-115">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="ef4d2-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef4d2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef4d2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ef4d2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef4d2-117">Request headers</span></span>

| <span data-ttu-id="ef4d2-118">名称</span><span class="sxs-lookup"><span data-stu-id="ef4d2-118">Name</span></span>          | <span data-ttu-id="ef4d2-119">说明</span><span class="sxs-lookup"><span data-stu-id="ef4d2-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ef4d2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef4d2-120">Authorization</span></span> | <span data-ttu-id="ef4d2-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ef4d2-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef4d2-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef4d2-122">Request body</span></span>

<span data-ttu-id="ef4d2-123">在请求正文中, 提供[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-123">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="ef4d2-124">下表显示创建 roleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-124">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="ef4d2-125">参数</span><span class="sxs-lookup"><span data-stu-id="ef4d2-125">Parameter</span></span> | <span data-ttu-id="ef4d2-126">类型</span><span class="sxs-lookup"><span data-stu-id="ef4d2-126">Type</span></span> | <span data-ttu-id="ef4d2-127">说明</span><span class="sxs-lookup"><span data-stu-id="ef4d2-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef4d2-128">displayName</span><span class="sxs-lookup"><span data-stu-id="ef4d2-128">displayName</span></span> |<span data-ttu-id="ef4d2-129">string</span><span class="sxs-lookup"><span data-stu-id="ef4d2-129">string</span></span> |<span data-ttu-id="ef4d2-130">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-130">The display name for the role definition.</span></span>|
|<span data-ttu-id="ef4d2-131">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ef4d2-131">isEnabled</span></span> |<span data-ttu-id="ef4d2-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef4d2-132">Boolean</span></span> |<span data-ttu-id="ef4d2-133">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-133">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="ef4d2-134">如果为 false, 则该角色不可用于分配。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-134">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="ef4d2-135">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ef4d2-135">rolePermissions</span></span> |<span data-ttu-id="ef4d2-136">[unifiedRolePermission](../resources/unifiedrolepermission.md)集合</span><span class="sxs-lookup"><span data-stu-id="ef4d2-136">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="ef4d2-137">角色中包含的权限的列表。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-137">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="ef4d2-138">响应</span><span class="sxs-lookup"><span data-stu-id="ef4d2-138">Response</span></span>

<span data-ttu-id="ef4d2-139">如果成功, 此方法在`201 Created`响应正文中返回响应代码和新的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-139">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef4d2-140">示例</span><span class="sxs-lookup"><span data-stu-id="ef4d2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef4d2-141">请求</span><span class="sxs-lookup"><span data-stu-id="ef4d2-141">Request</span></span>

<span data-ttu-id="ef4d2-142">下面是创建自定义角色的示例。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-142">The following is an example of creating a custom role.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```

### <a name="response"></a><span data-ttu-id="ef4d2-143">响应</span><span class="sxs-lookup"><span data-stu-id="ef4d2-143">Response</span></span>

<span data-ttu-id="ef4d2-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-144">The following is an example of the response.</span></span>

> <span data-ttu-id="ef4d2-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ef4d2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "c2cb59a3-2d01-4176-a458-95b0e674966f",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
