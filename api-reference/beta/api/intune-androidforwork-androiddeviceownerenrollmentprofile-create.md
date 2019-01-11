---
title: 创建 androidDeviceOwnerEnrollmentProfile
description: 创建新的 androidDeviceOwnerEnrollmentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17bec37639c51bf4d22624f8d55a3d758f0c683b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883116"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="7ddc7-103">创建 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="7ddc7-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="7ddc7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ddc7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ddc7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ddc7-107">创建新的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ddc7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ddc7-108">Prerequisites</span></span>
<span data-ttu-id="7ddc7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7ddc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ddc7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ddc7-111">Permission type</span></span>|<span data-ttu-id="7ddc7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ddc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ddc7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ddc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ddc7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ddc7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ddc7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ddc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ddc7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-116">Not supported.</span></span>|
|<span data-ttu-id="7ddc7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ddc7-117">Application</span></span>|<span data-ttu-id="7ddc7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ddc7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ddc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="7ddc7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ddc7-120">Request headers</span></span>
|<span data-ttu-id="7ddc7-121">标头</span><span class="sxs-lookup"><span data-stu-id="7ddc7-121">Header</span></span>|<span data-ttu-id="7ddc7-122">值</span><span class="sxs-lookup"><span data-stu-id="7ddc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ddc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ddc7-123">Authorization</span></span>|<span data-ttu-id="7ddc7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ddc7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ddc7-125">Accept</span></span>|<span data-ttu-id="7ddc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ddc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ddc7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ddc7-127">Request body</span></span>
<span data-ttu-id="7ddc7-128">在请求正文中，提供 androidDeviceOwnerEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="7ddc7-129">下表显示时创建 androidDeviceOwnerEnrollmentProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="7ddc7-130">属性</span><span class="sxs-lookup"><span data-stu-id="7ddc7-130">Property</span></span>|<span data-ttu-id="7ddc7-131">类型</span><span class="sxs-lookup"><span data-stu-id="7ddc7-131">Type</span></span>|<span data-ttu-id="7ddc7-132">说明</span><span class="sxs-lookup"><span data-stu-id="7ddc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ddc7-133">accountId</span><span class="sxs-lookup"><span data-stu-id="7ddc7-133">accountId</span></span>|<span data-ttu-id="7ddc7-134">String</span><span class="sxs-lookup"><span data-stu-id="7ddc7-134">String</span></span>|<span data-ttu-id="7ddc7-135">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="7ddc7-136">id</span><span class="sxs-lookup"><span data-stu-id="7ddc7-136">id</span></span>|<span data-ttu-id="7ddc7-137">String</span><span class="sxs-lookup"><span data-stu-id="7ddc7-137">String</span></span>|<span data-ttu-id="7ddc7-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="7ddc7-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7ddc7-139">displayName</span></span>|<span data-ttu-id="7ddc7-140">String</span><span class="sxs-lookup"><span data-stu-id="7ddc7-140">String</span></span>|<span data-ttu-id="7ddc7-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="7ddc7-142">description</span><span class="sxs-lookup"><span data-stu-id="7ddc7-142">description</span></span>|<span data-ttu-id="7ddc7-143">String</span><span class="sxs-lookup"><span data-stu-id="7ddc7-143">String</span></span>|<span data-ttu-id="7ddc7-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="7ddc7-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ddc7-145">createdDateTime</span></span>|<span data-ttu-id="7ddc7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ddc7-146">DateTimeOffset</span></span>|<span data-ttu-id="7ddc7-147">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="7ddc7-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ddc7-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7ddc7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ddc7-149">DateTimeOffset</span></span>|<span data-ttu-id="7ddc7-150">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="7ddc7-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="7ddc7-151">tokenValue</span></span>|<span data-ttu-id="7ddc7-152">String</span><span class="sxs-lookup"><span data-stu-id="7ddc7-152">String</span></span>|<span data-ttu-id="7ddc7-153">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="7ddc7-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="7ddc7-154">tokenCreationDateTime</span></span>|<span data-ttu-id="7ddc7-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ddc7-155">DateTimeOffset</span></span>|<span data-ttu-id="7ddc7-156">创建日期时间最近创建的令牌。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="7ddc7-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7ddc7-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="7ddc7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ddc7-158">DateTimeOffset</span></span>|<span data-ttu-id="7ddc7-159">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="7ddc7-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ddc7-160">enrolledDeviceCount</span></span>|<span data-ttu-id="7ddc7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="7ddc7-161">Int32</span></span>|<span data-ttu-id="7ddc7-162">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="7ddc7-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="7ddc7-163">qrCodeContent</span></span>|<span data-ttu-id="7ddc7-164">String</span><span class="sxs-lookup"><span data-stu-id="7ddc7-164">String</span></span>|<span data-ttu-id="7ddc7-165">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="7ddc7-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="7ddc7-166">qrCodeImage</span></span>|[<span data-ttu-id="7ddc7-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7ddc7-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7ddc7-168">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="7ddc7-169">响应</span><span class="sxs-lookup"><span data-stu-id="7ddc7-169">Response</span></span>
<span data-ttu-id="7ddc7-170">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-170">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ddc7-171">示例</span><span class="sxs-lookup"><span data-stu-id="7ddc7-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ddc7-172">请求</span><span class="sxs-lookup"><span data-stu-id="7ddc7-172">Request</span></span>
<span data-ttu-id="7ddc7-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
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

### <a name="response"></a><span data-ttu-id="7ddc7-174">响应</span><span class="sxs-lookup"><span data-stu-id="7ddc7-174">Response</span></span>
<span data-ttu-id="7ddc7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ddc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 737

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
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





