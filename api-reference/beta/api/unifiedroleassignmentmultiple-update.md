---
title: 更新 unifiedRoleAssignmentMultiple
description: 更新新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c13242b11ed9cfdf58c3047d40937edc483c1cd6
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869924"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="0a466-103">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0a466-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="0a466-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a466-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a466-105">更新 RBAC [提供程序的现有 unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a466-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="0a466-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="0a466-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="0a466-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="0a466-107">cloud PC</span></span> 
- <span data-ttu-id="0a466-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="0a466-108">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

<span data-ttu-id="0a466-109">相比之下 [，unifiedRoleAssignment](../resources/unifiedroleassignment.md) 不支持更新。</span><span class="sxs-lookup"><span data-stu-id="0a466-109">In contrast, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a466-110">权限</span><span class="sxs-lookup"><span data-stu-id="0a466-110">Permissions</span></span>

<span data-ttu-id="0a466-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="0a466-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="0a466-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="0a466-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="0a466-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="0a466-113">Supported provider</span></span>      | <span data-ttu-id="0a466-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a466-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="0a466-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a466-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a466-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a466-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="0a466-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="0a466-117">Cloud PC</span></span> | <span data-ttu-id="0a466-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a466-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="0a466-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a466-119">Not supported.</span></span> | <span data-ttu-id="0a466-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a466-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="0a466-121">Intune</span><span class="sxs-lookup"><span data-stu-id="0a466-121">Intune</span></span> | <span data-ttu-id="0a466-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a466-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="0a466-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a466-123">Not supported.</span></span>| <span data-ttu-id="0a466-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a466-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a466-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a466-125">HTTP request</span></span>

<span data-ttu-id="0a466-126">若要更新云电脑提供商的现有 unfiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="0a466-126">To update an existing unfiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="0a466-127">若要更新 Intune 提供程序的现有 unfiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="0a466-127">To update an existing unfiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0a466-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a466-128">Request headers</span></span>

| <span data-ttu-id="0a466-129">名称</span><span class="sxs-lookup"><span data-stu-id="0a466-129">Name</span></span> | <span data-ttu-id="0a466-130">说明</span><span class="sxs-lookup"><span data-stu-id="0a466-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0a466-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a466-131">Authorization</span></span> | <span data-ttu-id="0a466-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a466-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a466-134">Content-type</span><span class="sxs-lookup"><span data-stu-id="0a466-134">Content-type</span></span> | <span data-ttu-id="0a466-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0a466-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a466-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a466-137">Request body</span></span>

<span data-ttu-id="0a466-138">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0a466-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0a466-139">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0a466-139">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0a466-140">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0a466-140">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="0a466-141">响应</span><span class="sxs-lookup"><span data-stu-id="0a466-141">Response</span></span>

<span data-ttu-id="0a466-142">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a466-142">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a466-143">示例</span><span class="sxs-lookup"><span data-stu-id="0a466-143">Example</span></span>

### <a name="example-1-update-an-existing-unfiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="0a466-144">示例 1：更新 Intune 提供程序中的现有 unfiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0a466-144">Example 1: Update an existing unfiedRoleAssignmentMultiple in an Intune provider</span></span>
### <a name="request"></a><span data-ttu-id="0a466-145">请求</span><span class="sxs-lookup"><span data-stu-id="0a466-145">Request</span></span>

<span data-ttu-id="0a466-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a466-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0a466-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a466-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0a466-148">C#</span><span class="sxs-lookup"><span data-stu-id="0a466-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a466-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a466-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a466-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a466-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a466-151">Java</span><span class="sxs-lookup"><span data-stu-id="0a466-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a466-152">响应</span><span class="sxs-lookup"><span data-stu-id="0a466-152">Response</span></span>

<span data-ttu-id="0a466-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0a466-153">The following is an example of the response.</span></span>
> <span data-ttu-id="0a466-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a466-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK

```

## <a name="example-2-update-an-existing-unfiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="0a466-155">示例 2：更新云电脑提供商中的现有 unfiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0a466-155">Example 2: update an existing unfiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="0a466-156">请求</span><span class="sxs-lookup"><span data-stu-id="0a466-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0a466-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a466-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0a466-158">C#</span><span class="sxs-lookup"><span data-stu-id="0a466-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a466-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a466-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a466-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a466-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a466-161">Java</span><span class="sxs-lookup"><span data-stu-id="0a466-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0a466-162">响应</span><span class="sxs-lookup"><span data-stu-id="0a466-162">Response</span></span>

> <span data-ttu-id="0a466-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0a466-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


