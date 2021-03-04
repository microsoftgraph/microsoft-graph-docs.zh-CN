---
title: 更新 privilegedRoleSettings
description: 更新给定角色设置的角色设置。 将返回 privilegedRoleSettings 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 80797ba6965cade1625f6cc46abaf3f9fcbfadd2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441100"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="7d68a-104">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="7d68a-104">Update privilegedRoleSettings</span></span>

<span data-ttu-id="7d68a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d68a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d68a-106">更新给定角色设置的角色设置。</span><span class="sxs-lookup"><span data-stu-id="7d68a-106">Update the role settings for the given role setting.</span></span> <span data-ttu-id="7d68a-107">将 [返回 privilegedRoleSettings](../resources/privilegedrolesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d68a-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d68a-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="7d68a-108">Permissions</span></span>

<span data-ttu-id="7d68a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d68a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="7d68a-111">**注意：** 请求者必须具有 Privileged Role Administrator 角色才能更新角色设置。</span><span class="sxs-lookup"><span data-stu-id="7d68a-111">**Note:** The requester must have the Privileged Role Administrator role to update role settings.</span></span> 

|<span data-ttu-id="7d68a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d68a-112">Permission type</span></span>      | <span data-ttu-id="7d68a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d68a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d68a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d68a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7d68a-115">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d68a-115">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d68a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d68a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d68a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d68a-117">Not supported.</span></span>    |
|<span data-ttu-id="7d68a-118">Application</span><span class="sxs-lookup"><span data-stu-id="7d68a-118">Application</span></span> | <span data-ttu-id="7d68a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d68a-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d68a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d68a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="7d68a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d68a-121">Request headers</span></span>
| <span data-ttu-id="7d68a-122">名称</span><span class="sxs-lookup"><span data-stu-id="7d68a-122">Name</span></span>      |<span data-ttu-id="7d68a-123">说明</span><span class="sxs-lookup"><span data-stu-id="7d68a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d68a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d68a-124">Authorization</span></span>  | <span data-ttu-id="7d68a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d68a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d68a-127">Request body</span></span>
<span data-ttu-id="7d68a-128">在请求正文中，提供 [privilegedRoleSettings](../resources/privilegedrolesettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d68a-128">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="7d68a-129">下表列出了可在更新角色设置时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="7d68a-129">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="7d68a-130">属性</span><span class="sxs-lookup"><span data-stu-id="7d68a-130">Property</span></span>|<span data-ttu-id="7d68a-131">类型</span><span class="sxs-lookup"><span data-stu-id="7d68a-131">Type</span></span>|<span data-ttu-id="7d68a-132">说明</span><span class="sxs-lookup"><span data-stu-id="7d68a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d68a-133">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="7d68a-133">elevationDuration</span></span>|<span data-ttu-id="7d68a-134">duration</span><span class="sxs-lookup"><span data-stu-id="7d68a-134">duration</span></span>|<span data-ttu-id="7d68a-135">激活角色的持续时间。</span><span class="sxs-lookup"><span data-stu-id="7d68a-135">The duration when the role is activated.</span></span> <span data-ttu-id="7d68a-136">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-136">Required.</span></span>|
|<span data-ttu-id="7d68a-137">id</span><span class="sxs-lookup"><span data-stu-id="7d68a-137">id</span></span>|<span data-ttu-id="7d68a-138">string</span><span class="sxs-lookup"><span data-stu-id="7d68a-138">string</span></span>|<span data-ttu-id="7d68a-139">角色设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7d68a-139">The unique identifier for the role settings.</span></span> <span data-ttu-id="7d68a-140">只读。</span><span class="sxs-lookup"><span data-stu-id="7d68a-140">Read-only.</span></span> <span data-ttu-id="7d68a-141">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-141">Required.</span></span>|
|<span data-ttu-id="7d68a-142">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="7d68a-142">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="7d68a-143">boolean</span><span class="sxs-lookup"><span data-stu-id="7d68a-143">boolean</span></span>|<span data-ttu-id="7d68a-144">**如此** 如果 mfaOnElevation 是可配置的。</span><span class="sxs-lookup"><span data-stu-id="7d68a-144">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="7d68a-145">**假** 如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="7d68a-145">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="7d68a-146">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-146">Required.</span></span>|
|<span data-ttu-id="7d68a-147">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="7d68a-147">lastGlobalAdmin</span></span>|<span data-ttu-id="7d68a-148">布尔</span><span class="sxs-lookup"><span data-stu-id="7d68a-148">Boolean</span></span>|<span data-ttu-id="7d68a-149">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="7d68a-149">For internal use only.</span></span>|
|<span data-ttu-id="7d68a-150">maxEationDuration</span><span class="sxs-lookup"><span data-stu-id="7d68a-150">maxElavationDuration</span></span>|<span data-ttu-id="7d68a-151">duration</span><span class="sxs-lookup"><span data-stu-id="7d68a-151">duration</span></span>|<span data-ttu-id="7d68a-152">已激活角色的最大持续时间。</span><span class="sxs-lookup"><span data-stu-id="7d68a-152">Maximum duration for the activated role.</span></span> <span data-ttu-id="7d68a-153">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-153">Required.</span></span>|
|<span data-ttu-id="7d68a-154">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="7d68a-154">mfaOnElevation</span></span>|<span data-ttu-id="7d68a-155">布尔</span><span class="sxs-lookup"><span data-stu-id="7d68a-155">Boolean</span></span>|<span data-ttu-id="7d68a-156">**如果** 激活角色需要 MFA，则其为 true。</span><span class="sxs-lookup"><span data-stu-id="7d68a-156">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="7d68a-157">**假** 如果不需要 MFA 即可激活角色。</span><span class="sxs-lookup"><span data-stu-id="7d68a-157">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="7d68a-158">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-158">Required.</span></span>|
|<span data-ttu-id="7d68a-159">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="7d68a-159">minElevationDuration</span></span>|<span data-ttu-id="7d68a-160">duration</span><span class="sxs-lookup"><span data-stu-id="7d68a-160">duration</span></span>|<span data-ttu-id="7d68a-161">已激活角色的最小持续时间。</span><span class="sxs-lookup"><span data-stu-id="7d68a-161">Minimum duration for the activated role.</span></span> <span data-ttu-id="7d68a-162">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-162">Required.</span></span>|
|<span data-ttu-id="7d68a-163">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="7d68a-163">notificationToUserOnElevation</span></span>|<span data-ttu-id="7d68a-164">布尔</span><span class="sxs-lookup"><span data-stu-id="7d68a-164">Boolean</span></span>|<span data-ttu-id="7d68a-165">**如此** 如果激活角色时向最终用户发送通知。</span><span class="sxs-lookup"><span data-stu-id="7d68a-165">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="7d68a-166">**假** 如果激活角色时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="7d68a-166">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="7d68a-167">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-167">Required.</span></span>|
|<span data-ttu-id="7d68a-168">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="7d68a-168">ticketingInfoOnElevation</span></span>|<span data-ttu-id="7d68a-169">布尔</span><span class="sxs-lookup"><span data-stu-id="7d68a-169">Boolean</span></span>|<span data-ttu-id="7d68a-170">**如此** 如果激活角色时需要票证信息。</span><span class="sxs-lookup"><span data-stu-id="7d68a-170">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="7d68a-171">**假** 如果激活角色时不需要票证信息。</span><span class="sxs-lookup"><span data-stu-id="7d68a-171">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="7d68a-172">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-172">Required.</span></span>|
|<span data-ttu-id="7d68a-173">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="7d68a-173">approvalOnElevation</span></span>|<span data-ttu-id="7d68a-174">布尔</span><span class="sxs-lookup"><span data-stu-id="7d68a-174">Boolean</span></span>|<span data-ttu-id="7d68a-175">**如此** 如果激活角色时需要审批。</span><span class="sxs-lookup"><span data-stu-id="7d68a-175">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="7d68a-176">**假** 如果激活角色时不需要审批。</span><span class="sxs-lookup"><span data-stu-id="7d68a-176">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="7d68a-177">必需。</span><span class="sxs-lookup"><span data-stu-id="7d68a-177">Required.</span></span>|
|<span data-ttu-id="7d68a-178">approverIds</span><span class="sxs-lookup"><span data-stu-id="7d68a-178">approverIds</span></span>|<span data-ttu-id="7d68a-179">string 集合</span><span class="sxs-lookup"><span data-stu-id="7d68a-179">string collection</span></span>|<span data-ttu-id="7d68a-180">审批 ID 列表（如果需要审批才能激活）。</span><span class="sxs-lookup"><span data-stu-id="7d68a-180">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="7d68a-181">响应</span><span class="sxs-lookup"><span data-stu-id="7d68a-181">Response</span></span>

<span data-ttu-id="7d68a-182">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7d68a-182">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="7d68a-183">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="7d68a-183">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7d68a-184">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="7d68a-184">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="7d68a-185">示例</span><span class="sxs-lookup"><span data-stu-id="7d68a-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d68a-186">请求</span><span class="sxs-lookup"><span data-stu-id="7d68a-186">Request</span></span>
<span data-ttu-id="7d68a-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d68a-187">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d68a-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d68a-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
# <a name="c"></a>[<span data-ttu-id="7d68a-189">C#</span><span class="sxs-lookup"><span data-stu-id="7d68a-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d68a-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d68a-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d68a-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d68a-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d68a-192">Java</span><span class="sxs-lookup"><span data-stu-id="7d68a-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7d68a-193">响应</span><span class="sxs-lookup"><span data-stu-id="7d68a-193">Response</span></span>
<span data-ttu-id="7d68a-194">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7d68a-194">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


