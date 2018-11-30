---
title: 创建 depOnboardingSetting
description: 创建新的 depOnboardingSetting 对象。
ms.openlocfilehash: 612afd3111af00cc8fd9819017b272ce5a38fe4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048812"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="84024-103">创建 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="84024-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="84024-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="84024-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84024-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84024-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84024-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="84024-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84024-107">创建新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84024-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84024-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="84024-108">Prerequisites</span></span>
<span data-ttu-id="84024-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="84024-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84024-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="84024-111">Permission type</span></span>|<span data-ttu-id="84024-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84024-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84024-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84024-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84024-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84024-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="84024-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84024-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84024-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84024-116">Not supported.</span></span>|
|<span data-ttu-id="84024-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="84024-117">Application</span></span>|<span data-ttu-id="84024-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="84024-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84024-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84024-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="84024-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84024-120">Request headers</span></span>
|<span data-ttu-id="84024-121">标头</span><span class="sxs-lookup"><span data-stu-id="84024-121">Header</span></span>|<span data-ttu-id="84024-122">值</span><span class="sxs-lookup"><span data-stu-id="84024-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84024-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84024-123">Authorization</span></span>|<span data-ttu-id="84024-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84024-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84024-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84024-125">Accept</span></span>|<span data-ttu-id="84024-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84024-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84024-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="84024-127">Request body</span></span>
<span data-ttu-id="84024-128">在请求正文中，提供 depOnboardingSetting 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84024-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="84024-129">下表显示时创建 depOnboardingSetting 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="84024-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="84024-130">属性</span><span class="sxs-lookup"><span data-stu-id="84024-130">Property</span></span>|<span data-ttu-id="84024-131">类型</span><span class="sxs-lookup"><span data-stu-id="84024-131">Type</span></span>|<span data-ttu-id="84024-132">说明</span><span class="sxs-lookup"><span data-stu-id="84024-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84024-133">id</span><span class="sxs-lookup"><span data-stu-id="84024-133">id</span></span>|<span data-ttu-id="84024-134">String</span><span class="sxs-lookup"><span data-stu-id="84024-134">String</span></span>|<span data-ttu-id="84024-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="84024-135">UUID for the object</span></span>|
|<span data-ttu-id="84024-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="84024-136">appleIdentifier</span></span>|<span data-ttu-id="84024-137">String</span><span class="sxs-lookup"><span data-stu-id="84024-137">String</span></span>|<span data-ttu-id="84024-138">Apple ID 用来获取当前的令牌。</span><span class="sxs-lookup"><span data-stu-id="84024-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="84024-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84024-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="84024-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84024-140">DateTimeOffset</span></span>|<span data-ttu-id="84024-141">该令牌将过期时。</span><span class="sxs-lookup"><span data-stu-id="84024-141">When the token will expire.</span></span>|
|<span data-ttu-id="84024-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84024-142">lastModifiedDateTime</span></span>|<span data-ttu-id="84024-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84024-143">DateTimeOffset</span></span>|<span data-ttu-id="84024-144">当该服务已 onboarded。</span><span class="sxs-lookup"><span data-stu-id="84024-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="84024-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="84024-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="84024-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84024-146">DateTimeOffset</span></span>|<span data-ttu-id="84024-147">当服务与 Intune 的最后一个 syned</span><span class="sxs-lookup"><span data-stu-id="84024-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="84024-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="84024-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="84024-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84024-149">DateTimeOffset</span></span>|<span data-ttu-id="84024-150">当 Intune 上次请求同步。</span><span class="sxs-lookup"><span data-stu-id="84024-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="84024-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="84024-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="84024-152">布尔</span><span class="sxs-lookup"><span data-stu-id="84024-152">Boolean</span></span>|<span data-ttu-id="84024-153">是否 Dep 令牌共享将启用学校数据同步服务。</span><span class="sxs-lookup"><span data-stu-id="84024-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="84024-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="84024-154">lastSyncErrorCode</span></span>|<span data-ttu-id="84024-155">Int32</span><span class="sxs-lookup"><span data-stu-id="84024-155">Int32</span></span>|<span data-ttu-id="84024-156">在最后一个 dep 同步过程中由 Apple 报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="84024-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="84024-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="84024-157">tokenType</span></span>|[<span data-ttu-id="84024-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="84024-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="84024-159">获取或设置 Dep 标记类型。</span><span class="sxs-lookup"><span data-stu-id="84024-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="84024-160">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="84024-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="84024-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="84024-161">tokenName</span></span>|<span data-ttu-id="84024-162">字符串</span><span class="sxs-lookup"><span data-stu-id="84024-162">String</span></span>|<span data-ttu-id="84024-163">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="84024-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="84024-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="84024-164">syncedDeviceCount</span></span>|<span data-ttu-id="84024-165">Int32</span><span class="sxs-lookup"><span data-stu-id="84024-165">Int32</span></span>|<span data-ttu-id="84024-166">获取同步设备计数</span><span class="sxs-lookup"><span data-stu-id="84024-166">Gets synced device count</span></span>|
|<span data-ttu-id="84024-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="84024-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="84024-168">字符串</span><span class="sxs-lookup"><span data-stu-id="84024-168">String</span></span>|<span data-ttu-id="84024-169">获取同步设备计数</span><span class="sxs-lookup"><span data-stu-id="84024-169">Gets synced device count</span></span>|
|<span data-ttu-id="84024-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="84024-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="84024-171">布尔</span><span class="sxs-lookup"><span data-stu-id="84024-171">Boolean</span></span>|<span data-ttu-id="84024-172">授予许可与 Apple Dep 服务共享的数据</span><span class="sxs-lookup"><span data-stu-id="84024-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="84024-173">响应</span><span class="sxs-lookup"><span data-stu-id="84024-173">Response</span></span>
<span data-ttu-id="84024-174">如果成功，此方法返回`201 Created`响应代码和响应正文中的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84024-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84024-175">示例</span><span class="sxs-lookup"><span data-stu-id="84024-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="84024-176">请求</span><span class="sxs-lookup"><span data-stu-id="84024-176">Request</span></span>
<span data-ttu-id="84024-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84024-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="84024-178">响应</span><span class="sxs-lookup"><span data-stu-id="84024-178">Response</span></span>
<span data-ttu-id="84024-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84024-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```





