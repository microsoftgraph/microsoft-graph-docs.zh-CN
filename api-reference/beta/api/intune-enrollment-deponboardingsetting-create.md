---
title: 创建 depOnboardingSetting
description: 创建新的 depOnboardingSetting 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e9a5ed92f1a0ce656c1baa7af8a3cb23299395a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949484"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="580ad-103">创建 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="580ad-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="580ad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="580ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="580ad-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="580ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="580ad-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="580ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="580ad-107">创建新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="580ad-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="580ad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="580ad-108">Prerequisites</span></span>
<span data-ttu-id="580ad-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="580ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="580ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="580ad-111">Permission type</span></span>|<span data-ttu-id="580ad-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="580ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="580ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="580ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="580ad-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="580ad-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="580ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="580ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="580ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="580ad-116">Not supported.</span></span>|
|<span data-ttu-id="580ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="580ad-117">Application</span></span>|<span data-ttu-id="580ad-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="580ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="580ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="580ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="580ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="580ad-120">Request headers</span></span>
|<span data-ttu-id="580ad-121">标头</span><span class="sxs-lookup"><span data-stu-id="580ad-121">Header</span></span>|<span data-ttu-id="580ad-122">值</span><span class="sxs-lookup"><span data-stu-id="580ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="580ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="580ad-123">Authorization</span></span>|<span data-ttu-id="580ad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="580ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="580ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="580ad-125">Accept</span></span>|<span data-ttu-id="580ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="580ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="580ad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="580ad-127">Request body</span></span>
<span data-ttu-id="580ad-128">在请求正文中，提供 depOnboardingSetting 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="580ad-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="580ad-129">下表显示时创建 depOnboardingSetting 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="580ad-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="580ad-130">属性</span><span class="sxs-lookup"><span data-stu-id="580ad-130">Property</span></span>|<span data-ttu-id="580ad-131">类型</span><span class="sxs-lookup"><span data-stu-id="580ad-131">Type</span></span>|<span data-ttu-id="580ad-132">说明</span><span class="sxs-lookup"><span data-stu-id="580ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="580ad-133">id</span><span class="sxs-lookup"><span data-stu-id="580ad-133">id</span></span>|<span data-ttu-id="580ad-134">String</span><span class="sxs-lookup"><span data-stu-id="580ad-134">String</span></span>|<span data-ttu-id="580ad-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="580ad-135">UUID for the object</span></span>|
|<span data-ttu-id="580ad-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="580ad-136">appleIdentifier</span></span>|<span data-ttu-id="580ad-137">String</span><span class="sxs-lookup"><span data-stu-id="580ad-137">String</span></span>|<span data-ttu-id="580ad-138">Apple ID 用来获取当前的令牌。</span><span class="sxs-lookup"><span data-stu-id="580ad-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="580ad-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="580ad-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="580ad-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="580ad-140">DateTimeOffset</span></span>|<span data-ttu-id="580ad-141">该令牌将过期时。</span><span class="sxs-lookup"><span data-stu-id="580ad-141">When the token will expire.</span></span>|
|<span data-ttu-id="580ad-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="580ad-142">lastModifiedDateTime</span></span>|<span data-ttu-id="580ad-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="580ad-143">DateTimeOffset</span></span>|<span data-ttu-id="580ad-144">当该服务已 onboarded。</span><span class="sxs-lookup"><span data-stu-id="580ad-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="580ad-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="580ad-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="580ad-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="580ad-146">DateTimeOffset</span></span>|<span data-ttu-id="580ad-147">当服务与 Intune 的最后一个 syned</span><span class="sxs-lookup"><span data-stu-id="580ad-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="580ad-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="580ad-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="580ad-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="580ad-149">DateTimeOffset</span></span>|<span data-ttu-id="580ad-150">当 Intune 上次请求同步。</span><span class="sxs-lookup"><span data-stu-id="580ad-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="580ad-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="580ad-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="580ad-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="580ad-152">Boolean</span></span>|<span data-ttu-id="580ad-153">是否 Dep 令牌共享将启用学校数据同步服务。</span><span class="sxs-lookup"><span data-stu-id="580ad-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="580ad-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="580ad-154">lastSyncErrorCode</span></span>|<span data-ttu-id="580ad-155">Int32</span><span class="sxs-lookup"><span data-stu-id="580ad-155">Int32</span></span>|<span data-ttu-id="580ad-156">在最后一个 dep 同步过程中由 Apple 报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="580ad-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="580ad-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="580ad-157">tokenType</span></span>|[<span data-ttu-id="580ad-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="580ad-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="580ad-159">获取或设置 Dep 标记类型。</span><span class="sxs-lookup"><span data-stu-id="580ad-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="580ad-160">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="580ad-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="580ad-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="580ad-161">tokenName</span></span>|<span data-ttu-id="580ad-162">字符串</span><span class="sxs-lookup"><span data-stu-id="580ad-162">String</span></span>|<span data-ttu-id="580ad-163">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="580ad-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="580ad-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="580ad-164">syncedDeviceCount</span></span>|<span data-ttu-id="580ad-165">Int32</span><span class="sxs-lookup"><span data-stu-id="580ad-165">Int32</span></span>|<span data-ttu-id="580ad-166">获取同步设备计数</span><span class="sxs-lookup"><span data-stu-id="580ad-166">Gets synced device count</span></span>|
|<span data-ttu-id="580ad-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="580ad-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="580ad-168">字符串</span><span class="sxs-lookup"><span data-stu-id="580ad-168">String</span></span>|<span data-ttu-id="580ad-169">获取同步设备计数</span><span class="sxs-lookup"><span data-stu-id="580ad-169">Gets synced device count</span></span>|
|<span data-ttu-id="580ad-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="580ad-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="580ad-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="580ad-171">Boolean</span></span>|<span data-ttu-id="580ad-172">授予许可与 Apple Dep 服务共享的数据</span><span class="sxs-lookup"><span data-stu-id="580ad-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="580ad-173">响应</span><span class="sxs-lookup"><span data-stu-id="580ad-173">Response</span></span>
<span data-ttu-id="580ad-174">如果成功，此方法返回`201 Created`响应代码和响应正文中的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="580ad-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="580ad-175">示例</span><span class="sxs-lookup"><span data-stu-id="580ad-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="580ad-176">请求</span><span class="sxs-lookup"><span data-stu-id="580ad-176">Request</span></span>
<span data-ttu-id="580ad-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="580ad-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="580ad-178">响应</span><span class="sxs-lookup"><span data-stu-id="580ad-178">Response</span></span>
<span data-ttu-id="580ad-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="580ad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





