---
title: 更新 vppToken
description: 更新 vppToken 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19541267f099afd03b5910b034234dbe34146e44
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978701"
---
# <a name="update-vpptoken"></a><span data-ttu-id="6aade-103">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="6aade-103">Update vppToken</span></span>

> <span data-ttu-id="6aade-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6aade-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aade-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6aade-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aade-106">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6aade-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aade-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6aade-107">Prerequisites</span></span>
<span data-ttu-id="6aade-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6aade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aade-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6aade-110">Permission type</span></span>|<span data-ttu-id="6aade-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6aade-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aade-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6aade-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aade-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aade-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6aade-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6aade-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aade-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aade-115">Not supported.</span></span>|
|<span data-ttu-id="6aade-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6aade-116">Application</span></span>|<span data-ttu-id="6aade-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aade-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aade-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6aade-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="6aade-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6aade-119">Request headers</span></span>
|<span data-ttu-id="6aade-120">标头</span><span class="sxs-lookup"><span data-stu-id="6aade-120">Header</span></span>|<span data-ttu-id="6aade-121">值</span><span class="sxs-lookup"><span data-stu-id="6aade-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aade-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aade-122">Authorization</span></span>|<span data-ttu-id="6aade-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6aade-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aade-124">接受</span><span class="sxs-lookup"><span data-stu-id="6aade-124">Accept</span></span>|<span data-ttu-id="6aade-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6aade-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aade-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6aade-126">Request body</span></span>
<span data-ttu-id="6aade-127">在请求正文中，提供 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6aade-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="6aade-128">下表显示创建 [vppToken](../resources/intune-onboarding-vpptoken.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6aade-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="6aade-129">属性</span><span class="sxs-lookup"><span data-stu-id="6aade-129">Property</span></span>|<span data-ttu-id="6aade-130">类型</span><span class="sxs-lookup"><span data-stu-id="6aade-130">Type</span></span>|<span data-ttu-id="6aade-131">说明</span><span class="sxs-lookup"><span data-stu-id="6aade-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aade-132">id</span><span class="sxs-lookup"><span data-stu-id="6aade-132">id</span></span>|<span data-ttu-id="6aade-133">String</span><span class="sxs-lookup"><span data-stu-id="6aade-133">String</span></span>|<span data-ttu-id="6aade-134">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="6aade-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="6aade-135">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="6aade-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="6aade-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="6aade-136">organizationName</span></span>|<span data-ttu-id="6aade-137">String</span><span class="sxs-lookup"><span data-stu-id="6aade-137">String</span></span>|<span data-ttu-id="6aade-138">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="6aade-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="6aade-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="6aade-139">vppTokenAccountType</span></span>|[<span data-ttu-id="6aade-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="6aade-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="6aade-141">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="6aade-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="6aade-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="6aade-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="6aade-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="6aade-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="6aade-144">appleId</span><span class="sxs-lookup"><span data-stu-id="6aade-144">appleId</span></span>|<span data-ttu-id="6aade-145">String</span><span class="sxs-lookup"><span data-stu-id="6aade-145">String</span></span>|<span data-ttu-id="6aade-146">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="6aade-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6aade-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6aade-147">expirationDateTime</span></span>|<span data-ttu-id="6aade-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aade-148">DateTimeOffset</span></span>|<span data-ttu-id="6aade-149">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="6aade-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6aade-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6aade-150">lastSyncDateTime</span></span>|<span data-ttu-id="6aade-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aade-151">DateTimeOffset</span></span>|<span data-ttu-id="6aade-152">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="6aade-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6aade-153">token</span><span class="sxs-lookup"><span data-stu-id="6aade-153">token</span></span>|<span data-ttu-id="6aade-154">String</span><span class="sxs-lookup"><span data-stu-id="6aade-154">String</span></span>|<span data-ttu-id="6aade-155">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="6aade-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="6aade-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6aade-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6aade-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aade-157">DateTimeOffset</span></span>|<span data-ttu-id="6aade-158">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="6aade-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6aade-159">state</span><span class="sxs-lookup"><span data-stu-id="6aade-159">state</span></span>|[<span data-ttu-id="6aade-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="6aade-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="6aade-161">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="6aade-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="6aade-162">可取值为：`unknown`、`valid`、`expired`、`invalid` 或 `assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="6aade-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="6aade-163">可取值为：`unknown`、`valid`、`expired`、`invalid` 或 `assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="6aade-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="6aade-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="6aade-164">tokenActionResults</span></span>|<span data-ttu-id="6aade-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="6aade-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="6aade-166">在 Apple volume purchase program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="6aade-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6aade-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="6aade-167">lastSyncStatus</span></span>|[<span data-ttu-id="6aade-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="6aade-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="6aade-169">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="6aade-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="6aade-170">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="6aade-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="6aade-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="6aade-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="6aade-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="6aade-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="6aade-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aade-173">Boolean</span></span>|<span data-ttu-id="6aade-174">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="6aade-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="6aade-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="6aade-175">countryOrRegion</span></span>|<span data-ttu-id="6aade-176">String</span><span class="sxs-lookup"><span data-stu-id="6aade-176">String</span></span>|<span data-ttu-id="6aade-177">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="6aade-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="6aade-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="6aade-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="6aade-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aade-179">Boolean</span></span>|<span data-ttu-id="6aade-180">同意授予与 Apple volume purchase program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="6aade-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="6aade-181">displayName</span><span class="sxs-lookup"><span data-stu-id="6aade-181">displayName</span></span>|<span data-ttu-id="6aade-182">String</span><span class="sxs-lookup"><span data-stu-id="6aade-182">String</span></span>|<span data-ttu-id="6aade-183">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="6aade-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="6aade-184">locationName</span><span class="sxs-lookup"><span data-stu-id="6aade-184">locationName</span></span>|<span data-ttu-id="6aade-185">String</span><span class="sxs-lookup"><span data-stu-id="6aade-185">String</span></span>|<span data-ttu-id="6aade-186">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="6aade-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="6aade-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="6aade-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="6aade-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aade-188">Boolean</span></span>|<span data-ttu-id="6aade-189">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="6aade-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="6aade-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6aade-190">roleScopeTagIds</span></span>|<span data-ttu-id="6aade-191">String 集合</span><span class="sxs-lookup"><span data-stu-id="6aade-191">String collection</span></span>|<span data-ttu-id="6aade-192">分配给此实体的角色范围标记 id。</span><span class="sxs-lookup"><span data-stu-id="6aade-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6aade-193">响应</span><span class="sxs-lookup"><span data-stu-id="6aade-193">Response</span></span>
<span data-ttu-id="6aade-194">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6aade-194">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aade-195">示例</span><span class="sxs-lookup"><span data-stu-id="6aade-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aade-196">请求</span><span class="sxs-lookup"><span data-stu-id="6aade-196">Request</span></span>
<span data-ttu-id="6aade-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6aade-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6aade-198">响应</span><span class="sxs-lookup"><span data-stu-id="6aade-198">Response</span></span>
<span data-ttu-id="6aade-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6aade-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




