---
title: 更新 privilegedRoleSettings
description: 更新给定的角色设置的角色设置。 将返回一个 privilegedRoleSettings 对象。
ms.openlocfilehash: 0e0f6b7253a1c1d8570c0b91fac4b08bbd39dfff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048708"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="cccb4-104">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="cccb4-104">Update privilegedRoleSettings</span></span>

> <span data-ttu-id="cccb4-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cccb4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cccb4-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cccb4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cccb4-107">更新给定的角色设置的角色设置。</span><span class="sxs-lookup"><span data-stu-id="cccb4-107">Update the role settings for the given role setting.</span></span> <span data-ttu-id="cccb4-108">将返回一个[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cccb4-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="cccb4-109">权限</span><span class="sxs-lookup"><span data-stu-id="cccb4-109">Permissions</span></span>

<span data-ttu-id="cccb4-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cccb4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="cccb4-112">**注意：** 请求者必须具有以下角色之一： 具有权限的角色管理员、 全局管理员、 安全管理员或安全读取器。</span><span class="sxs-lookup"><span data-stu-id="cccb4-112">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="cccb4-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="cccb4-113">Permission type</span></span>      | <span data-ttu-id="cccb4-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cccb4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cccb4-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cccb4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="cccb4-116">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cccb4-116">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cccb4-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cccb4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cccb4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cccb4-118">Not supported.</span></span>    |
|<span data-ttu-id="cccb4-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="cccb4-119">Application</span></span> | <span data-ttu-id="cccb4-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="cccb4-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cccb4-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cccb4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="cccb4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="cccb4-122">Request headers</span></span>
| <span data-ttu-id="cccb4-123">名称</span><span class="sxs-lookup"><span data-stu-id="cccb4-123">Name</span></span>      |<span data-ttu-id="cccb4-124">说明</span><span class="sxs-lookup"><span data-stu-id="cccb4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cccb4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cccb4-125">Authorization</span></span>  | <span data-ttu-id="cccb4-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cccb4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cccb4-128">Request body</span></span>
<span data-ttu-id="cccb4-129">在请求正文中，提供[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cccb4-129">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="cccb4-130">下表列出更新角色设置时可以提供的属性。</span><span class="sxs-lookup"><span data-stu-id="cccb4-130">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="cccb4-131">属性</span><span class="sxs-lookup"><span data-stu-id="cccb4-131">Property</span></span>|<span data-ttu-id="cccb4-132">类型</span><span class="sxs-lookup"><span data-stu-id="cccb4-132">Type</span></span>|<span data-ttu-id="cccb4-133">说明</span><span class="sxs-lookup"><span data-stu-id="cccb4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cccb4-134">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="cccb4-134">elevationDuration</span></span>|<span data-ttu-id="cccb4-135">duration</span><span class="sxs-lookup"><span data-stu-id="cccb4-135">duration</span></span>|<span data-ttu-id="cccb4-136">当激活角色持续时间。</span><span class="sxs-lookup"><span data-stu-id="cccb4-136">The duration when the role is activated.</span></span> <span data-ttu-id="cccb4-137">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-137">Required.</span></span>|
|<span data-ttu-id="cccb4-138">id</span><span class="sxs-lookup"><span data-stu-id="cccb4-138">id</span></span>|<span data-ttu-id="cccb4-139">string</span><span class="sxs-lookup"><span data-stu-id="cccb4-139">string</span></span>|<span data-ttu-id="cccb4-140">角色设置唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb4-140">The unique identifier for the role settings.</span></span> <span data-ttu-id="cccb4-141">只读。</span><span class="sxs-lookup"><span data-stu-id="cccb4-141">Read-only.</span></span> <span data-ttu-id="cccb4-142">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-142">Required.</span></span>|
|<span data-ttu-id="cccb4-143">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="cccb4-143">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="cccb4-144">boolean</span><span class="sxs-lookup"><span data-stu-id="cccb4-144">boolean</span></span>|<span data-ttu-id="cccb4-145">**true**如果 mfaOnElevation 可配置。</span><span class="sxs-lookup"><span data-stu-id="cccb4-145">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="cccb4-146">**false**如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="cccb4-146">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="cccb4-147">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-147">Required.</span></span>|
|<span data-ttu-id="cccb4-148">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="cccb4-148">lastGlobalAdmin</span></span>|<span data-ttu-id="cccb4-149">布尔</span><span class="sxs-lookup"><span data-stu-id="cccb4-149">Boolean</span></span>|<span data-ttu-id="cccb4-150">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="cccb4-150">For internal use only.</span></span>|
|<span data-ttu-id="cccb4-151">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="cccb4-151">maxElavationDuration</span></span>|<span data-ttu-id="cccb4-152">duration</span><span class="sxs-lookup"><span data-stu-id="cccb4-152">duration</span></span>|<span data-ttu-id="cccb4-153">激活角色的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="cccb4-153">Maximum duration for the activated role.</span></span> <span data-ttu-id="cccb4-154">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-154">Required.</span></span>|
|<span data-ttu-id="cccb4-155">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="cccb4-155">mfaOnElevation</span></span>|<span data-ttu-id="cccb4-156">布尔</span><span class="sxs-lookup"><span data-stu-id="cccb4-156">Boolean</span></span>|<span data-ttu-id="cccb4-157">如果为**true** MFA 需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="cccb4-157">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="cccb4-158">**false**如果 MFA 不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="cccb4-158">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="cccb4-159">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-159">Required.</span></span>|
|<span data-ttu-id="cccb4-160">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="cccb4-160">minElevationDuration</span></span>|<span data-ttu-id="cccb4-161">duration</span><span class="sxs-lookup"><span data-stu-id="cccb4-161">duration</span></span>|<span data-ttu-id="cccb4-162">激活角色的最低持续时间。</span><span class="sxs-lookup"><span data-stu-id="cccb4-162">Minimum duration for the activated role.</span></span> <span data-ttu-id="cccb4-163">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-163">Required.</span></span>|
|<span data-ttu-id="cccb4-164">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="cccb4-164">notificationToUserOnElevation</span></span>|<span data-ttu-id="cccb4-165">布尔</span><span class="sxs-lookup"><span data-stu-id="cccb4-165">Boolean</span></span>|<span data-ttu-id="cccb4-166">**true**如果角色激活时向最终用户发送通知。</span><span class="sxs-lookup"><span data-stu-id="cccb4-166">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="cccb4-167">**false**如果角色被激活时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="cccb4-167">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="cccb4-168">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-168">Required.</span></span>|
|<span data-ttu-id="cccb4-169">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="cccb4-169">ticketingInfoOnElevation</span></span>|<span data-ttu-id="cccb4-170">布尔</span><span class="sxs-lookup"><span data-stu-id="cccb4-170">Boolean</span></span>|<span data-ttu-id="cccb4-171">如果为**true**时，票证信息是必需激活角色。</span><span class="sxs-lookup"><span data-stu-id="cccb4-171">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="cccb4-172">**false**如果票证信息不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="cccb4-172">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="cccb4-173">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-173">Required.</span></span>|
|<span data-ttu-id="cccb4-174">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="cccb4-174">approvalOnElevation</span></span>|<span data-ttu-id="cccb4-175">布尔</span><span class="sxs-lookup"><span data-stu-id="cccb4-175">Boolean</span></span>|<span data-ttu-id="cccb4-176">**true**如果情况下审批，需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="cccb4-176">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="cccb4-177">**false**如果审批不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="cccb4-177">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="cccb4-178">必需。</span><span class="sxs-lookup"><span data-stu-id="cccb4-178">Required.</span></span>|
|<span data-ttu-id="cccb4-179">approverIds</span><span class="sxs-lookup"><span data-stu-id="cccb4-179">approverIds</span></span>|<span data-ttu-id="cccb4-180">array</span><span class="sxs-lookup"><span data-stu-id="cccb4-180">array</span></span>|<span data-ttu-id="cccb4-181">审批 Id，如果需要激活审核的列表。</span><span class="sxs-lookup"><span data-stu-id="cccb4-181">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="cccb4-182">响应</span><span class="sxs-lookup"><span data-stu-id="cccb4-182">Response</span></span>

<span data-ttu-id="cccb4-183">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cccb4-183">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="cccb4-184">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="cccb4-184">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cccb4-185">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="cccb4-185">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="cccb4-186">示例</span><span class="sxs-lookup"><span data-stu-id="cccb4-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cccb4-187">请求</span><span class="sxs-lookup"><span data-stu-id="cccb4-187">Request</span></span>
<span data-ttu-id="cccb4-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cccb4-188">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="cccb4-189">响应</span><span class="sxs-lookup"><span data-stu-id="cccb4-189">Response</span></span>
<span data-ttu-id="cccb4-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cccb4-190">Here is an example of the response.</span></span>

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
