---
title: 更新 tenantTag
description: 更新 tenantTag 对象的属性。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 367fd71e769ae2fa4cd73b0f25f120b22fa5f0d9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442710"
---
# <a name="update-tenanttag"></a><span data-ttu-id="540df-103">更新 tenantTag</span><span class="sxs-lookup"><span data-stu-id="540df-103">Update tenantTag</span></span>
<span data-ttu-id="540df-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="540df-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="540df-105">更新 [tenantTag 对象](../resources/managedtenants-tenanttag.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="540df-105">Update the properties of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="540df-106">权限</span><span class="sxs-lookup"><span data-stu-id="540df-106">Permissions</span></span>
<span data-ttu-id="540df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="540df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="540df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="540df-109">Permission type</span></span>|<span data-ttu-id="540df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="540df-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="540df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="540df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="540df-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="540df-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="540df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="540df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="540df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="540df-114">Not supported.</span></span>|
|<span data-ttu-id="540df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="540df-115">Application</span></span>|<span data-ttu-id="540df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="540df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="540df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="540df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="540df-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="540df-118">Request headers</span></span>
|<span data-ttu-id="540df-119">名称</span><span class="sxs-lookup"><span data-stu-id="540df-119">Name</span></span>|<span data-ttu-id="540df-120">说明</span><span class="sxs-lookup"><span data-stu-id="540df-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="540df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="540df-121">Authorization</span></span>|<span data-ttu-id="540df-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="540df-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="540df-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="540df-124">Content-Type</span></span>|<span data-ttu-id="540df-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="540df-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="540df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="540df-127">Request body</span></span>
<span data-ttu-id="540df-128">在请求正文中，提供应更新的相关 [tenantTag](../resources/managedtenants-tenanttag.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="540df-128">In the request body, supply the values for relevant [tenantTag](../resources/managedtenants-tenanttag.md) fields that should be updated.</span></span> <span data-ttu-id="540df-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="540df-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="540df-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="540df-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="540df-131">可以更新以下属性：</span><span class="sxs-lookup"><span data-stu-id="540df-131">Following properties can be updated:</span></span>

| <span data-ttu-id="540df-132">属性</span><span class="sxs-lookup"><span data-stu-id="540df-132">Property</span></span>     | <span data-ttu-id="540df-133">类型</span><span class="sxs-lookup"><span data-stu-id="540df-133">Type</span></span>        | <span data-ttu-id="540df-134">说明</span><span class="sxs-lookup"><span data-stu-id="540df-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="540df-135">displayName</span><span class="sxs-lookup"><span data-stu-id="540df-135">displayName</span></span>|<span data-ttu-id="540df-136">String</span><span class="sxs-lookup"><span data-stu-id="540df-136">String</span></span>|<span data-ttu-id="540df-137">租户显示名称的变量。</span><span class="sxs-lookup"><span data-stu-id="540df-137">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="540df-138">说明</span><span class="sxs-lookup"><span data-stu-id="540df-138">description</span></span>|<span data-ttu-id="540df-139">String</span><span class="sxs-lookup"><span data-stu-id="540df-139">String</span></span>|<span data-ttu-id="540df-140">租户标记的说明。</span><span class="sxs-lookup"><span data-stu-id="540df-140">The description for the tenant tag.</span></span>|
|<span data-ttu-id="540df-141">tenants</span><span class="sxs-lookup"><span data-stu-id="540df-141">tenants</span></span>|<span data-ttu-id="540df-142">[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="540df-142">[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) collection</span></span>|<span data-ttu-id="540df-143">与租户标记关联的托管租户的集合。</span><span class="sxs-lookup"><span data-stu-id="540df-143">The collection of managed tenants associated with the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="540df-144">响应</span><span class="sxs-lookup"><span data-stu-id="540df-144">Response</span></span>

<span data-ttu-id="540df-145">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="540df-145">If successful, this method returns a `200 OK` response code and an updated [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="540df-146">示例</span><span class="sxs-lookup"><span data-stu-id="540df-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="540df-147">请求</span><span class="sxs-lookup"><span data-stu-id="540df-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="540df-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="540df-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenanttag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
Content-Type: application/json
Content-length: 382

{
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding"
}
```
# <a name="c"></a>[<span data-ttu-id="540df-149">C#</span><span class="sxs-lookup"><span data-stu-id="540df-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="540df-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="540df-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="540df-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="540df-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="540df-152">Java</span><span class="sxs-lookup"><span data-stu-id="540df-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="540df-153">响应</span><span class="sxs-lookup"><span data-stu-id="540df-153">Response</span></span>
><span data-ttu-id="540df-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="540df-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "913391c0-5466-42b4-900d-0a7501399cb0",
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding",
  "tenantIds": [
    {
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-16T20:36:31.086644Z",
  "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
  "lastActionDateTime": "2021-07-11T18:54:44.5262828Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
