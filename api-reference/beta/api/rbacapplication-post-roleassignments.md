---
title: 创建 unifiedRoleAssignment
description: 创建新的 unifiedRoleAssignment 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1ce6c7d99a3316bdb5c45780f41e181906ff76f7
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437690"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="7824a-103">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7824a-103">Create unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7824a-104">创建新的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7824a-104">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7824a-105">权限</span><span class="sxs-lookup"><span data-stu-id="7824a-105">Permissions</span></span>

<span data-ttu-id="7824a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7824a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7824a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7824a-108">Permission type</span></span>                        | <span data-ttu-id="7824a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7824a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7824a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7824a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7824a-111">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="7824a-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="7824a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7824a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7824a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7824a-113">Not supported.</span></span> |
| <span data-ttu-id="7824a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7824a-114">Application</span></span>                            | <span data-ttu-id="7824a-115">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="7824a-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="7824a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7824a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="7824a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7824a-117">Request headers</span></span>

| <span data-ttu-id="7824a-118">名称</span><span class="sxs-lookup"><span data-stu-id="7824a-118">Name</span></span>          | <span data-ttu-id="7824a-119">说明</span><span class="sxs-lookup"><span data-stu-id="7824a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7824a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7824a-120">Authorization</span></span> | <span data-ttu-id="7824a-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7824a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7824a-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="7824a-122">Request body</span></span>

<span data-ttu-id="7824a-123">在请求正文中, 提供[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7824a-123">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7824a-124">响应</span><span class="sxs-lookup"><span data-stu-id="7824a-124">Response</span></span>

<span data-ttu-id="7824a-125">如果成功, 此方法在`201 Created`响应正文中返回响应代码和新的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7824a-125">If successful, this method returns `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7824a-126">示例</span><span class="sxs-lookup"><span data-stu-id="7824a-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="7824a-127">请求</span><span class="sxs-lookup"><span data-stu-id="7824a-127">Request</span></span>

<span data-ttu-id="7824a-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7824a-128">The following is an example of the request.</span></span> <span data-ttu-id="7824a-129">请注意, 使用 roleTemplateId 进行 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="7824a-129">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="7824a-130">roleDefinitionId 可以是服务范围的模板 Id, 也可以是特定于目录的 roleDefinitionId。</span><span class="sxs-lookup"><span data-stu-id="7824a-130">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>
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

### <a name="response"></a><span data-ttu-id="7824a-131">响应</span><span class="sxs-lookup"><span data-stu-id="7824a-131">Response</span></span>

<span data-ttu-id="7824a-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7824a-132">The following is an example of the response.</span></span>

> <span data-ttu-id="7824a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7824a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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