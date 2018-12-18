---
title: 创建 vppToken
description: 创建新的 vppToken 对象。
author: tfitzmac
ms.openlocfilehash: 029af74ac49b6e95412f32a82bf57e69a78ffe4f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351315"
---
# <a name="create-vpptoken"></a><span data-ttu-id="52c31-103">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="52c31-103">Create vppToken</span></span>

> <span data-ttu-id="52c31-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="52c31-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52c31-105">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52c31-105">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52c31-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="52c31-106">Prerequisites</span></span>
<span data-ttu-id="52c31-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="52c31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52c31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52c31-109">Permission type</span></span>|<span data-ttu-id="52c31-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="52c31-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52c31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52c31-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52c31-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52c31-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="52c31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52c31-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52c31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52c31-114">Not supported.</span></span>|
|<span data-ttu-id="52c31-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52c31-115">Application</span></span>|<span data-ttu-id="52c31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52c31-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52c31-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52c31-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="52c31-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="52c31-118">Request headers</span></span>
|<span data-ttu-id="52c31-119">标头</span><span class="sxs-lookup"><span data-stu-id="52c31-119">Header</span></span>|<span data-ttu-id="52c31-120">值</span><span class="sxs-lookup"><span data-stu-id="52c31-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52c31-121">授权</span><span class="sxs-lookup"><span data-stu-id="52c31-121">Authorization</span></span>|<span data-ttu-id="52c31-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="52c31-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52c31-123">Accept</span><span class="sxs-lookup"><span data-stu-id="52c31-123">Accept</span></span>|<span data-ttu-id="52c31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="52c31-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52c31-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="52c31-125">Request body</span></span>
<span data-ttu-id="52c31-126">在请求正文中，提供 vppToken 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52c31-126">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="52c31-127">下表显示创建 vppToken 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="52c31-127">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="52c31-128">属性</span><span class="sxs-lookup"><span data-stu-id="52c31-128">Property</span></span>|<span data-ttu-id="52c31-129">类型</span><span class="sxs-lookup"><span data-stu-id="52c31-129">Type</span></span>|<span data-ttu-id="52c31-130">说明</span><span class="sxs-lookup"><span data-stu-id="52c31-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52c31-131">id</span><span class="sxs-lookup"><span data-stu-id="52c31-131">id</span></span>|<span data-ttu-id="52c31-132">String</span><span class="sxs-lookup"><span data-stu-id="52c31-132">String</span></span>|<span data-ttu-id="52c31-133">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="52c31-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="52c31-134">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="52c31-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="52c31-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="52c31-135">organizationName</span></span>|<span data-ttu-id="52c31-136">String</span><span class="sxs-lookup"><span data-stu-id="52c31-136">String</span></span>|<span data-ttu-id="52c31-137">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="52c31-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="52c31-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="52c31-138">vppTokenAccountType</span></span>|[<span data-ttu-id="52c31-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="52c31-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="52c31-140">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="52c31-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="52c31-141">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="52c31-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="52c31-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="52c31-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="52c31-143">appleId</span><span class="sxs-lookup"><span data-stu-id="52c31-143">appleId</span></span>|<span data-ttu-id="52c31-144">String</span><span class="sxs-lookup"><span data-stu-id="52c31-144">String</span></span>|<span data-ttu-id="52c31-145">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="52c31-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="52c31-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="52c31-146">expirationDateTime</span></span>|<span data-ttu-id="52c31-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52c31-147">DateTimeOffset</span></span>|<span data-ttu-id="52c31-148">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="52c31-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="52c31-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="52c31-149">lastSyncDateTime</span></span>|<span data-ttu-id="52c31-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52c31-150">DateTimeOffset</span></span>|<span data-ttu-id="52c31-151">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="52c31-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="52c31-152">token</span><span class="sxs-lookup"><span data-stu-id="52c31-152">token</span></span>|<span data-ttu-id="52c31-153">String</span><span class="sxs-lookup"><span data-stu-id="52c31-153">String</span></span>|<span data-ttu-id="52c31-154">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="52c31-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="52c31-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52c31-155">lastModifiedDateTime</span></span>|<span data-ttu-id="52c31-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52c31-156">DateTimeOffset</span></span>|<span data-ttu-id="52c31-157">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="52c31-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="52c31-158">state</span><span class="sxs-lookup"><span data-stu-id="52c31-158">state</span></span>|[<span data-ttu-id="52c31-159">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="52c31-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="52c31-160">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="52c31-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="52c31-161">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="52c31-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="52c31-162">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="52c31-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="52c31-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="52c31-163">lastSyncStatus</span></span>|[<span data-ttu-id="52c31-164">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="52c31-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="52c31-165">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="52c31-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="52c31-166">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="52c31-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="52c31-167">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="52c31-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="52c31-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="52c31-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="52c31-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="52c31-169">Boolean</span></span>|<span data-ttu-id="52c31-170">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="52c31-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="52c31-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="52c31-171">countryOrRegion</span></span>|<span data-ttu-id="52c31-172">String</span><span class="sxs-lookup"><span data-stu-id="52c31-172">String</span></span>|<span data-ttu-id="52c31-173">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="52c31-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="52c31-174">响应</span><span class="sxs-lookup"><span data-stu-id="52c31-174">Response</span></span>
<span data-ttu-id="52c31-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52c31-175">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52c31-176">示例</span><span class="sxs-lookup"><span data-stu-id="52c31-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="52c31-177">请求</span><span class="sxs-lookup"><span data-stu-id="52c31-177">Request</span></span>
<span data-ttu-id="52c31-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52c31-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="52c31-179">响应</span><span class="sxs-lookup"><span data-stu-id="52c31-179">Response</span></span>
<span data-ttu-id="52c31-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52c31-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

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
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```



