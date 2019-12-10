---
title: 更新 vppToken
description: 更新 vppToken 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c783cfbba7f846b86a9dadb9a93745d505dff653
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941482"
---
# <a name="update-vpptoken"></a><span data-ttu-id="abbff-103">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="abbff-103">Update vppToken</span></span>

> <span data-ttu-id="abbff-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="abbff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abbff-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="abbff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abbff-106">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="abbff-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abbff-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="abbff-107">Prerequisites</span></span>
<span data-ttu-id="abbff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abbff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abbff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="abbff-110">Permission type</span></span>|<span data-ttu-id="abbff-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="abbff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abbff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abbff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abbff-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abbff-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="abbff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abbff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abbff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="abbff-115">Not supported.</span></span>|
|<span data-ttu-id="abbff-116">Application</span><span class="sxs-lookup"><span data-stu-id="abbff-116">Application</span></span>|<span data-ttu-id="abbff-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abbff-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abbff-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abbff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="abbff-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="abbff-119">Request headers</span></span>
|<span data-ttu-id="abbff-120">标头</span><span class="sxs-lookup"><span data-stu-id="abbff-120">Header</span></span>|<span data-ttu-id="abbff-121">值</span><span class="sxs-lookup"><span data-stu-id="abbff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abbff-122">授权</span><span class="sxs-lookup"><span data-stu-id="abbff-122">Authorization</span></span>|<span data-ttu-id="abbff-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="abbff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abbff-124">接受</span><span class="sxs-lookup"><span data-stu-id="abbff-124">Accept</span></span>|<span data-ttu-id="abbff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abbff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abbff-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="abbff-126">Request body</span></span>
<span data-ttu-id="abbff-127">在请求正文中，提供 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abbff-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="abbff-128">下表显示创建 [vppToken](../resources/intune-onboarding-vpptoken.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="abbff-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="abbff-129">属性</span><span class="sxs-lookup"><span data-stu-id="abbff-129">Property</span></span>|<span data-ttu-id="abbff-130">类型</span><span class="sxs-lookup"><span data-stu-id="abbff-130">Type</span></span>|<span data-ttu-id="abbff-131">说明</span><span class="sxs-lookup"><span data-stu-id="abbff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abbff-132">id</span><span class="sxs-lookup"><span data-stu-id="abbff-132">id</span></span>|<span data-ttu-id="abbff-133">字符串</span><span class="sxs-lookup"><span data-stu-id="abbff-133">String</span></span>|<span data-ttu-id="abbff-134">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="abbff-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="abbff-135">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="abbff-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="abbff-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="abbff-136">organizationName</span></span>|<span data-ttu-id="abbff-137">字符串</span><span class="sxs-lookup"><span data-stu-id="abbff-137">String</span></span>|<span data-ttu-id="abbff-138">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="abbff-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="abbff-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="abbff-139">vppTokenAccountType</span></span>|[<span data-ttu-id="abbff-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="abbff-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="abbff-141">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="abbff-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="abbff-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="abbff-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="abbff-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="abbff-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="abbff-144">appleId</span><span class="sxs-lookup"><span data-stu-id="abbff-144">appleId</span></span>|<span data-ttu-id="abbff-145">字符串</span><span class="sxs-lookup"><span data-stu-id="abbff-145">String</span></span>|<span data-ttu-id="abbff-146">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="abbff-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="abbff-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="abbff-147">expirationDateTime</span></span>|<span data-ttu-id="abbff-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbff-148">DateTimeOffset</span></span>|<span data-ttu-id="abbff-149">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="abbff-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="abbff-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="abbff-150">lastSyncDateTime</span></span>|<span data-ttu-id="abbff-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbff-151">DateTimeOffset</span></span>|<span data-ttu-id="abbff-152">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="abbff-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="abbff-153">token</span><span class="sxs-lookup"><span data-stu-id="abbff-153">token</span></span>|<span data-ttu-id="abbff-154">String</span><span class="sxs-lookup"><span data-stu-id="abbff-154">String</span></span>|<span data-ttu-id="abbff-155">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="abbff-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="abbff-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abbff-156">lastModifiedDateTime</span></span>|<span data-ttu-id="abbff-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbff-157">DateTimeOffset</span></span>|<span data-ttu-id="abbff-158">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="abbff-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="abbff-159">state</span><span class="sxs-lookup"><span data-stu-id="abbff-159">state</span></span>|[<span data-ttu-id="abbff-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="abbff-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="abbff-161">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="abbff-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="abbff-162">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="abbff-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="abbff-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="abbff-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="abbff-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="abbff-164">tokenActionResults</span></span>|<span data-ttu-id="abbff-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="abbff-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="abbff-166">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="abbff-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="abbff-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="abbff-167">lastSyncStatus</span></span>|[<span data-ttu-id="abbff-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="abbff-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="abbff-169">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="abbff-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="abbff-170">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="abbff-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="abbff-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="abbff-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="abbff-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="abbff-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="abbff-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="abbff-173">Boolean</span></span>|<span data-ttu-id="abbff-174">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="abbff-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="abbff-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="abbff-175">countryOrRegion</span></span>|<span data-ttu-id="abbff-176">String</span><span class="sxs-lookup"><span data-stu-id="abbff-176">String</span></span>|<span data-ttu-id="abbff-177">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="abbff-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="abbff-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="abbff-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="abbff-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="abbff-179">Boolean</span></span>|<span data-ttu-id="abbff-180">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="abbff-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="abbff-181">displayName</span><span class="sxs-lookup"><span data-stu-id="abbff-181">displayName</span></span>|<span data-ttu-id="abbff-182">字符串</span><span class="sxs-lookup"><span data-stu-id="abbff-182">String</span></span>|<span data-ttu-id="abbff-183">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="abbff-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="abbff-184">locationName</span><span class="sxs-lookup"><span data-stu-id="abbff-184">locationName</span></span>|<span data-ttu-id="abbff-185">字符串</span><span class="sxs-lookup"><span data-stu-id="abbff-185">String</span></span>|<span data-ttu-id="abbff-186">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="abbff-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="abbff-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="abbff-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="abbff-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="abbff-188">Boolean</span></span>|<span data-ttu-id="abbff-189">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="abbff-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="abbff-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="abbff-190">roleScopeTagIds</span></span>|<span data-ttu-id="abbff-191">String collection</span><span class="sxs-lookup"><span data-stu-id="abbff-191">String collection</span></span>|<span data-ttu-id="abbff-192">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="abbff-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="abbff-193">响应</span><span class="sxs-lookup"><span data-stu-id="abbff-193">Response</span></span>
<span data-ttu-id="abbff-194">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abbff-194">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abbff-195">示例</span><span class="sxs-lookup"><span data-stu-id="abbff-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="abbff-196">请求</span><span class="sxs-lookup"><span data-stu-id="abbff-196">Request</span></span>
<span data-ttu-id="abbff-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="abbff-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
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

### <a name="response"></a><span data-ttu-id="abbff-198">响应</span><span class="sxs-lookup"><span data-stu-id="abbff-198">Response</span></span>
<span data-ttu-id="abbff-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="abbff-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





