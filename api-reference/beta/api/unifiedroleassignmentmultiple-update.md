---
title: 更新 unifiedRoleAssignmentMultiple
description: 更新新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 60684d2aea0d6a0dc1148f8e486707422d538faf
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160340"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="d095d-103">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d095d-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="d095d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d095d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d095d-105">更新现有的[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d095d-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="d095d-106">使用此项可在 Microsoft Intune 中更新角色分配。</span><span class="sxs-lookup"><span data-stu-id="d095d-106">Use this to update role assignments in Microsoft Intune.</span></span> <span data-ttu-id="d095d-107">请注意， [unifiedRoleAssignment](../resources/unifiedroleassignment.md)不支持 update。</span><span class="sxs-lookup"><span data-stu-id="d095d-107">Note that [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="d095d-108">权限</span><span class="sxs-lookup"><span data-stu-id="d095d-108">Permissions</span></span>

<span data-ttu-id="d095d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d095d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d095d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d095d-111">Permission type</span></span> | <span data-ttu-id="d095d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d095d-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="d095d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d095d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d095d-114">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="d095d-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="d095d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d095d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d095d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d095d-116">Not supported.</span></span> |
| <span data-ttu-id="d095d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d095d-117">Application</span></span> | <span data-ttu-id="d095d-118">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="d095d-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="d095d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d095d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d095d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d095d-120">Request headers</span></span>

| <span data-ttu-id="d095d-121">名称</span><span class="sxs-lookup"><span data-stu-id="d095d-121">Name</span></span> | <span data-ttu-id="d095d-122">说明</span><span class="sxs-lookup"><span data-stu-id="d095d-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="d095d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d095d-123">Authorization</span></span> | <span data-ttu-id="d095d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d095d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d095d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d095d-126">Content-type</span></span> | <span data-ttu-id="d095d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d095d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d095d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d095d-129">Request body</span></span>

<span data-ttu-id="d095d-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d095d-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d095d-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d095d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d095d-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d095d-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="d095d-133">响应</span><span class="sxs-lookup"><span data-stu-id="d095d-133">Response</span></span>

<span data-ttu-id="d095d-134">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d095d-134">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d095d-135">示例</span><span class="sxs-lookup"><span data-stu-id="d095d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="d095d-136">请求</span><span class="sxs-lookup"><span data-stu-id="d095d-136">Request</span></span>

<span data-ttu-id="d095d-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d095d-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
Content-type: application/json

{ 
    "principalIds": ["0aeec2c1-fee7-4e02-b534-6f920d25b300", "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"]
}
```

### <a name="response"></a><span data-ttu-id="d095d-138">响应</span><span class="sxs-lookup"><span data-stu-id="d095d-138">Response</span></span>

<span data-ttu-id="d095d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d095d-139">The following is an example of the response.</span></span>
> <span data-ttu-id="d095d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d095d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 204 OK

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
