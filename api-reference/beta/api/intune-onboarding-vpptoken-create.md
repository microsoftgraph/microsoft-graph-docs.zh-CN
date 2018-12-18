---
title: 创建 vppToken
description: 创建新的 vppToken 对象。
author: tfitzmac
ms.openlocfilehash: ab4c4c061f7a527583768382f309ef8c9adcb709
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353002"
---
# <a name="create-vpptoken"></a><span data-ttu-id="cedcf-103">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="cedcf-103">Create vppToken</span></span>

> <span data-ttu-id="cedcf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cedcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cedcf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cedcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cedcf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cedcf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cedcf-107">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cedcf-107">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cedcf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cedcf-108">Prerequisites</span></span>
<span data-ttu-id="cedcf-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cedcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cedcf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cedcf-111">Permission type</span></span>|<span data-ttu-id="cedcf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cedcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cedcf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cedcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cedcf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cedcf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cedcf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cedcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cedcf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cedcf-116">Not supported.</span></span>|
|<span data-ttu-id="cedcf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cedcf-117">Application</span></span>|<span data-ttu-id="cedcf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cedcf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cedcf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cedcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="cedcf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cedcf-120">Request headers</span></span>
|<span data-ttu-id="cedcf-121">标头</span><span class="sxs-lookup"><span data-stu-id="cedcf-121">Header</span></span>|<span data-ttu-id="cedcf-122">值</span><span class="sxs-lookup"><span data-stu-id="cedcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cedcf-123">授权</span><span class="sxs-lookup"><span data-stu-id="cedcf-123">Authorization</span></span>|<span data-ttu-id="cedcf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cedcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cedcf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cedcf-125">Accept</span></span>|<span data-ttu-id="cedcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cedcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cedcf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cedcf-127">Request body</span></span>
<span data-ttu-id="cedcf-128">在请求正文中，提供 vppToken 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cedcf-128">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="cedcf-129">下表显示创建 vppToken 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cedcf-129">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="cedcf-130">属性</span><span class="sxs-lookup"><span data-stu-id="cedcf-130">Property</span></span>|<span data-ttu-id="cedcf-131">类型</span><span class="sxs-lookup"><span data-stu-id="cedcf-131">Type</span></span>|<span data-ttu-id="cedcf-132">说明</span><span class="sxs-lookup"><span data-stu-id="cedcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cedcf-133">id</span><span class="sxs-lookup"><span data-stu-id="cedcf-133">id</span></span>|<span data-ttu-id="cedcf-134">String</span><span class="sxs-lookup"><span data-stu-id="cedcf-134">String</span></span>|<span data-ttu-id="cedcf-135">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="cedcf-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="cedcf-136">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="cedcf-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="cedcf-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="cedcf-137">organizationName</span></span>|<span data-ttu-id="cedcf-138">String</span><span class="sxs-lookup"><span data-stu-id="cedcf-138">String</span></span>|<span data-ttu-id="cedcf-139">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="cedcf-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="cedcf-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="cedcf-140">vppTokenAccountType</span></span>|[<span data-ttu-id="cedcf-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="cedcf-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="cedcf-142">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="cedcf-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="cedcf-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="cedcf-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="cedcf-144">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="cedcf-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="cedcf-145">appleId</span><span class="sxs-lookup"><span data-stu-id="cedcf-145">appleId</span></span>|<span data-ttu-id="cedcf-146">String</span><span class="sxs-lookup"><span data-stu-id="cedcf-146">String</span></span>|<span data-ttu-id="cedcf-147">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="cedcf-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="cedcf-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cedcf-148">expirationDateTime</span></span>|<span data-ttu-id="cedcf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedcf-149">DateTimeOffset</span></span>|<span data-ttu-id="cedcf-150">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="cedcf-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="cedcf-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cedcf-151">lastSyncDateTime</span></span>|<span data-ttu-id="cedcf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedcf-152">DateTimeOffset</span></span>|<span data-ttu-id="cedcf-153">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="cedcf-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="cedcf-154">token</span><span class="sxs-lookup"><span data-stu-id="cedcf-154">token</span></span>|<span data-ttu-id="cedcf-155">String</span><span class="sxs-lookup"><span data-stu-id="cedcf-155">String</span></span>|<span data-ttu-id="cedcf-156">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="cedcf-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="cedcf-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cedcf-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cedcf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedcf-158">DateTimeOffset</span></span>|<span data-ttu-id="cedcf-159">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="cedcf-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="cedcf-160">state</span><span class="sxs-lookup"><span data-stu-id="cedcf-160">state</span></span>|[<span data-ttu-id="cedcf-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="cedcf-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="cedcf-162">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="cedcf-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="cedcf-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="cedcf-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="cedcf-164">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="cedcf-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="cedcf-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="cedcf-165">tokenActionResults</span></span>|<span data-ttu-id="cedcf-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="cedcf-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="cedcf-167">在 Apple 卷购买程序令牌执行的操作状态的集合。</span><span class="sxs-lookup"><span data-stu-id="cedcf-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="cedcf-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="cedcf-168">lastSyncStatus</span></span>|[<span data-ttu-id="cedcf-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="cedcf-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="cedcf-170">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="cedcf-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="cedcf-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="cedcf-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="cedcf-172">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="cedcf-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="cedcf-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="cedcf-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="cedcf-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="cedcf-174">Boolean</span></span>|<span data-ttu-id="cedcf-175">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="cedcf-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="cedcf-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="cedcf-176">countryOrRegion</span></span>|<span data-ttu-id="cedcf-177">String</span><span class="sxs-lookup"><span data-stu-id="cedcf-177">String</span></span>|<span data-ttu-id="cedcf-178">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="cedcf-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="cedcf-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="cedcf-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="cedcf-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="cedcf-180">Boolean</span></span>|<span data-ttu-id="cedcf-181">Consent 授予与 Apple 卷购买程序共享的数据。</span><span class="sxs-lookup"><span data-stu-id="cedcf-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="cedcf-182">displayName</span><span class="sxs-lookup"><span data-stu-id="cedcf-182">displayName</span></span>|<span data-ttu-id="cedcf-183">字符串</span><span class="sxs-lookup"><span data-stu-id="cedcf-183">String</span></span>|<span data-ttu-id="cedcf-184">管理员指定标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="cedcf-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="cedcf-185">locationName</span><span class="sxs-lookup"><span data-stu-id="cedcf-185">locationName</span></span>|<span data-ttu-id="cedcf-186">字符串</span><span class="sxs-lookup"><span data-stu-id="cedcf-186">String</span></span>|<span data-ttu-id="cedcf-187">返回从 Apple VPP 令牌的位置。</span><span class="sxs-lookup"><span data-stu-id="cedcf-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="cedcf-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="cedcf-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="cedcf-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="cedcf-189">Boolean</span></span>|<span data-ttu-id="cedcf-190">管理员同意以允许声称令牌管理从外部 mdm。</span><span class="sxs-lookup"><span data-stu-id="cedcf-190">Admin consent to allow claiming token management from external MDM.</span></span>|



## <a name="response"></a><span data-ttu-id="cedcf-191">响应</span><span class="sxs-lookup"><span data-stu-id="cedcf-191">Response</span></span>
<span data-ttu-id="cedcf-192">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cedcf-192">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cedcf-193">示例</span><span class="sxs-lookup"><span data-stu-id="cedcf-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="cedcf-194">请求</span><span class="sxs-lookup"><span data-stu-id="cedcf-194">Request</span></span>
<span data-ttu-id="cedcf-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cedcf-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 1004

{
  "@odata.type": "#microsoft.graph.vppToken",
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
  "claimTokenManagementFromExternalMdm": true
}
```

### <a name="response"></a><span data-ttu-id="cedcf-196">响应</span><span class="sxs-lookup"><span data-stu-id="cedcf-196">Response</span></span>
<span data-ttu-id="cedcf-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cedcf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1053

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
  "claimTokenManagementFromExternalMdm": true
}
```





