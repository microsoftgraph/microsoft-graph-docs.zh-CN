---
title: 更新 vppToken
description: 更新 vppToken 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1e38660c1fa83ced205b0bbcc506303a3968c41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954145"
---
# <a name="update-vpptoken"></a><span data-ttu-id="b4438-103">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="b4438-103">Update vppToken</span></span>

> <span data-ttu-id="b4438-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b4438-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4438-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b4438-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4438-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b4438-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4438-107">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4438-107">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4438-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4438-108">Prerequisites</span></span>
<span data-ttu-id="b4438-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b4438-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4438-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4438-111">Permission type</span></span>|<span data-ttu-id="b4438-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b4438-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4438-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4438-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4438-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4438-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b4438-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4438-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4438-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4438-116">Not supported.</span></span>|
|<span data-ttu-id="b4438-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4438-117">Application</span></span>|<span data-ttu-id="b4438-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4438-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4438-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4438-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="b4438-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4438-120">Request headers</span></span>
|<span data-ttu-id="b4438-121">标头</span><span class="sxs-lookup"><span data-stu-id="b4438-121">Header</span></span>|<span data-ttu-id="b4438-122">值</span><span class="sxs-lookup"><span data-stu-id="b4438-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4438-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4438-123">Authorization</span></span>|<span data-ttu-id="b4438-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4438-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4438-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4438-125">Accept</span></span>|<span data-ttu-id="b4438-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4438-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4438-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4438-127">Request body</span></span>
<span data-ttu-id="b4438-128">在请求正文中，提供 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4438-128">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="b4438-129">下表显示创建 [vppToken](../resources/intune-onboarding-vpptoken.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b4438-129">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="b4438-130">属性</span><span class="sxs-lookup"><span data-stu-id="b4438-130">Property</span></span>|<span data-ttu-id="b4438-131">类型</span><span class="sxs-lookup"><span data-stu-id="b4438-131">Type</span></span>|<span data-ttu-id="b4438-132">说明</span><span class="sxs-lookup"><span data-stu-id="b4438-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4438-133">id</span><span class="sxs-lookup"><span data-stu-id="b4438-133">id</span></span>|<span data-ttu-id="b4438-134">String</span><span class="sxs-lookup"><span data-stu-id="b4438-134">String</span></span>|<span data-ttu-id="b4438-135">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="b4438-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="b4438-136">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="b4438-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="b4438-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="b4438-137">organizationName</span></span>|<span data-ttu-id="b4438-138">String</span><span class="sxs-lookup"><span data-stu-id="b4438-138">String</span></span>|<span data-ttu-id="b4438-139">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="b4438-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b4438-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b4438-140">vppTokenAccountType</span></span>|[<span data-ttu-id="b4438-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b4438-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="b4438-142">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="b4438-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="b4438-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="b4438-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="b4438-144">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="b4438-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b4438-145">appleId</span><span class="sxs-lookup"><span data-stu-id="b4438-145">appleId</span></span>|<span data-ttu-id="b4438-146">String</span><span class="sxs-lookup"><span data-stu-id="b4438-146">String</span></span>|<span data-ttu-id="b4438-147">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b4438-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b4438-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b4438-148">expirationDateTime</span></span>|<span data-ttu-id="b4438-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4438-149">DateTimeOffset</span></span>|<span data-ttu-id="b4438-150">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="b4438-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b4438-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b4438-151">lastSyncDateTime</span></span>|<span data-ttu-id="b4438-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4438-152">DateTimeOffset</span></span>|<span data-ttu-id="b4438-153">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="b4438-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b4438-154">token</span><span class="sxs-lookup"><span data-stu-id="b4438-154">token</span></span>|<span data-ttu-id="b4438-155">String</span><span class="sxs-lookup"><span data-stu-id="b4438-155">String</span></span>|<span data-ttu-id="b4438-156">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="b4438-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="b4438-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4438-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b4438-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4438-158">DateTimeOffset</span></span>|<span data-ttu-id="b4438-159">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b4438-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b4438-160">state</span><span class="sxs-lookup"><span data-stu-id="b4438-160">state</span></span>|[<span data-ttu-id="b4438-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="b4438-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="b4438-162">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="b4438-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b4438-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="b4438-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="b4438-164">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="b4438-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="b4438-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="b4438-165">tokenActionResults</span></span>|<span data-ttu-id="b4438-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="b4438-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="b4438-167">在 Apple 卷购买程序令牌执行的操作状态的集合。</span><span class="sxs-lookup"><span data-stu-id="b4438-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b4438-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b4438-168">lastSyncStatus</span></span>|[<span data-ttu-id="b4438-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b4438-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="b4438-170">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="b4438-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b4438-171">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b4438-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="b4438-172">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b4438-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="b4438-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="b4438-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="b4438-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4438-174">Boolean</span></span>|<span data-ttu-id="b4438-175">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="b4438-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="b4438-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b4438-176">countryOrRegion</span></span>|<span data-ttu-id="b4438-177">String</span><span class="sxs-lookup"><span data-stu-id="b4438-177">String</span></span>|<span data-ttu-id="b4438-178">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="b4438-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="b4438-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="b4438-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="b4438-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4438-180">Boolean</span></span>|<span data-ttu-id="b4438-181">Consent 授予与 Apple 卷购买程序共享的数据。</span><span class="sxs-lookup"><span data-stu-id="b4438-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="b4438-182">displayName</span><span class="sxs-lookup"><span data-stu-id="b4438-182">displayName</span></span>|<span data-ttu-id="b4438-183">字符串</span><span class="sxs-lookup"><span data-stu-id="b4438-183">String</span></span>|<span data-ttu-id="b4438-184">管理员指定标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="b4438-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="b4438-185">locationName</span><span class="sxs-lookup"><span data-stu-id="b4438-185">locationName</span></span>|<span data-ttu-id="b4438-186">字符串</span><span class="sxs-lookup"><span data-stu-id="b4438-186">String</span></span>|<span data-ttu-id="b4438-187">返回从 Apple VPP 令牌的位置。</span><span class="sxs-lookup"><span data-stu-id="b4438-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="b4438-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="b4438-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="b4438-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4438-189">Boolean</span></span>|<span data-ttu-id="b4438-190">管理员同意以允许声称令牌管理从外部 mdm。</span><span class="sxs-lookup"><span data-stu-id="b4438-190">Admin consent to allow claiming token management from external MDM.</span></span>|



## <a name="response"></a><span data-ttu-id="b4438-191">响应</span><span class="sxs-lookup"><span data-stu-id="b4438-191">Response</span></span>
<span data-ttu-id="b4438-192">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4438-192">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4438-193">示例</span><span class="sxs-lookup"><span data-stu-id="b4438-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4438-194">请求</span><span class="sxs-lookup"><span data-stu-id="b4438-194">Request</span></span>
<span data-ttu-id="b4438-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4438-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 957

{
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

### <a name="response"></a><span data-ttu-id="b4438-196">响应</span><span class="sxs-lookup"><span data-stu-id="b4438-196">Response</span></span>
<span data-ttu-id="b4438-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4438-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





