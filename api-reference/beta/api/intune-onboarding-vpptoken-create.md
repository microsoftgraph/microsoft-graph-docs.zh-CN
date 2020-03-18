---
title: 创建 vppToken
description: 创建新的 vppToken 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75f8715e1a1358365551c9a4ddfbcca7d10116ec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802697"
---
# <a name="create-vpptoken"></a><span data-ttu-id="4dd5e-103">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="4dd5e-103">Create vppToken</span></span>

> <span data-ttu-id="4dd5e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dd5e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dd5e-106">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-106">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dd5e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4dd5e-107">Prerequisites</span></span>
<span data-ttu-id="4dd5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dd5e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dd5e-110">Permission type</span></span>|<span data-ttu-id="4dd5e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4dd5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dd5e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dd5e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dd5e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4dd5e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dd5e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-115">Not supported.</span></span>|
|<span data-ttu-id="4dd5e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dd5e-116">Application</span></span>|<span data-ttu-id="4dd5e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dd5e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dd5e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dd5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="4dd5e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dd5e-119">Request headers</span></span>
|<span data-ttu-id="4dd5e-120">标头</span><span class="sxs-lookup"><span data-stu-id="4dd5e-120">Header</span></span>|<span data-ttu-id="4dd5e-121">值</span><span class="sxs-lookup"><span data-stu-id="4dd5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dd5e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dd5e-122">Authorization</span></span>|<span data-ttu-id="4dd5e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dd5e-124">接受</span><span class="sxs-lookup"><span data-stu-id="4dd5e-124">Accept</span></span>|<span data-ttu-id="4dd5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dd5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dd5e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dd5e-126">Request body</span></span>
<span data-ttu-id="4dd5e-127">在请求正文中，提供 vppToken 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-127">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="4dd5e-128">下表显示创建 vppToken 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-128">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="4dd5e-129">属性</span><span class="sxs-lookup"><span data-stu-id="4dd5e-129">Property</span></span>|<span data-ttu-id="4dd5e-130">类型</span><span class="sxs-lookup"><span data-stu-id="4dd5e-130">Type</span></span>|<span data-ttu-id="4dd5e-131">说明</span><span class="sxs-lookup"><span data-stu-id="4dd5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dd5e-132">id</span><span class="sxs-lookup"><span data-stu-id="4dd5e-132">id</span></span>|<span data-ttu-id="4dd5e-133">String</span><span class="sxs-lookup"><span data-stu-id="4dd5e-133">String</span></span>|<span data-ttu-id="4dd5e-134">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="4dd5e-135">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="4dd5e-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="4dd5e-136">organizationName</span></span>|<span data-ttu-id="4dd5e-137">String</span><span class="sxs-lookup"><span data-stu-id="4dd5e-137">String</span></span>|<span data-ttu-id="4dd5e-138">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="4dd5e-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="4dd5e-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="4dd5e-139">vppTokenAccountType</span></span>|[<span data-ttu-id="4dd5e-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="4dd5e-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="4dd5e-141">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="4dd5e-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="4dd5e-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="4dd5e-144">appleId</span><span class="sxs-lookup"><span data-stu-id="4dd5e-144">appleId</span></span>|<span data-ttu-id="4dd5e-145">String</span><span class="sxs-lookup"><span data-stu-id="4dd5e-145">String</span></span>|<span data-ttu-id="4dd5e-146">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4dd5e-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4dd5e-147">expirationDateTime</span></span>|<span data-ttu-id="4dd5e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dd5e-148">DateTimeOffset</span></span>|<span data-ttu-id="4dd5e-149">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4dd5e-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4dd5e-150">lastSyncDateTime</span></span>|<span data-ttu-id="4dd5e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dd5e-151">DateTimeOffset</span></span>|<span data-ttu-id="4dd5e-152">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4dd5e-153">token</span><span class="sxs-lookup"><span data-stu-id="4dd5e-153">token</span></span>|<span data-ttu-id="4dd5e-154">String</span><span class="sxs-lookup"><span data-stu-id="4dd5e-154">String</span></span>|<span data-ttu-id="4dd5e-155">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="4dd5e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dd5e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4dd5e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dd5e-157">DateTimeOffset</span></span>|<span data-ttu-id="4dd5e-158">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4dd5e-159">state</span><span class="sxs-lookup"><span data-stu-id="4dd5e-159">state</span></span>|[<span data-ttu-id="4dd5e-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="4dd5e-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="4dd5e-161">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="4dd5e-162">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="4dd5e-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="4dd5e-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="4dd5e-164">tokenActionResults</span></span>|<span data-ttu-id="4dd5e-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="4dd5e-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="4dd5e-166">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4dd5e-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="4dd5e-167">lastSyncStatus</span></span>|[<span data-ttu-id="4dd5e-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="4dd5e-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="4dd5e-169">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="4dd5e-170">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="4dd5e-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="4dd5e-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="4dd5e-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="4dd5e-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dd5e-173">Boolean</span></span>|<span data-ttu-id="4dd5e-174">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="4dd5e-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="4dd5e-175">countryOrRegion</span></span>|<span data-ttu-id="4dd5e-176">String</span><span class="sxs-lookup"><span data-stu-id="4dd5e-176">String</span></span>|<span data-ttu-id="4dd5e-177">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="4dd5e-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="4dd5e-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="4dd5e-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="4dd5e-179">Boolean</span></span>|<span data-ttu-id="4dd5e-180">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="4dd5e-181">displayName</span><span class="sxs-lookup"><span data-stu-id="4dd5e-181">displayName</span></span>|<span data-ttu-id="4dd5e-182">String</span><span class="sxs-lookup"><span data-stu-id="4dd5e-182">String</span></span>|<span data-ttu-id="4dd5e-183">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="4dd5e-184">locationName</span><span class="sxs-lookup"><span data-stu-id="4dd5e-184">locationName</span></span>|<span data-ttu-id="4dd5e-185">String</span><span class="sxs-lookup"><span data-stu-id="4dd5e-185">String</span></span>|<span data-ttu-id="4dd5e-186">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="4dd5e-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="4dd5e-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="4dd5e-188">布尔值</span><span class="sxs-lookup"><span data-stu-id="4dd5e-188">Boolean</span></span>|<span data-ttu-id="4dd5e-189">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="4dd5e-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4dd5e-190">roleScopeTagIds</span></span>|<span data-ttu-id="4dd5e-191">String collection</span><span class="sxs-lookup"><span data-stu-id="4dd5e-191">String collection</span></span>|<span data-ttu-id="4dd5e-192">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4dd5e-193">响应</span><span class="sxs-lookup"><span data-stu-id="4dd5e-193">Response</span></span>
<span data-ttu-id="4dd5e-194">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-194">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dd5e-195">示例</span><span class="sxs-lookup"><span data-stu-id="4dd5e-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dd5e-196">请求</span><span class="sxs-lookup"><span data-stu-id="4dd5e-196">Request</span></span>
<span data-ttu-id="4dd5e-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4dd5e-198">响应</span><span class="sxs-lookup"><span data-stu-id="4dd5e-198">Response</span></span>
<span data-ttu-id="4dd5e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dd5e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




