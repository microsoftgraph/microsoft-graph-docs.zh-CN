---
title: 创建 vppToken
description: 创建新的 vppToken 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55498d2257758e4ba52bbf334db2b06512aeff33
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620274"
---
# <a name="create-vpptoken"></a><span data-ttu-id="05331-103">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="05331-103">Create vppToken</span></span>

> <span data-ttu-id="05331-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05331-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05331-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05331-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05331-106">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05331-106">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05331-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="05331-107">Prerequisites</span></span>
<span data-ttu-id="05331-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05331-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="05331-110">Permission type</span></span>|<span data-ttu-id="05331-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05331-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05331-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05331-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05331-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05331-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="05331-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05331-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05331-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="05331-115">Not supported.</span></span>|
|<span data-ttu-id="05331-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="05331-116">Application</span></span>|<span data-ttu-id="05331-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="05331-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05331-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05331-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="05331-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="05331-119">Request headers</span></span>
|<span data-ttu-id="05331-120">标头</span><span class="sxs-lookup"><span data-stu-id="05331-120">Header</span></span>|<span data-ttu-id="05331-121">值</span><span class="sxs-lookup"><span data-stu-id="05331-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05331-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05331-122">Authorization</span></span>|<span data-ttu-id="05331-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05331-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05331-124">接受</span><span class="sxs-lookup"><span data-stu-id="05331-124">Accept</span></span>|<span data-ttu-id="05331-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05331-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05331-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="05331-126">Request body</span></span>
<span data-ttu-id="05331-127">在请求正文中，提供 vppToken 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05331-127">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="05331-128">下表显示创建 vppToken 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="05331-128">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="05331-129">属性</span><span class="sxs-lookup"><span data-stu-id="05331-129">Property</span></span>|<span data-ttu-id="05331-130">类型</span><span class="sxs-lookup"><span data-stu-id="05331-130">Type</span></span>|<span data-ttu-id="05331-131">说明</span><span class="sxs-lookup"><span data-stu-id="05331-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05331-132">id</span><span class="sxs-lookup"><span data-stu-id="05331-132">id</span></span>|<span data-ttu-id="05331-133">String</span><span class="sxs-lookup"><span data-stu-id="05331-133">String</span></span>|<span data-ttu-id="05331-134">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="05331-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="05331-135">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="05331-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="05331-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="05331-136">organizationName</span></span>|<span data-ttu-id="05331-137">String</span><span class="sxs-lookup"><span data-stu-id="05331-137">String</span></span>|<span data-ttu-id="05331-138">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="05331-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="05331-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="05331-139">vppTokenAccountType</span></span>|[<span data-ttu-id="05331-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="05331-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="05331-141">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="05331-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="05331-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="05331-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="05331-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="05331-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="05331-144">appleId</span><span class="sxs-lookup"><span data-stu-id="05331-144">appleId</span></span>|<span data-ttu-id="05331-145">String</span><span class="sxs-lookup"><span data-stu-id="05331-145">String</span></span>|<span data-ttu-id="05331-146">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="05331-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="05331-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="05331-147">expirationDateTime</span></span>|<span data-ttu-id="05331-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05331-148">DateTimeOffset</span></span>|<span data-ttu-id="05331-149">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="05331-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="05331-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="05331-150">lastSyncDateTime</span></span>|<span data-ttu-id="05331-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05331-151">DateTimeOffset</span></span>|<span data-ttu-id="05331-152">上次使用 Apple Volume purchase program 服务 (apple Volume purchase program 令牌) 完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="05331-152">The last time when an application sync was done with the Apple volume purchase program service using the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="05331-153">token</span><span class="sxs-lookup"><span data-stu-id="05331-153">token</span></span>|<span data-ttu-id="05331-154">String</span><span class="sxs-lookup"><span data-stu-id="05331-154">String</span></span>|<span data-ttu-id="05331-155">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="05331-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="05331-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05331-156">lastModifiedDateTime</span></span>|<span data-ttu-id="05331-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05331-157">DateTimeOffset</span></span>|<span data-ttu-id="05331-158">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="05331-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="05331-159">state</span><span class="sxs-lookup"><span data-stu-id="05331-159">state</span></span>|[<span data-ttu-id="05331-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="05331-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="05331-161">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="05331-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="05331-162">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="05331-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="05331-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="05331-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="05331-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="05331-164">tokenActionResults</span></span>|<span data-ttu-id="05331-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="05331-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="05331-166">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="05331-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="05331-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="05331-167">lastSyncStatus</span></span>|[<span data-ttu-id="05331-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="05331-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="05331-169">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="05331-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="05331-170">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="05331-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="05331-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="05331-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="05331-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="05331-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="05331-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="05331-173">Boolean</span></span>|<span data-ttu-id="05331-174">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="05331-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="05331-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="05331-175">countryOrRegion</span></span>|<span data-ttu-id="05331-176">String</span><span class="sxs-lookup"><span data-stu-id="05331-176">String</span></span>|<span data-ttu-id="05331-177">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="05331-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="05331-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="05331-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="05331-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="05331-179">Boolean</span></span>|<span data-ttu-id="05331-180">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="05331-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="05331-181">displayName</span><span class="sxs-lookup"><span data-stu-id="05331-181">displayName</span></span>|<span data-ttu-id="05331-182">String</span><span class="sxs-lookup"><span data-stu-id="05331-182">String</span></span>|<span data-ttu-id="05331-183">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="05331-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="05331-184">locationName</span><span class="sxs-lookup"><span data-stu-id="05331-184">locationName</span></span>|<span data-ttu-id="05331-185">String</span><span class="sxs-lookup"><span data-stu-id="05331-185">String</span></span>|<span data-ttu-id="05331-186">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="05331-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="05331-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="05331-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="05331-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="05331-188">Boolean</span></span>|<span data-ttu-id="05331-189">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="05331-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="05331-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="05331-190">roleScopeTagIds</span></span>|<span data-ttu-id="05331-191">String collection</span><span class="sxs-lookup"><span data-stu-id="05331-191">String collection</span></span>|<span data-ttu-id="05331-192">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="05331-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="05331-193">响应</span><span class="sxs-lookup"><span data-stu-id="05331-193">Response</span></span>
<span data-ttu-id="05331-194">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05331-194">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05331-195">示例</span><span class="sxs-lookup"><span data-stu-id="05331-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="05331-196">请求</span><span class="sxs-lookup"><span data-stu-id="05331-196">Request</span></span>
<span data-ttu-id="05331-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05331-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05331-198">响应</span><span class="sxs-lookup"><span data-stu-id="05331-198">Response</span></span>
<span data-ttu-id="05331-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05331-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





