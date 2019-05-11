---
title: 创建 androidForWorkEnrollmentProfile
description: 创建新的 androidForWorkEnrollmentProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da20ba9352dd14d1168ac76b4fb4a4f92d8d6726
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938679"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="ae3a4-103">创建 androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ae3a4-103">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="ae3a4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae3a4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae3a4-106">创建新的 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-106">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae3a4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ae3a4-107">Prerequisites</span></span>
<span data-ttu-id="ae3a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae3a4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae3a4-110">Permission type</span></span>|<span data-ttu-id="ae3a4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ae3a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae3a4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae3a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae3a4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae3a4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae3a4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae3a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae3a4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-115">Not supported.</span></span>|
|<span data-ttu-id="ae3a4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae3a4-116">Application</span></span>|<span data-ttu-id="ae3a4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae3a4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae3a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ae3a4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae3a4-119">Request headers</span></span>
|<span data-ttu-id="ae3a4-120">标头</span><span class="sxs-lookup"><span data-stu-id="ae3a4-120">Header</span></span>|<span data-ttu-id="ae3a4-121">值</span><span class="sxs-lookup"><span data-stu-id="ae3a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae3a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae3a4-122">Authorization</span></span>|<span data-ttu-id="ae3a4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae3a4-124">接受</span><span class="sxs-lookup"><span data-stu-id="ae3a4-124">Accept</span></span>|<span data-ttu-id="ae3a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae3a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae3a4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae3a4-126">Request body</span></span>
<span data-ttu-id="ae3a4-127">在请求正文中，提供 androidForWorkEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-127">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="ae3a4-128">下表显示创建 androidForWorkEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-128">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="ae3a4-129">属性</span><span class="sxs-lookup"><span data-stu-id="ae3a4-129">Property</span></span>|<span data-ttu-id="ae3a4-130">类型</span><span class="sxs-lookup"><span data-stu-id="ae3a4-130">Type</span></span>|<span data-ttu-id="ae3a4-131">说明</span><span class="sxs-lookup"><span data-stu-id="ae3a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae3a4-132">accountId</span><span class="sxs-lookup"><span data-stu-id="ae3a4-132">accountId</span></span>|<span data-ttu-id="ae3a4-133">String</span><span class="sxs-lookup"><span data-stu-id="ae3a4-133">String</span></span>|<span data-ttu-id="ae3a4-134">注册配置文件隶属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="ae3a4-135">id</span><span class="sxs-lookup"><span data-stu-id="ae3a4-135">id</span></span>|<span data-ttu-id="ae3a4-136">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3a4-136">String</span></span>|<span data-ttu-id="ae3a4-137">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="ae3a4-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ae3a4-138">displayName</span></span>|<span data-ttu-id="ae3a4-139">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3a4-139">String</span></span>|<span data-ttu-id="ae3a4-140">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="ae3a4-141">说明</span><span class="sxs-lookup"><span data-stu-id="ae3a4-141">description</span></span>|<span data-ttu-id="ae3a4-142">String</span><span class="sxs-lookup"><span data-stu-id="ae3a4-142">String</span></span>|<span data-ttu-id="ae3a4-143">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="ae3a4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3a4-144">createdDateTime</span></span>|<span data-ttu-id="ae3a4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3a4-145">DateTimeOffset</span></span>|<span data-ttu-id="ae3a4-146">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="ae3a4-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3a4-147">lastModifiedDateTime</span></span>|<span data-ttu-id="ae3a4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3a4-148">DateTimeOffset</span></span>|<span data-ttu-id="ae3a4-149">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="ae3a4-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="ae3a4-150">tokenValue</span></span>|<span data-ttu-id="ae3a4-151">String</span><span class="sxs-lookup"><span data-stu-id="ae3a4-151">String</span></span>|<span data-ttu-id="ae3a4-152">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="ae3a4-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3a4-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="ae3a4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3a4-154">DateTimeOffset</span></span>|<span data-ttu-id="ae3a4-155">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="ae3a4-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae3a4-156">enrolledDeviceCount</span></span>|<span data-ttu-id="ae3a4-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ae3a4-157">Int32</span></span>|<span data-ttu-id="ae3a4-158">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="ae3a4-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="ae3a4-159">qrCodeContent</span></span>|<span data-ttu-id="ae3a4-160">String</span><span class="sxs-lookup"><span data-stu-id="ae3a4-160">String</span></span>|<span data-ttu-id="ae3a4-161">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="ae3a4-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="ae3a4-162">qrCodeImage</span></span>|[<span data-ttu-id="ae3a4-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ae3a4-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ae3a4-164">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="ae3a4-165">响应</span><span class="sxs-lookup"><span data-stu-id="ae3a4-165">Response</span></span>
<span data-ttu-id="ae3a4-166">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-166">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae3a4-167">示例</span><span class="sxs-lookup"><span data-stu-id="ae3a4-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae3a4-168">请求</span><span class="sxs-lookup"><span data-stu-id="ae3a4-168">Request</span></span>
<span data-ttu-id="ae3a4-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="ae3a4-170">响应</span><span class="sxs-lookup"><span data-stu-id="ae3a4-170">Response</span></span>
<span data-ttu-id="ae3a4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae3a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```




