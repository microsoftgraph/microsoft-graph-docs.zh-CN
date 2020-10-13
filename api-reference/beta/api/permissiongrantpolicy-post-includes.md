---
title: 在包含 permissionGrantPolicy 的集合中创建 permissionGrantConditionSet
description: 添加权限授予策略中包含权限授予事件的条件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: e53acd2bb17a1082384f7c7f694aea34fc3911fc
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433541"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="78a6c-103">在包含 permissionGrantPolicy 的集合中创建 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="78a6c-103">Create permissionGrantConditionSet in includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="78a6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78a6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78a6c-105">添加权限授予策略中 *包含* 权限授予事件的条件。</span><span class="sxs-lookup"><span data-stu-id="78a6c-105">Add conditions under which a permission grant event is *included* in a permission grant policy.</span></span> <span data-ttu-id="78a6c-106">为此，请将[permissionGrantConditionSet](../resources/permissiongrantconditionset.md)添加到[permissionGrantPolicy](../resources/permissionGrantPolicy.md)的**包含**集合中。</span><span class="sxs-lookup"><span data-stu-id="78a6c-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **includes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="78a6c-107">权限</span><span class="sxs-lookup"><span data-stu-id="78a6c-107">Permissions</span></span>

<span data-ttu-id="78a6c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78a6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78a6c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="78a6c-110">Permission type</span></span>      | <span data-ttu-id="78a6c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78a6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78a6c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78a6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78a6c-113">PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="78a6c-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="78a6c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78a6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78a6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="78a6c-115">Not supported.</span></span>    |
|<span data-ttu-id="78a6c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="78a6c-116">Application</span></span> | <span data-ttu-id="78a6c-117">PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="78a6c-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="78a6c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78a6c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a><span data-ttu-id="78a6c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="78a6c-119">Request headers</span></span>

| <span data-ttu-id="78a6c-120">名称</span><span class="sxs-lookup"><span data-stu-id="78a6c-120">Name</span></span>       | <span data-ttu-id="78a6c-121">说明</span><span class="sxs-lookup"><span data-stu-id="78a6c-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="78a6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78a6c-122">Authorization</span></span> | <span data-ttu-id="78a6c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78a6c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="78a6c-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="78a6c-125">Content-type</span></span> | <span data-ttu-id="78a6c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="78a6c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78a6c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="78a6c-128">Request body</span></span>

<span data-ttu-id="78a6c-129">在请求正文中，提供 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78a6c-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="78a6c-130">响应</span><span class="sxs-lookup"><span data-stu-id="78a6c-130">Response</span></span>

<span data-ttu-id="78a6c-131">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78a6c-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78a6c-132">示例</span><span class="sxs-lookup"><span data-stu-id="78a6c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78a6c-133">请求</span><span class="sxs-lookup"><span data-stu-id="78a6c-133">Request</span></span>

<span data-ttu-id="78a6c-134">在此示例中，来自已验证发布者的客户端应用程序的 *所有* 委派权限都包含在权限授予策略中。</span><span class="sxs-lookup"><span data-stu-id="78a6c-134">In this example, *all* delegated permissions for client apps from verified publishers are included in the permission grant policy.</span></span> <span data-ttu-id="78a6c-135">由于省略了 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 中的所有其他条件，因此它们将采用其默认值，在每种情况下都是最包含的值。</span><span class="sxs-lookup"><span data-stu-id="78a6c-135">Because all the other conditions from the [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) were omitted, they will take their default values, which in each case is the most-inclusive.</span></span>

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
}
```

### <a name="response"></a><span data-ttu-id="78a6c-136">响应</span><span class="sxs-lookup"><span data-stu-id="78a6c-136">Response</span></span>

<span data-ttu-id="78a6c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="78a6c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="78a6c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78a6c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "75ffda85-9314-43bc-bf19-554a7d079e96",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "any",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
