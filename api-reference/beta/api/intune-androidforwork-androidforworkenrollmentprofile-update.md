---
title: 更新 androidForWorkEnrollmentProfile
description: 更新 androidForWorkEnrollmentProfile 对象的属性。
ms.openlocfilehash: f0af5db7115de09657d08d093836527e3198cad0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047433"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="ac8c0-103">更新 androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ac8c0-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="ac8c0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac8c0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac8c0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac8c0-107">更新 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac8c0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ac8c0-108">Prerequisites</span></span>
<span data-ttu-id="ac8c0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ac8c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac8c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac8c0-111">Permission type</span></span>|<span data-ttu-id="ac8c0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ac8c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac8c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac8c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac8c0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac8c0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac8c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac8c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac8c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-116">Not supported.</span></span>|
|<span data-ttu-id="ac8c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac8c0-117">Application</span></span>|<span data-ttu-id="ac8c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac8c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac8c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="ac8c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac8c0-120">Request headers</span></span>
|<span data-ttu-id="ac8c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="ac8c0-121">Header</span></span>|<span data-ttu-id="ac8c0-122">值</span><span class="sxs-lookup"><span data-stu-id="ac8c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac8c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac8c0-123">Authorization</span></span>|<span data-ttu-id="ac8c0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac8c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac8c0-125">Accept</span></span>|<span data-ttu-id="ac8c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac8c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac8c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac8c0-127">Request body</span></span>
<span data-ttu-id="ac8c0-128">在请求正文中，提供 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="ac8c0-129">下表显示创建 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="ac8c0-130">属性</span><span class="sxs-lookup"><span data-stu-id="ac8c0-130">Property</span></span>|<span data-ttu-id="ac8c0-131">类型</span><span class="sxs-lookup"><span data-stu-id="ac8c0-131">Type</span></span>|<span data-ttu-id="ac8c0-132">说明</span><span class="sxs-lookup"><span data-stu-id="ac8c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac8c0-133">accountId</span><span class="sxs-lookup"><span data-stu-id="ac8c0-133">accountId</span></span>|<span data-ttu-id="ac8c0-134">String</span><span class="sxs-lookup"><span data-stu-id="ac8c0-134">String</span></span>|<span data-ttu-id="ac8c0-135">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="ac8c0-136">id</span><span class="sxs-lookup"><span data-stu-id="ac8c0-136">id</span></span>|<span data-ttu-id="ac8c0-137">String</span><span class="sxs-lookup"><span data-stu-id="ac8c0-137">String</span></span>|<span data-ttu-id="ac8c0-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="ac8c0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ac8c0-139">displayName</span></span>|<span data-ttu-id="ac8c0-140">String</span><span class="sxs-lookup"><span data-stu-id="ac8c0-140">String</span></span>|<span data-ttu-id="ac8c0-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="ac8c0-142">description</span><span class="sxs-lookup"><span data-stu-id="ac8c0-142">description</span></span>|<span data-ttu-id="ac8c0-143">String</span><span class="sxs-lookup"><span data-stu-id="ac8c0-143">String</span></span>|<span data-ttu-id="ac8c0-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="ac8c0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac8c0-145">createdDateTime</span></span>|<span data-ttu-id="ac8c0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac8c0-146">DateTimeOffset</span></span>|<span data-ttu-id="ac8c0-147">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="ac8c0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac8c0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ac8c0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac8c0-149">DateTimeOffset</span></span>|<span data-ttu-id="ac8c0-150">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="ac8c0-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="ac8c0-151">tokenValue</span></span>|<span data-ttu-id="ac8c0-152">String</span><span class="sxs-lookup"><span data-stu-id="ac8c0-152">String</span></span>|<span data-ttu-id="ac8c0-153">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="ac8c0-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ac8c0-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="ac8c0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac8c0-155">DateTimeOffset</span></span>|<span data-ttu-id="ac8c0-156">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="ac8c0-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac8c0-157">enrolledDeviceCount</span></span>|<span data-ttu-id="ac8c0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ac8c0-158">Int32</span></span>|<span data-ttu-id="ac8c0-159">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="ac8c0-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="ac8c0-160">qrCodeContent</span></span>|<span data-ttu-id="ac8c0-161">String</span><span class="sxs-lookup"><span data-stu-id="ac8c0-161">String</span></span>|<span data-ttu-id="ac8c0-162">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="ac8c0-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="ac8c0-163">qrCodeImage</span></span>|[<span data-ttu-id="ac8c0-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ac8c0-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ac8c0-165">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="ac8c0-166">响应</span><span class="sxs-lookup"><span data-stu-id="ac8c0-166">Response</span></span>
<span data-ttu-id="ac8c0-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac8c0-168">示例</span><span class="sxs-lookup"><span data-stu-id="ac8c0-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac8c0-169">请求</span><span class="sxs-lookup"><span data-stu-id="ac8c0-169">Request</span></span>
<span data-ttu-id="ac8c0-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 490

{
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="ac8c0-171">响应</span><span class="sxs-lookup"><span data-stu-id="ac8c0-171">Response</span></span>
<span data-ttu-id="ac8c0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac8c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





