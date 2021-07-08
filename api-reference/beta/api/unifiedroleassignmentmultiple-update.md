---
title: 更新 unifiedRoleAssignmentMultiple
description: 更新新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3423c216e9b0c5b6928d0473c1e7db021e1344c9
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334491"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="f8b27-103">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="f8b27-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="f8b27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8b27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8b27-105">更新 RBAC [提供程序的现有 unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8b27-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="f8b27-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="f8b27-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="f8b27-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="f8b27-107">cloud PC</span></span> 
- <span data-ttu-id="f8b27-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="f8b27-108">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

<span data-ttu-id="f8b27-109">相比之下 [，unifiedRoleAssignment](../resources/unifiedroleassignment.md) 不支持更新。</span><span class="sxs-lookup"><span data-stu-id="f8b27-109">In contrast, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8b27-110">权限</span><span class="sxs-lookup"><span data-stu-id="f8b27-110">Permissions</span></span>

<span data-ttu-id="f8b27-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="f8b27-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="f8b27-112">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8b27-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="f8b27-113">对于云电脑提供商</span><span class="sxs-lookup"><span data-stu-id="f8b27-113">For Cloud PC provider</span></span>

|<span data-ttu-id="f8b27-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8b27-114">Permission type</span></span>      | <span data-ttu-id="f8b27-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8b27-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8b27-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8b27-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="f8b27-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b27-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="f8b27-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8b27-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8b27-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8b27-119">Not supported.</span></span>    |
|<span data-ttu-id="f8b27-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8b27-120">Application</span></span> | <span data-ttu-id="f8b27-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b27-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="f8b27-122">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="f8b27-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="f8b27-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8b27-123">Permission type</span></span>      | <span data-ttu-id="f8b27-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8b27-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8b27-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8b27-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="f8b27-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b27-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="f8b27-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8b27-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8b27-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8b27-128">Not supported.</span></span>    |
|<span data-ttu-id="f8b27-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8b27-129">Application</span></span> | <span data-ttu-id="f8b27-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b27-130">DeviceManagementRBAC.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f8b27-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8b27-131">HTTP request</span></span>

<span data-ttu-id="f8b27-132">若要更新云电脑提供商的现有 unfiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="f8b27-132">To update an existing unfiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="f8b27-133">若要更新 Intune 提供程序的现有 unfiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="f8b27-133">To update an existing unfiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="f8b27-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8b27-134">Request headers</span></span>

| <span data-ttu-id="f8b27-135">名称</span><span class="sxs-lookup"><span data-stu-id="f8b27-135">Name</span></span> | <span data-ttu-id="f8b27-136">说明</span><span class="sxs-lookup"><span data-stu-id="f8b27-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="f8b27-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8b27-137">Authorization</span></span> | <span data-ttu-id="f8b27-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8b27-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8b27-140">Content-type</span><span class="sxs-lookup"><span data-stu-id="f8b27-140">Content-type</span></span> | <span data-ttu-id="f8b27-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f8b27-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8b27-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8b27-143">Request body</span></span>

<span data-ttu-id="f8b27-144">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f8b27-144">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f8b27-145">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f8b27-145">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f8b27-146">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f8b27-146">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="f8b27-147">响应</span><span class="sxs-lookup"><span data-stu-id="f8b27-147">Response</span></span>

<span data-ttu-id="f8b27-148">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8b27-148">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8b27-149">示例</span><span class="sxs-lookup"><span data-stu-id="f8b27-149">Example</span></span>

### <a name="example-1-update-an-existing-unfiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="f8b27-150">示例 1：更新 Intune 提供程序中的现有 unfiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="f8b27-150">Example 1: Update an existing unfiedRoleAssignmentMultiple in an Intune provider</span></span>
### <a name="request"></a><span data-ttu-id="f8b27-151">请求</span><span class="sxs-lookup"><span data-stu-id="f8b27-151">Request</span></span>

<span data-ttu-id="f8b27-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8b27-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f8b27-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8b27-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f8b27-154">C#</span><span class="sxs-lookup"><span data-stu-id="f8b27-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8b27-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8b27-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8b27-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8b27-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8b27-157">Java</span><span class="sxs-lookup"><span data-stu-id="f8b27-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8b27-158">响应</span><span class="sxs-lookup"><span data-stu-id="f8b27-158">Response</span></span>

<span data-ttu-id="f8b27-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8b27-159">The following is an example of the response.</span></span>
> <span data-ttu-id="f8b27-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8b27-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK

```

## <a name="example-2-update-an-existing-unfiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="f8b27-161">示例 2：更新云电脑提供商中的现有 unfiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="f8b27-161">Example 2: update an existing unfiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="f8b27-162">请求</span><span class="sxs-lookup"><span data-stu-id="f8b27-162">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f8b27-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8b27-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
Content-type: application/json

{
    "displayName": "NewName",
    "description": "A new roleAssignment"
}
```
# <a name="c"></a>[<span data-ttu-id="f8b27-164">C#</span><span class="sxs-lookup"><span data-stu-id="f8b27-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8b27-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8b27-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8b27-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8b27-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8b27-167">Java</span><span class="sxs-lookup"><span data-stu-id="f8b27-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f8b27-168">响应</span><span class="sxs-lookup"><span data-stu-id="f8b27-168">Response</span></span>

> <span data-ttu-id="f8b27-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f8b27-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "description": "A new roleAssignment",
    "displayName": "NewName",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "0aeec2c1-fee7-4e02-b534-6f920d25b300",
        "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
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


