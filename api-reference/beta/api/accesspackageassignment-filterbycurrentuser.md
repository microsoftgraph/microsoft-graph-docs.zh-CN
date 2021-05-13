---
title: accessPackageAssignment：filterByCurrentUser
description: 检索在登录用户上筛选的 accesspackageassignment 对象列表。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b9ea85fb61525c2d9a3d109b358e8295631ac627
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473998"
---
# <a name="accesspackageassignment-filterbycurrentuser"></a><span data-ttu-id="4e342-103">accessPackageAssignment：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="4e342-103">accessPackageAssignment: filterByCurrentUser</span></span>
<span data-ttu-id="4e342-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e342-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e342-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索已登录用户筛选的 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="4e342-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e342-106">权限</span><span class="sxs-lookup"><span data-stu-id="4e342-106">Permissions</span></span>
<span data-ttu-id="4e342-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e342-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e342-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e342-109">Permission type</span></span>|<span data-ttu-id="4e342-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e342-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e342-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e342-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4e342-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e342-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="4e342-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e342-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e342-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e342-114">Not supported.</span></span>|
|<span data-ttu-id="4e342-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e342-115">Application</span></span>|<span data-ttu-id="4e342-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e342-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e342-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e342-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="4e342-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="4e342-118">Function parameters</span></span>
<span data-ttu-id="4e342-119">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="4e342-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4e342-120">参数</span><span class="sxs-lookup"><span data-stu-id="4e342-120">Parameter</span></span>|<span data-ttu-id="4e342-121">类型</span><span class="sxs-lookup"><span data-stu-id="4e342-121">Type</span></span>|<span data-ttu-id="4e342-122">说明</span><span class="sxs-lookup"><span data-stu-id="4e342-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e342-123">on</span><span class="sxs-lookup"><span data-stu-id="4e342-123">on</span></span>|[<span data-ttu-id="4e342-124">accessPackageAssignmentFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="4e342-124">accessPackageAssignmentFilterByCurrentUserOptions</span></span>](../resources/accesspackageassignment-accesspackageassignmentfilterbycurrentuseroptions.md)|<span data-ttu-id="4e342-125">可用于在访问包分配列表上进行筛选的当前用户选项的列表。</span><span class="sxs-lookup"><span data-stu-id="4e342-125">The list of current user options that can be used to filter on the access package assignments list.</span></span>|

- <span data-ttu-id="4e342-126">`target` 用于获取 `accessPackageAssignment` 已登录用户作为目标的对象。</span><span class="sxs-lookup"><span data-stu-id="4e342-126">`target` is used to get the `accessPackageAssignment` objects where the signed-in user is the target.</span></span> <span data-ttu-id="4e342-127">生成的列表包括所有目录和访问包中调用方的所有分配（当前分配和过期分配）。</span><span class="sxs-lookup"><span data-stu-id="4e342-127">The resulting list includes all of the assignments, current and expired, for the caller across all catalogs and access packages.</span></span>

- <span data-ttu-id="4e342-128">`createdBy` 用于获取 `accessPackageAssignment` 已登录用户创建的对象。</span><span class="sxs-lookup"><span data-stu-id="4e342-128">`createdBy` is used to get the `accessPackageAssignment` objects created by the signed-in user.</span></span> <span data-ttu-id="4e342-129">结果列表包括所有目录和访问包中调用方为自己或代表其他人创建的所有分配，例如管理员直接分配。</span><span class="sxs-lookup"><span data-stu-id="4e342-129">The resulting list includes all of the assignments that the caller created for themselves or on behalf of others, such as in case of admin direct assignment, across all catalogs and access packages.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e342-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e342-130">Request headers</span></span>
|<span data-ttu-id="4e342-131">名称</span><span class="sxs-lookup"><span data-stu-id="4e342-131">Name</span></span>|<span data-ttu-id="4e342-132">说明</span><span class="sxs-lookup"><span data-stu-id="4e342-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4e342-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e342-133">Authorization</span></span>|<span data-ttu-id="4e342-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e342-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e342-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e342-136">Request body</span></span>
<span data-ttu-id="4e342-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e342-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e342-138">响应</span><span class="sxs-lookup"><span data-stu-id="4e342-138">Response</span></span>

<span data-ttu-id="4e342-139">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignment](../resources/accesspackageassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="4e342-139">If successful, this method returns a `200 OK` response code and an [accessPackageAssignment](../resources/accesspackageassignment.md) collection in the response body.</span></span>

<span data-ttu-id="4e342-140">当结果集跨多个页面时，Microsoft Graph 返回该页面，该页面在响应中包含指向下一 `@odata.nextLink` 页结果的 URL 中的属性。</span><span class="sxs-lookup"><span data-stu-id="4e342-140">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="4e342-141">如果存在该属性，请继续使用每个响应中的 URL 提出其他请求， `@odata.nextLink` 直到返回所有结果。</span><span class="sxs-lookup"><span data-stu-id="4e342-141">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned.</span></span> <span data-ttu-id="4e342-142">有关详细信息，请参阅分页[Microsoft Graph应用中的数据](/graph/paging.md)。</span><span class="sxs-lookup"><span data-stu-id="4e342-142">For more information, see [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

## <a name="examples"></a><span data-ttu-id="4e342-143">示例</span><span class="sxs-lookup"><span data-stu-id="4e342-143">Examples</span></span>

<span data-ttu-id="4e342-144">以下示例获取针对已登录用户的访问包分配的状态。</span><span class="sxs-lookup"><span data-stu-id="4e342-144">The following example gets the status of access package assignments targeted for the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="4e342-145">请求</span><span class="sxs-lookup"><span data-stu-id="4e342-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4e342-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e342-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser(on='target')
```
# <a name="c"></a>[<span data-ttu-id="4e342-147">C#</span><span class="sxs-lookup"><span data-stu-id="4e342-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignment-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e342-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e342-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignment-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e342-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e342-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignment-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e342-150">Java</span><span class="sxs-lookup"><span data-stu-id="4e342-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignment-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4e342-151">响应</span><span class="sxs-lookup"><span data-stu-id="4e342-151">Response</span></span>
> <span data-ttu-id="4e342-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e342-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "5521fb4f-6a6c-410a-9191-461a65fd39d4",
            "catalogId": "34cfe9a8-88bc-4c82-b3d8-6b77d7035c33",
            "accessPackageId": "ca6992f8-e413-49a1-9619-c9819f4f73e0",
            "assignmentPolicyId": "7c6e6874-789e-4f11-b351-cc7b5883deef",
            "targetId": "2cb14f51-0108-41d8-89da-cd0e05e2c988",
            "assignmentStatus": "Delivered",
            "assignmentState": "Delivered",
            "isExtended": false,
            "expiredDateTime": null,
            "schedule": {
                "startDateTime": "2021-01-19T20:02:36.013Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": "2022-01-19T20:02:36.013Z",
                    "duration": null,
                    "type": "afterDateTime"
                }
            }
        }
  ]
}

```

