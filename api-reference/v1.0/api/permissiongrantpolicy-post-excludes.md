---
title: 在排除 permissionGrantPolicy 集合中创建 permissionGrantConditionSet
description: 添加在权限授予策略中排除权限授予事件的条件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9011d194e0de5f0efea0d5a483219896b0f71073
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377151"
---
# <a name="create-permissiongrantconditionset-in-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="3511d-103">在排除 permissionGrantPolicy 集合中创建 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="3511d-103">Create permissionGrantConditionSet in excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="3511d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3511d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3511d-105">添加在权限授予策略中 *排除* 权限授予事件的条件。</span><span class="sxs-lookup"><span data-stu-id="3511d-105">Add conditions under which a permission grant event is *excluded* in a permission grant policy.</span></span> <span data-ttu-id="3511d-106">为此，请将 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md)添加到 [permissionGrantPolicy](../resources/permissionGrantPolicy.md)的 "**排除**" 集合中。</span><span class="sxs-lookup"><span data-stu-id="3511d-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **excludes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3511d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3511d-107">Permissions</span></span>

<span data-ttu-id="3511d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3511d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3511d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3511d-110">Permission type</span></span>      | <span data-ttu-id="3511d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3511d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3511d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3511d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3511d-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="3511d-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="3511d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3511d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3511d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3511d-115">Not supported.</span></span>    |
|<span data-ttu-id="3511d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3511d-116">Application</span></span> | <span data-ttu-id="3511d-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="3511d-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="3511d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3511d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="request-headers"></a><span data-ttu-id="3511d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3511d-119">Request headers</span></span>

| <span data-ttu-id="3511d-120">名称</span><span class="sxs-lookup"><span data-stu-id="3511d-120">Name</span></span>       | <span data-ttu-id="3511d-121">说明</span><span class="sxs-lookup"><span data-stu-id="3511d-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="3511d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3511d-122">Authorization</span></span> | <span data-ttu-id="3511d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3511d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3511d-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="3511d-125">Content-type</span></span> | <span data-ttu-id="3511d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3511d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3511d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3511d-128">Request body</span></span>

<span data-ttu-id="3511d-129">在请求正文中，提供 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3511d-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3511d-130">响应</span><span class="sxs-lookup"><span data-stu-id="3511d-130">Response</span></span>

<span data-ttu-id="3511d-131">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3511d-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3511d-132">示例</span><span class="sxs-lookup"><span data-stu-id="3511d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3511d-133">请求</span><span class="sxs-lookup"><span data-stu-id="3511d-133">Request</span></span>

<span data-ttu-id="3511d-134">在此示例中，Microsoft Graph 的 *所有* 委派权限 (**appId** 00000003-0000-0000-c000-000000000000) 被排除在权限授予策略之外。</span><span class="sxs-lookup"><span data-stu-id="3511d-134">In this example, *all* delegated permissions for Microsoft Graph (**appId** 00000003-0000-0000-c000-000000000000) are excluded from the permission grant policy.</span></span>

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_excludes"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes
Content-Type: application/json

{
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000"
}
```

### <a name="response"></a><span data-ttu-id="3511d-135">响应</span><span class="sxs-lookup"><span data-stu-id="3511d-135">Response</span></span>

<span data-ttu-id="3511d-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3511d-136">The following is an example of the response.</span></span>

> <span data-ttu-id="3511d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3511d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "9a532f49-e646-405d-8c7c-d4c8e8a4d294",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
