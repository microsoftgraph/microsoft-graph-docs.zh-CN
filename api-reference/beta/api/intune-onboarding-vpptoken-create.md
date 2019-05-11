---
title: 创建 vppToken
description: 创建新的 vppToken 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ecb914d14a70950dd1128001333a6a94c7b5150
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899807"
---
# <a name="create-vpptoken"></a><span data-ttu-id="742fa-103">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="742fa-103">Create vppToken</span></span>

> <span data-ttu-id="742fa-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="742fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="742fa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="742fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="742fa-106">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="742fa-106">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="742fa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="742fa-107">Prerequisites</span></span>
<span data-ttu-id="742fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="742fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="742fa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="742fa-110">Permission type</span></span>|<span data-ttu-id="742fa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="742fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="742fa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="742fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="742fa-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="742fa-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="742fa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="742fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="742fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="742fa-115">Not supported.</span></span>|
|<span data-ttu-id="742fa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="742fa-116">Application</span></span>|<span data-ttu-id="742fa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="742fa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="742fa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="742fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="742fa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="742fa-119">Request headers</span></span>
|<span data-ttu-id="742fa-120">标头</span><span class="sxs-lookup"><span data-stu-id="742fa-120">Header</span></span>|<span data-ttu-id="742fa-121">值</span><span class="sxs-lookup"><span data-stu-id="742fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="742fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="742fa-122">Authorization</span></span>|<span data-ttu-id="742fa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="742fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="742fa-124">接受</span><span class="sxs-lookup"><span data-stu-id="742fa-124">Accept</span></span>|<span data-ttu-id="742fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="742fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="742fa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="742fa-126">Request body</span></span>
<span data-ttu-id="742fa-127">在请求正文中，提供 vppToken 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="742fa-127">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="742fa-128">下表显示创建 vppToken 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="742fa-128">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="742fa-129">属性</span><span class="sxs-lookup"><span data-stu-id="742fa-129">Property</span></span>|<span data-ttu-id="742fa-130">类型</span><span class="sxs-lookup"><span data-stu-id="742fa-130">Type</span></span>|<span data-ttu-id="742fa-131">说明</span><span class="sxs-lookup"><span data-stu-id="742fa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="742fa-132">id</span><span class="sxs-lookup"><span data-stu-id="742fa-132">id</span></span>|<span data-ttu-id="742fa-133">String</span><span class="sxs-lookup"><span data-stu-id="742fa-133">String</span></span>|<span data-ttu-id="742fa-134">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="742fa-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="742fa-135">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="742fa-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="742fa-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="742fa-136">organizationName</span></span>|<span data-ttu-id="742fa-137">String</span><span class="sxs-lookup"><span data-stu-id="742fa-137">String</span></span>|<span data-ttu-id="742fa-138">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="742fa-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="742fa-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="742fa-139">vppTokenAccountType</span></span>|[<span data-ttu-id="742fa-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="742fa-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="742fa-141">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="742fa-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="742fa-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="742fa-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="742fa-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="742fa-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="742fa-144">appleId</span><span class="sxs-lookup"><span data-stu-id="742fa-144">appleId</span></span>|<span data-ttu-id="742fa-145">String</span><span class="sxs-lookup"><span data-stu-id="742fa-145">String</span></span>|<span data-ttu-id="742fa-146">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="742fa-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="742fa-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="742fa-147">expirationDateTime</span></span>|<span data-ttu-id="742fa-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="742fa-148">DateTimeOffset</span></span>|<span data-ttu-id="742fa-149">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="742fa-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="742fa-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="742fa-150">lastSyncDateTime</span></span>|<span data-ttu-id="742fa-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="742fa-151">DateTimeOffset</span></span>|<span data-ttu-id="742fa-152">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="742fa-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="742fa-153">token</span><span class="sxs-lookup"><span data-stu-id="742fa-153">token</span></span>|<span data-ttu-id="742fa-154">String</span><span class="sxs-lookup"><span data-stu-id="742fa-154">String</span></span>|<span data-ttu-id="742fa-155">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="742fa-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="742fa-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="742fa-156">lastModifiedDateTime</span></span>|<span data-ttu-id="742fa-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="742fa-157">DateTimeOffset</span></span>|<span data-ttu-id="742fa-158">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="742fa-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="742fa-159">state</span><span class="sxs-lookup"><span data-stu-id="742fa-159">state</span></span>|[<span data-ttu-id="742fa-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="742fa-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="742fa-161">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="742fa-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="742fa-162">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="742fa-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="742fa-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="742fa-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="742fa-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="742fa-164">tokenActionResults</span></span>|<span data-ttu-id="742fa-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="742fa-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="742fa-166">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="742fa-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="742fa-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="742fa-167">lastSyncStatus</span></span>|[<span data-ttu-id="742fa-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="742fa-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="742fa-169">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="742fa-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="742fa-170">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="742fa-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="742fa-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="742fa-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="742fa-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="742fa-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="742fa-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="742fa-173">Boolean</span></span>|<span data-ttu-id="742fa-174">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="742fa-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="742fa-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="742fa-175">countryOrRegion</span></span>|<span data-ttu-id="742fa-176">String</span><span class="sxs-lookup"><span data-stu-id="742fa-176">String</span></span>|<span data-ttu-id="742fa-177">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="742fa-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="742fa-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="742fa-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="742fa-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="742fa-179">Boolean</span></span>|<span data-ttu-id="742fa-180">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="742fa-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="742fa-181">displayName</span><span class="sxs-lookup"><span data-stu-id="742fa-181">displayName</span></span>|<span data-ttu-id="742fa-182">String</span><span class="sxs-lookup"><span data-stu-id="742fa-182">String</span></span>|<span data-ttu-id="742fa-183">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="742fa-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="742fa-184">locationName</span><span class="sxs-lookup"><span data-stu-id="742fa-184">locationName</span></span>|<span data-ttu-id="742fa-185">String</span><span class="sxs-lookup"><span data-stu-id="742fa-185">String</span></span>|<span data-ttu-id="742fa-186">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="742fa-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="742fa-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="742fa-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="742fa-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="742fa-188">Boolean</span></span>|<span data-ttu-id="742fa-189">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="742fa-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="742fa-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="742fa-190">roleScopeTagIds</span></span>|<span data-ttu-id="742fa-191">String collection</span><span class="sxs-lookup"><span data-stu-id="742fa-191">String collection</span></span>|<span data-ttu-id="742fa-192">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="742fa-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="742fa-193">响应</span><span class="sxs-lookup"><span data-stu-id="742fa-193">Response</span></span>
<span data-ttu-id="742fa-194">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="742fa-194">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="742fa-195">示例</span><span class="sxs-lookup"><span data-stu-id="742fa-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="742fa-196">请求</span><span class="sxs-lookup"><span data-stu-id="742fa-196">Request</span></span>
<span data-ttu-id="742fa-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="742fa-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="742fa-198">响应</span><span class="sxs-lookup"><span data-stu-id="742fa-198">Response</span></span>
<span data-ttu-id="742fa-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="742fa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1115

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




