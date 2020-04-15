---
title: 更新 vppToken
description: 更新 vppToken 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 77c8e44b3f4ab04f40620c5b2286471d3334c627
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452772"
---
# <a name="update-vpptoken"></a><span data-ttu-id="08c94-103">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="08c94-103">Update vppToken</span></span>

<span data-ttu-id="08c94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08c94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08c94-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08c94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08c94-106">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="08c94-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08c94-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="08c94-107">Prerequisites</span></span>
<span data-ttu-id="08c94-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08c94-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="08c94-110">Permission type</span></span>|<span data-ttu-id="08c94-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08c94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08c94-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08c94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08c94-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08c94-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08c94-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08c94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08c94-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08c94-115">Not supported.</span></span>|
|<span data-ttu-id="08c94-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="08c94-116">Application</span></span>|<span data-ttu-id="08c94-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="08c94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08c94-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08c94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="08c94-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="08c94-119">Request headers</span></span>
|<span data-ttu-id="08c94-120">标头</span><span class="sxs-lookup"><span data-stu-id="08c94-120">Header</span></span>|<span data-ttu-id="08c94-121">值</span><span class="sxs-lookup"><span data-stu-id="08c94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08c94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c94-122">Authorization</span></span>|<span data-ttu-id="08c94-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08c94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08c94-124">接受</span><span class="sxs-lookup"><span data-stu-id="08c94-124">Accept</span></span>|<span data-ttu-id="08c94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08c94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08c94-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="08c94-126">Request body</span></span>
<span data-ttu-id="08c94-127">在请求正文中，提供 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08c94-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="08c94-128">下表显示创建 [vppToken](../resources/intune-onboarding-vpptoken.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08c94-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="08c94-129">属性</span><span class="sxs-lookup"><span data-stu-id="08c94-129">Property</span></span>|<span data-ttu-id="08c94-130">类型</span><span class="sxs-lookup"><span data-stu-id="08c94-130">Type</span></span>|<span data-ttu-id="08c94-131">说明</span><span class="sxs-lookup"><span data-stu-id="08c94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08c94-132">id</span><span class="sxs-lookup"><span data-stu-id="08c94-132">id</span></span>|<span data-ttu-id="08c94-133">String</span><span class="sxs-lookup"><span data-stu-id="08c94-133">String</span></span>|<span data-ttu-id="08c94-134">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="08c94-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="08c94-135">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="08c94-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="08c94-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="08c94-136">organizationName</span></span>|<span data-ttu-id="08c94-137">String</span><span class="sxs-lookup"><span data-stu-id="08c94-137">String</span></span>|<span data-ttu-id="08c94-138">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="08c94-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="08c94-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="08c94-139">vppTokenAccountType</span></span>|[<span data-ttu-id="08c94-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="08c94-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="08c94-141">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="08c94-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="08c94-142">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="08c94-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="08c94-143">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="08c94-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="08c94-144">appleId</span><span class="sxs-lookup"><span data-stu-id="08c94-144">appleId</span></span>|<span data-ttu-id="08c94-145">String</span><span class="sxs-lookup"><span data-stu-id="08c94-145">String</span></span>|<span data-ttu-id="08c94-146">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="08c94-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="08c94-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="08c94-147">expirationDateTime</span></span>|<span data-ttu-id="08c94-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08c94-148">DateTimeOffset</span></span>|<span data-ttu-id="08c94-149">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="08c94-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="08c94-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="08c94-150">lastSyncDateTime</span></span>|<span data-ttu-id="08c94-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08c94-151">DateTimeOffset</span></span>|<span data-ttu-id="08c94-152">上次使用 Apple Volume purchase program 服务（apple Volume purchase program 令牌）完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="08c94-152">The last time when an application sync was done with the Apple volume purchase program service using the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="08c94-153">token</span><span class="sxs-lookup"><span data-stu-id="08c94-153">token</span></span>|<span data-ttu-id="08c94-154">String</span><span class="sxs-lookup"><span data-stu-id="08c94-154">String</span></span>|<span data-ttu-id="08c94-155">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="08c94-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="08c94-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08c94-156">lastModifiedDateTime</span></span>|<span data-ttu-id="08c94-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08c94-157">DateTimeOffset</span></span>|<span data-ttu-id="08c94-158">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="08c94-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="08c94-159">state</span><span class="sxs-lookup"><span data-stu-id="08c94-159">state</span></span>|[<span data-ttu-id="08c94-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="08c94-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="08c94-161">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="08c94-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="08c94-162">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="08c94-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="08c94-163">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="08c94-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="08c94-164">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="08c94-164">lastSyncStatus</span></span>|[<span data-ttu-id="08c94-165">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="08c94-165">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="08c94-166">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="08c94-166">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="08c94-167">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="08c94-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="08c94-168">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="08c94-168">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="08c94-169">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="08c94-169">automaticallyUpdateApps</span></span>|<span data-ttu-id="08c94-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="08c94-170">Boolean</span></span>|<span data-ttu-id="08c94-171">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="08c94-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="08c94-172">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="08c94-172">countryOrRegion</span></span>|<span data-ttu-id="08c94-173">String</span><span class="sxs-lookup"><span data-stu-id="08c94-173">String</span></span>|<span data-ttu-id="08c94-174">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="08c94-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="08c94-175">响应</span><span class="sxs-lookup"><span data-stu-id="08c94-175">Response</span></span>
<span data-ttu-id="08c94-176">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08c94-176">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08c94-177">示例</span><span class="sxs-lookup"><span data-stu-id="08c94-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="08c94-178">请求</span><span class="sxs-lookup"><span data-stu-id="08c94-178">Request</span></span>
<span data-ttu-id="08c94-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08c94-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08c94-180">响应</span><span class="sxs-lookup"><span data-stu-id="08c94-180">Response</span></span>
<span data-ttu-id="08c94-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08c94-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






