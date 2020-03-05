---
title: 更新 vppToken
description: 更新 vppToken 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: feaa8f13cbb63e2b656ca7507fb204b0d4a7700c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461625"
---
# <a name="update-vpptoken"></a><span data-ttu-id="85e70-103">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="85e70-103">Update vppToken</span></span>

<span data-ttu-id="85e70-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="85e70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85e70-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85e70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85e70-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85e70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e70-107">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="85e70-107">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85e70-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85e70-108">Prerequisites</span></span>
<span data-ttu-id="85e70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e70-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85e70-111">Permission type</span></span>|<span data-ttu-id="85e70-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85e70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85e70-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85e70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85e70-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e70-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85e70-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85e70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85e70-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85e70-116">Not supported.</span></span>|
|<span data-ttu-id="85e70-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="85e70-117">Application</span></span>|<span data-ttu-id="85e70-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e70-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85e70-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85e70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="85e70-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="85e70-120">Request headers</span></span>
|<span data-ttu-id="85e70-121">标头</span><span class="sxs-lookup"><span data-stu-id="85e70-121">Header</span></span>|<span data-ttu-id="85e70-122">值</span><span class="sxs-lookup"><span data-stu-id="85e70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85e70-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85e70-123">Authorization</span></span>|<span data-ttu-id="85e70-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85e70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85e70-125">接受</span><span class="sxs-lookup"><span data-stu-id="85e70-125">Accept</span></span>|<span data-ttu-id="85e70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85e70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85e70-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85e70-127">Request body</span></span>
<span data-ttu-id="85e70-128">在请求正文中，提供 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85e70-128">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="85e70-129">下表显示创建 [vppToken](../resources/intune-onboarding-vpptoken.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85e70-129">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="85e70-130">属性</span><span class="sxs-lookup"><span data-stu-id="85e70-130">Property</span></span>|<span data-ttu-id="85e70-131">类型</span><span class="sxs-lookup"><span data-stu-id="85e70-131">Type</span></span>|<span data-ttu-id="85e70-132">说明</span><span class="sxs-lookup"><span data-stu-id="85e70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e70-133">id</span><span class="sxs-lookup"><span data-stu-id="85e70-133">id</span></span>|<span data-ttu-id="85e70-134">String</span><span class="sxs-lookup"><span data-stu-id="85e70-134">String</span></span>|<span data-ttu-id="85e70-135">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="85e70-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="85e70-136">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="85e70-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="85e70-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="85e70-137">organizationName</span></span>|<span data-ttu-id="85e70-138">String</span><span class="sxs-lookup"><span data-stu-id="85e70-138">String</span></span>|<span data-ttu-id="85e70-139">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="85e70-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="85e70-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="85e70-140">vppTokenAccountType</span></span>|[<span data-ttu-id="85e70-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="85e70-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="85e70-142">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="85e70-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="85e70-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="85e70-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="85e70-144">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="85e70-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="85e70-145">appleId</span><span class="sxs-lookup"><span data-stu-id="85e70-145">appleId</span></span>|<span data-ttu-id="85e70-146">String</span><span class="sxs-lookup"><span data-stu-id="85e70-146">String</span></span>|<span data-ttu-id="85e70-147">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="85e70-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="85e70-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="85e70-148">expirationDateTime</span></span>|<span data-ttu-id="85e70-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e70-149">DateTimeOffset</span></span>|<span data-ttu-id="85e70-150">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="85e70-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="85e70-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="85e70-151">lastSyncDateTime</span></span>|<span data-ttu-id="85e70-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e70-152">DateTimeOffset</span></span>|<span data-ttu-id="85e70-153">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="85e70-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="85e70-154">token</span><span class="sxs-lookup"><span data-stu-id="85e70-154">token</span></span>|<span data-ttu-id="85e70-155">String</span><span class="sxs-lookup"><span data-stu-id="85e70-155">String</span></span>|<span data-ttu-id="85e70-156">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="85e70-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="85e70-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85e70-157">lastModifiedDateTime</span></span>|<span data-ttu-id="85e70-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e70-158">DateTimeOffset</span></span>|<span data-ttu-id="85e70-159">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="85e70-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="85e70-160">state</span><span class="sxs-lookup"><span data-stu-id="85e70-160">state</span></span>|[<span data-ttu-id="85e70-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="85e70-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="85e70-162">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="85e70-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="85e70-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="85e70-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="85e70-164">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="85e70-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="85e70-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="85e70-165">tokenActionResults</span></span>|<span data-ttu-id="85e70-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="85e70-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="85e70-167">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="85e70-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="85e70-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="85e70-168">lastSyncStatus</span></span>|[<span data-ttu-id="85e70-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="85e70-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="85e70-170">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="85e70-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="85e70-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="85e70-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="85e70-172">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="85e70-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="85e70-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="85e70-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="85e70-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e70-174">Boolean</span></span>|<span data-ttu-id="85e70-175">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="85e70-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="85e70-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="85e70-176">countryOrRegion</span></span>|<span data-ttu-id="85e70-177">String</span><span class="sxs-lookup"><span data-stu-id="85e70-177">String</span></span>|<span data-ttu-id="85e70-178">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="85e70-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="85e70-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="85e70-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="85e70-180">布尔</span><span class="sxs-lookup"><span data-stu-id="85e70-180">Boolean</span></span>|<span data-ttu-id="85e70-181">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="85e70-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="85e70-182">displayName</span><span class="sxs-lookup"><span data-stu-id="85e70-182">displayName</span></span>|<span data-ttu-id="85e70-183">String</span><span class="sxs-lookup"><span data-stu-id="85e70-183">String</span></span>|<span data-ttu-id="85e70-184">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="85e70-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="85e70-185">locationName</span><span class="sxs-lookup"><span data-stu-id="85e70-185">locationName</span></span>|<span data-ttu-id="85e70-186">String</span><span class="sxs-lookup"><span data-stu-id="85e70-186">String</span></span>|<span data-ttu-id="85e70-187">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="85e70-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="85e70-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="85e70-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="85e70-189">布尔</span><span class="sxs-lookup"><span data-stu-id="85e70-189">Boolean</span></span>|<span data-ttu-id="85e70-190">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="85e70-190">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="85e70-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85e70-191">roleScopeTagIds</span></span>|<span data-ttu-id="85e70-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="85e70-192">String collection</span></span>|<span data-ttu-id="85e70-193">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="85e70-193">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="85e70-194">响应</span><span class="sxs-lookup"><span data-stu-id="85e70-194">Response</span></span>
<span data-ttu-id="85e70-195">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85e70-195">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85e70-196">示例</span><span class="sxs-lookup"><span data-stu-id="85e70-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="85e70-197">请求</span><span class="sxs-lookup"><span data-stu-id="85e70-197">Request</span></span>
<span data-ttu-id="85e70-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85e70-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85e70-199">响应</span><span class="sxs-lookup"><span data-stu-id="85e70-199">Response</span></span>
<span data-ttu-id="85e70-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85e70-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





