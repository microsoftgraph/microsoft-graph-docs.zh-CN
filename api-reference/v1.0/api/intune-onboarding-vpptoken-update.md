---
title: 更新 vppToken
description: 更新 vppToken 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a427a7ff1acdecef20ba7d1930cfe84f8538fd7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023970"
---
# <a name="update-vpptoken"></a><span data-ttu-id="91a62-103">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="91a62-103">Update vppToken</span></span>

> <span data-ttu-id="91a62-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91a62-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91a62-105">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="91a62-105">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91a62-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="91a62-106">Prerequisites</span></span>
<span data-ttu-id="91a62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91a62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91a62-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="91a62-109">Permission type</span></span>|<span data-ttu-id="91a62-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="91a62-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91a62-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91a62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91a62-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91a62-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="91a62-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91a62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91a62-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="91a62-114">Not supported.</span></span>|
|<span data-ttu-id="91a62-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="91a62-115">Application</span></span>|<span data-ttu-id="91a62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91a62-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91a62-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91a62-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="91a62-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="91a62-118">Request headers</span></span>
|<span data-ttu-id="91a62-119">标头</span><span class="sxs-lookup"><span data-stu-id="91a62-119">Header</span></span>|<span data-ttu-id="91a62-120">值</span><span class="sxs-lookup"><span data-stu-id="91a62-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91a62-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91a62-121">Authorization</span></span>|<span data-ttu-id="91a62-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91a62-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91a62-123">接受</span><span class="sxs-lookup"><span data-stu-id="91a62-123">Accept</span></span>|<span data-ttu-id="91a62-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91a62-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91a62-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="91a62-125">Request body</span></span>
<span data-ttu-id="91a62-126">在请求正文中，提供 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91a62-126">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="91a62-127">下表显示创建 [vppToken](../resources/intune-onboarding-vpptoken.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="91a62-127">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="91a62-128">属性</span><span class="sxs-lookup"><span data-stu-id="91a62-128">Property</span></span>|<span data-ttu-id="91a62-129">类型</span><span class="sxs-lookup"><span data-stu-id="91a62-129">Type</span></span>|<span data-ttu-id="91a62-130">说明</span><span class="sxs-lookup"><span data-stu-id="91a62-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91a62-131">id</span><span class="sxs-lookup"><span data-stu-id="91a62-131">id</span></span>|<span data-ttu-id="91a62-132">String</span><span class="sxs-lookup"><span data-stu-id="91a62-132">String</span></span>|<span data-ttu-id="91a62-133">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="91a62-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="91a62-134">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="91a62-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="91a62-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="91a62-135">organizationName</span></span>|<span data-ttu-id="91a62-136">String</span><span class="sxs-lookup"><span data-stu-id="91a62-136">String</span></span>|<span data-ttu-id="91a62-137">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="91a62-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="91a62-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="91a62-138">vppTokenAccountType</span></span>|[<span data-ttu-id="91a62-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="91a62-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="91a62-140">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="91a62-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="91a62-141">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="91a62-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="91a62-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="91a62-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="91a62-143">appleId</span><span class="sxs-lookup"><span data-stu-id="91a62-143">appleId</span></span>|<span data-ttu-id="91a62-144">String</span><span class="sxs-lookup"><span data-stu-id="91a62-144">String</span></span>|<span data-ttu-id="91a62-145">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="91a62-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="91a62-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="91a62-146">expirationDateTime</span></span>|<span data-ttu-id="91a62-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91a62-147">DateTimeOffset</span></span>|<span data-ttu-id="91a62-148">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="91a62-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="91a62-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="91a62-149">lastSyncDateTime</span></span>|<span data-ttu-id="91a62-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91a62-150">DateTimeOffset</span></span>|<span data-ttu-id="91a62-151">上次使用 Apple Volume purchase program 服务 (apple Volume purchase program 令牌) 完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="91a62-151">The last time when an application sync was done with the Apple volume purchase program service using the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="91a62-152">token</span><span class="sxs-lookup"><span data-stu-id="91a62-152">token</span></span>|<span data-ttu-id="91a62-153">String</span><span class="sxs-lookup"><span data-stu-id="91a62-153">String</span></span>|<span data-ttu-id="91a62-154">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="91a62-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="91a62-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91a62-155">lastModifiedDateTime</span></span>|<span data-ttu-id="91a62-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91a62-156">DateTimeOffset</span></span>|<span data-ttu-id="91a62-157">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="91a62-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="91a62-158">state</span><span class="sxs-lookup"><span data-stu-id="91a62-158">state</span></span>|[<span data-ttu-id="91a62-159">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="91a62-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="91a62-160">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="91a62-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="91a62-161">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="91a62-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="91a62-162">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="91a62-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="91a62-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="91a62-163">lastSyncStatus</span></span>|[<span data-ttu-id="91a62-164">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="91a62-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="91a62-165">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="91a62-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="91a62-166">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="91a62-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="91a62-167">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="91a62-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="91a62-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="91a62-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="91a62-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="91a62-169">Boolean</span></span>|<span data-ttu-id="91a62-170">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="91a62-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="91a62-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="91a62-171">countryOrRegion</span></span>|<span data-ttu-id="91a62-172">String</span><span class="sxs-lookup"><span data-stu-id="91a62-172">String</span></span>|<span data-ttu-id="91a62-173">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="91a62-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="91a62-174">响应</span><span class="sxs-lookup"><span data-stu-id="91a62-174">Response</span></span>
<span data-ttu-id="91a62-175">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91a62-175">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91a62-176">示例</span><span class="sxs-lookup"><span data-stu-id="91a62-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="91a62-177">请求</span><span class="sxs-lookup"><span data-stu-id="91a62-177">Request</span></span>
<span data-ttu-id="91a62-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91a62-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
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

### <a name="response"></a><span data-ttu-id="91a62-179">响应</span><span class="sxs-lookup"><span data-stu-id="91a62-179">Response</span></span>
<span data-ttu-id="91a62-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91a62-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



