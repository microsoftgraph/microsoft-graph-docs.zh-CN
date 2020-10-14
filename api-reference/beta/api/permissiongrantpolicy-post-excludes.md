---
title: 在排除 permissionGrantPolicy 集合中创建 permissionGrantConditionSet
description: 添加在权限授予策略中排除权限授予事件的条件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4fc5f04ebfcb4c07fb8eef894445b2fa9164ed6c
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458694"
---
# <a name="create-permissiongrantconditionset-in-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="bd263-103">在排除 permissionGrantPolicy 集合中创建 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="bd263-103">Create permissionGrantConditionSet in excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="bd263-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd263-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd263-105">添加在权限授予策略中 *排除* 权限授予事件的条件。</span><span class="sxs-lookup"><span data-stu-id="bd263-105">Add conditions under which a permission grant event is *excluded* in a permission grant policy.</span></span> <span data-ttu-id="bd263-106">为此，请将[permissionGrantConditionSet](../resources/permissiongrantconditionset.md)添加到[permissionGrantPolicy](../resources/permissionGrantPolicy.md)的 "**排除**" 集合中。</span><span class="sxs-lookup"><span data-stu-id="bd263-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **excludes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd263-107">权限</span><span class="sxs-lookup"><span data-stu-id="bd263-107">Permissions</span></span>

<span data-ttu-id="bd263-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd263-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd263-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd263-110">Permission type</span></span>      | <span data-ttu-id="bd263-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd263-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd263-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd263-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bd263-113">PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bd263-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="bd263-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd263-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd263-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd263-115">Not supported.</span></span>    |
|<span data-ttu-id="bd263-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd263-116">Application</span></span> | <span data-ttu-id="bd263-117">PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bd263-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd263-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd263-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="request-headers"></a><span data-ttu-id="bd263-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd263-119">Request headers</span></span>

| <span data-ttu-id="bd263-120">名称</span><span class="sxs-lookup"><span data-stu-id="bd263-120">Name</span></span>       | <span data-ttu-id="bd263-121">说明</span><span class="sxs-lookup"><span data-stu-id="bd263-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="bd263-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd263-122">Authorization</span></span> | <span data-ttu-id="bd263-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd263-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd263-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="bd263-125">Content-type</span></span> | <span data-ttu-id="bd263-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bd263-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd263-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd263-128">Request body</span></span>

<span data-ttu-id="bd263-129">在请求正文中，提供 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd263-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bd263-130">响应</span><span class="sxs-lookup"><span data-stu-id="bd263-130">Response</span></span>

<span data-ttu-id="bd263-131">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd263-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd263-132">示例</span><span class="sxs-lookup"><span data-stu-id="bd263-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd263-133">请求</span><span class="sxs-lookup"><span data-stu-id="bd263-133">Request</span></span>

<span data-ttu-id="bd263-134">在此示例中，Microsoft Graph 的 *所有* 委派权限 (**appId** 00000003-0000-0000-c000-000000000000) 被排除在权限授予策略之外。</span><span class="sxs-lookup"><span data-stu-id="bd263-134">In this example, *all* delegated permissions for Microsoft Graph (**appId** 00000003-0000-0000-c000-000000000000) are excluded from the permission grant policy.</span></span>


# <a name="http"></a>[<span data-ttu-id="bd263-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd263-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_excludes"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes
Content-Type: application/json

{
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="bd263-136">C#</span><span class="sxs-lookup"><span data-stu-id="bd263-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd263-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd263-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd263-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd263-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd263-139">响应</span><span class="sxs-lookup"><span data-stu-id="bd263-139">Response</span></span>

<span data-ttu-id="bd263-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd263-140">The following is an example of the response.</span></span>

> <span data-ttu-id="bd263-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd263-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
