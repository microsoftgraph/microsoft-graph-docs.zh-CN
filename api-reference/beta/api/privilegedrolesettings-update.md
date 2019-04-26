---
title: 更新 privilegedRoleSettings
description: 更新给定角色设置的角色设置。 将返回一个 privilegedRoleSettings 对象。
localization_priority: Normal
ms.openlocfilehash: ce04a6e8c61c59f576d3a5e36592ba8ab4373de3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337250"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="9510f-104">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9510f-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9510f-105">更新给定角色设置的角色设置。</span><span class="sxs-lookup"><span data-stu-id="9510f-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="9510f-106">将返回一个[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9510f-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="9510f-107">权限</span><span class="sxs-lookup"><span data-stu-id="9510f-107">Permissions</span></span>

<span data-ttu-id="9510f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9510f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="9510f-110">**注意:** 请求者必须具有以下角色之一: 特权角色管理员、全局管理员、安全管理员或安全阅读者。</span><span class="sxs-lookup"><span data-stu-id="9510f-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="9510f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9510f-111">Permission type</span></span>      | <span data-ttu-id="9510f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9510f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9510f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9510f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9510f-114">PrivilegedAccess 的 AzureAD、directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="9510f-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9510f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9510f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9510f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9510f-116">Not supported.</span></span>    |
|<span data-ttu-id="9510f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9510f-117">Application</span></span> | <span data-ttu-id="9510f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9510f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9510f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9510f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="9510f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9510f-120">Request headers</span></span>
| <span data-ttu-id="9510f-121">名称</span><span class="sxs-lookup"><span data-stu-id="9510f-121">Name</span></span>      |<span data-ttu-id="9510f-122">说明</span><span class="sxs-lookup"><span data-stu-id="9510f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9510f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9510f-123">Authorization</span></span>  | <span data-ttu-id="9510f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9510f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9510f-126">Request body</span></span>
<span data-ttu-id="9510f-127">在请求正文中, 提供[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9510f-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="9510f-128">下表列出了在更新角色设置时可以提供的属性。</span><span class="sxs-lookup"><span data-stu-id="9510f-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="9510f-129">属性</span><span class="sxs-lookup"><span data-stu-id="9510f-129">Property</span></span>|<span data-ttu-id="9510f-130">类型</span><span class="sxs-lookup"><span data-stu-id="9510f-130">Type</span></span>|<span data-ttu-id="9510f-131">说明</span><span class="sxs-lookup"><span data-stu-id="9510f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9510f-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="9510f-132">elevationDuration</span></span>|<span data-ttu-id="9510f-133">duration</span><span class="sxs-lookup"><span data-stu-id="9510f-133">duration</span></span>|<span data-ttu-id="9510f-134">激活角色的持续时间。</span><span class="sxs-lookup"><span data-stu-id="9510f-134">The duration when the role is activated.</span></span> <span data-ttu-id="9510f-135">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-135">Required.</span></span>|
|<span data-ttu-id="9510f-136">id</span><span class="sxs-lookup"><span data-stu-id="9510f-136">id</span></span>|<span data-ttu-id="9510f-137">string</span><span class="sxs-lookup"><span data-stu-id="9510f-137">string</span></span>|<span data-ttu-id="9510f-138">角色设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9510f-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="9510f-139">只读。</span><span class="sxs-lookup"><span data-stu-id="9510f-139">Read-only.</span></span> <span data-ttu-id="9510f-140">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-140">Required.</span></span>|
|<span data-ttu-id="9510f-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="9510f-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="9510f-142">boolean</span><span class="sxs-lookup"><span data-stu-id="9510f-142">boolean</span></span>|<span data-ttu-id="9510f-143">如果 mfaOnElevation 是可配置的,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="9510f-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="9510f-144">**假**如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="9510f-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="9510f-145">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-145">Required.</span></span>|
|<span data-ttu-id="9510f-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="9510f-146">lastGlobalAdmin</span></span>|<span data-ttu-id="9510f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="9510f-147">Boolean</span></span>|<span data-ttu-id="9510f-148">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="9510f-148">For internal use only.</span></span>|
|<span data-ttu-id="9510f-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="9510f-149">maxElavationDuration</span></span>|<span data-ttu-id="9510f-150">duration</span><span class="sxs-lookup"><span data-stu-id="9510f-150">duration</span></span>|<span data-ttu-id="9510f-151">已激活角色的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="9510f-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="9510f-152">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-152">Required.</span></span>|
|<span data-ttu-id="9510f-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="9510f-153">mfaOnElevation</span></span>|<span data-ttu-id="9510f-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="9510f-154">Boolean</span></span>|<span data-ttu-id="9510f-155">如果需要 MFA 以激活角色,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="9510f-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="9510f-156">**假**如果无需进行 MFA 即可激活角色。</span><span class="sxs-lookup"><span data-stu-id="9510f-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="9510f-157">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-157">Required.</span></span>|
|<span data-ttu-id="9510f-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="9510f-158">minElevationDuration</span></span>|<span data-ttu-id="9510f-159">duration</span><span class="sxs-lookup"><span data-stu-id="9510f-159">duration</span></span>|<span data-ttu-id="9510f-160">已激活角色的最小持续时间。</span><span class="sxs-lookup"><span data-stu-id="9510f-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="9510f-161">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-161">Required.</span></span>|
|<span data-ttu-id="9510f-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="9510f-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="9510f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9510f-163">Boolean</span></span>|<span data-ttu-id="9510f-164">如果激活角色时向最终用户发送通知,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="9510f-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="9510f-165">**假**如果在角色激活时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="9510f-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="9510f-166">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-166">Required.</span></span>|
|<span data-ttu-id="9510f-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="9510f-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="9510f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="9510f-168">Boolean</span></span>|<span data-ttu-id="9510f-169">如果激活角色时需要票证信息,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="9510f-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="9510f-170">**假**如果激活角色时不需要票证信息。</span><span class="sxs-lookup"><span data-stu-id="9510f-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="9510f-171">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-171">Required.</span></span>|
|<span data-ttu-id="9510f-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="9510f-172">approvalOnElevation</span></span>|<span data-ttu-id="9510f-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="9510f-173">Boolean</span></span>|<span data-ttu-id="9510f-174">如果激活角色时需要进行审批,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="9510f-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="9510f-175">**假**如果激活该角色时不需要审批。</span><span class="sxs-lookup"><span data-stu-id="9510f-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="9510f-176">必需。</span><span class="sxs-lookup"><span data-stu-id="9510f-176">Required.</span></span>|
|<span data-ttu-id="9510f-177">approverIds</span><span class="sxs-lookup"><span data-stu-id="9510f-177">approverIds</span></span>|<span data-ttu-id="9510f-178">字符串集合</span><span class="sxs-lookup"><span data-stu-id="9510f-178">string collection</span></span>|<span data-ttu-id="9510f-179">审批 id 的列表 (如果激活需要审批)。</span><span class="sxs-lookup"><span data-stu-id="9510f-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="9510f-180">响应</span><span class="sxs-lookup"><span data-stu-id="9510f-180">Response</span></span>

<span data-ttu-id="9510f-181">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9510f-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="9510f-182">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="9510f-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9510f-183">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="9510f-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="9510f-184">示例</span><span class="sxs-lookup"><span data-stu-id="9510f-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9510f-185">请求</span><span class="sxs-lookup"><span data-stu-id="9510f-185">Request</span></span>
<span data-ttu-id="9510f-186">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9510f-186">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9510f-187">响应</span><span class="sxs-lookup"><span data-stu-id="9510f-187">Response</span></span>
<span data-ttu-id="9510f-188">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9510f-188">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->
