---
title: 创建 vppToken
description: 创建新的 vppToken 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 713a6bf583ff9c315ec88a83811312e6a6af5d92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582547"
---
# <a name="create-vpptoken"></a><span data-ttu-id="a7628-103">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="a7628-103">Create vppToken</span></span>

> <span data-ttu-id="a7628-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7628-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7628-105">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7628-105">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7628-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7628-106">Prerequisites</span></span>
<span data-ttu-id="a7628-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7628-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7628-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7628-109">Permission type</span></span>|<span data-ttu-id="a7628-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7628-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7628-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7628-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7628-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7628-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a7628-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7628-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7628-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7628-114">Not supported.</span></span>|
|<span data-ttu-id="a7628-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7628-115">Application</span></span>|<span data-ttu-id="a7628-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7628-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7628-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7628-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="a7628-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7628-118">Request headers</span></span>
|<span data-ttu-id="a7628-119">标头</span><span class="sxs-lookup"><span data-stu-id="a7628-119">Header</span></span>|<span data-ttu-id="a7628-120">值</span><span class="sxs-lookup"><span data-stu-id="a7628-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7628-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7628-121">Authorization</span></span>|<span data-ttu-id="a7628-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7628-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7628-123">接受</span><span class="sxs-lookup"><span data-stu-id="a7628-123">Accept</span></span>|<span data-ttu-id="a7628-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7628-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7628-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7628-125">Request body</span></span>
<span data-ttu-id="a7628-126">在请求正文中，提供 vppToken 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7628-126">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="a7628-127">下表显示创建 vppToken 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a7628-127">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="a7628-128">属性</span><span class="sxs-lookup"><span data-stu-id="a7628-128">Property</span></span>|<span data-ttu-id="a7628-129">类型</span><span class="sxs-lookup"><span data-stu-id="a7628-129">Type</span></span>|<span data-ttu-id="a7628-130">说明</span><span class="sxs-lookup"><span data-stu-id="a7628-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7628-131">id</span><span class="sxs-lookup"><span data-stu-id="a7628-131">id</span></span>|<span data-ttu-id="a7628-132">String</span><span class="sxs-lookup"><span data-stu-id="a7628-132">String</span></span>|<span data-ttu-id="a7628-133">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="a7628-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="a7628-134">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="a7628-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="a7628-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="a7628-135">organizationName</span></span>|<span data-ttu-id="a7628-136">String</span><span class="sxs-lookup"><span data-stu-id="a7628-136">String</span></span>|<span data-ttu-id="a7628-137">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="a7628-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="a7628-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a7628-138">vppTokenAccountType</span></span>|[<span data-ttu-id="a7628-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a7628-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="a7628-140">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="a7628-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="a7628-141">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="a7628-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="a7628-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="a7628-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="a7628-143">appleId</span><span class="sxs-lookup"><span data-stu-id="a7628-143">appleId</span></span>|<span data-ttu-id="a7628-144">String</span><span class="sxs-lookup"><span data-stu-id="a7628-144">String</span></span>|<span data-ttu-id="a7628-145">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a7628-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a7628-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a7628-146">expirationDateTime</span></span>|<span data-ttu-id="a7628-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7628-147">DateTimeOffset</span></span>|<span data-ttu-id="a7628-148">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="a7628-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a7628-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a7628-149">lastSyncDateTime</span></span>|<span data-ttu-id="a7628-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7628-150">DateTimeOffset</span></span>|<span data-ttu-id="a7628-151">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="a7628-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a7628-152">token</span><span class="sxs-lookup"><span data-stu-id="a7628-152">token</span></span>|<span data-ttu-id="a7628-153">String</span><span class="sxs-lookup"><span data-stu-id="a7628-153">String</span></span>|<span data-ttu-id="a7628-154">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="a7628-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="a7628-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7628-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a7628-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7628-156">DateTimeOffset</span></span>|<span data-ttu-id="a7628-157">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="a7628-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a7628-158">state</span><span class="sxs-lookup"><span data-stu-id="a7628-158">state</span></span>|[<span data-ttu-id="a7628-159">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="a7628-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="a7628-160">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a7628-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a7628-161">可取值为：`unknown`、`valid`、`expired`、`invalid` 或 `assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="a7628-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="a7628-162">可取值为：`unknown`、`valid`、`expired`、`invalid` 或 `assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="a7628-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="a7628-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a7628-163">lastSyncStatus</span></span>|[<span data-ttu-id="a7628-164">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a7628-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="a7628-165">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="a7628-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a7628-166">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a7628-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="a7628-167">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a7628-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a7628-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="a7628-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="a7628-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7628-169">Boolean</span></span>|<span data-ttu-id="a7628-170">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="a7628-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="a7628-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a7628-171">countryOrRegion</span></span>|<span data-ttu-id="a7628-172">String</span><span class="sxs-lookup"><span data-stu-id="a7628-172">String</span></span>|<span data-ttu-id="a7628-173">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="a7628-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="a7628-174">响应</span><span class="sxs-lookup"><span data-stu-id="a7628-174">Response</span></span>
<span data-ttu-id="a7628-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7628-175">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7628-176">示例</span><span class="sxs-lookup"><span data-stu-id="a7628-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7628-177">请求</span><span class="sxs-lookup"><span data-stu-id="a7628-177">Request</span></span>
<span data-ttu-id="a7628-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7628-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7628-179">响应</span><span class="sxs-lookup"><span data-stu-id="a7628-179">Response</span></span>
<span data-ttu-id="a7628-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7628-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



