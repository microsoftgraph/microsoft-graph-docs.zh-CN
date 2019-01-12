---
title: 更新 androidDeviceOwnerEnrollmentProfile
description: 更新 androidDeviceOwnerEnrollmentProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4b8e87f44259e2bf3db9460f71a376b107d28d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921281"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="fbde0-103">更新 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="fbde0-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="fbde0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fbde0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbde0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fbde0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbde0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbde0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbde0-107">更新[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fbde0-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbde0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fbde0-108">Prerequisites</span></span>
<span data-ttu-id="fbde0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fbde0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbde0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbde0-111">Permission type</span></span>|<span data-ttu-id="fbde0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fbde0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbde0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbde0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbde0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbde0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fbde0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbde0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbde0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbde0-116">Not supported.</span></span>|
|<span data-ttu-id="fbde0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbde0-117">Application</span></span>|<span data-ttu-id="fbde0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbde0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbde0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbde0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="fbde0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbde0-120">Request headers</span></span>
|<span data-ttu-id="fbde0-121">标头</span><span class="sxs-lookup"><span data-stu-id="fbde0-121">Header</span></span>|<span data-ttu-id="fbde0-122">值</span><span class="sxs-lookup"><span data-stu-id="fbde0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbde0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbde0-123">Authorization</span></span>|<span data-ttu-id="fbde0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fbde0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbde0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbde0-125">Accept</span></span>|<span data-ttu-id="fbde0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbde0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbde0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbde0-127">Request body</span></span>
<span data-ttu-id="fbde0-128">在请求正文中，提供[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbde0-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="fbde0-129">下表显示时创建[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fbde0-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="fbde0-130">属性</span><span class="sxs-lookup"><span data-stu-id="fbde0-130">Property</span></span>|<span data-ttu-id="fbde0-131">类型</span><span class="sxs-lookup"><span data-stu-id="fbde0-131">Type</span></span>|<span data-ttu-id="fbde0-132">说明</span><span class="sxs-lookup"><span data-stu-id="fbde0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbde0-133">accountId</span><span class="sxs-lookup"><span data-stu-id="fbde0-133">accountId</span></span>|<span data-ttu-id="fbde0-134">String</span><span class="sxs-lookup"><span data-stu-id="fbde0-134">String</span></span>|<span data-ttu-id="fbde0-135">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="fbde0-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="fbde0-136">id</span><span class="sxs-lookup"><span data-stu-id="fbde0-136">id</span></span>|<span data-ttu-id="fbde0-137">String</span><span class="sxs-lookup"><span data-stu-id="fbde0-137">String</span></span>|<span data-ttu-id="fbde0-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="fbde0-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="fbde0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="fbde0-139">displayName</span></span>|<span data-ttu-id="fbde0-140">String</span><span class="sxs-lookup"><span data-stu-id="fbde0-140">String</span></span>|<span data-ttu-id="fbde0-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fbde0-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="fbde0-142">description</span><span class="sxs-lookup"><span data-stu-id="fbde0-142">description</span></span>|<span data-ttu-id="fbde0-143">String</span><span class="sxs-lookup"><span data-stu-id="fbde0-143">String</span></span>|<span data-ttu-id="fbde0-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="fbde0-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="fbde0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbde0-145">createdDateTime</span></span>|<span data-ttu-id="fbde0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbde0-146">DateTimeOffset</span></span>|<span data-ttu-id="fbde0-147">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fbde0-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="fbde0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbde0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="fbde0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbde0-149">DateTimeOffset</span></span>|<span data-ttu-id="fbde0-150">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fbde0-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="fbde0-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="fbde0-151">tokenValue</span></span>|<span data-ttu-id="fbde0-152">String</span><span class="sxs-lookup"><span data-stu-id="fbde0-152">String</span></span>|<span data-ttu-id="fbde0-153">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="fbde0-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="fbde0-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="fbde0-154">tokenCreationDateTime</span></span>|<span data-ttu-id="fbde0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbde0-155">DateTimeOffset</span></span>|<span data-ttu-id="fbde0-156">创建日期时间最近创建的令牌。</span><span class="sxs-lookup"><span data-stu-id="fbde0-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="fbde0-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fbde0-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="fbde0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbde0-158">DateTimeOffset</span></span>|<span data-ttu-id="fbde0-159">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fbde0-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="fbde0-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fbde0-160">enrolledDeviceCount</span></span>|<span data-ttu-id="fbde0-161">Int32</span><span class="sxs-lookup"><span data-stu-id="fbde0-161">Int32</span></span>|<span data-ttu-id="fbde0-162">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="fbde0-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="fbde0-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="fbde0-163">qrCodeContent</span></span>|<span data-ttu-id="fbde0-164">String</span><span class="sxs-lookup"><span data-stu-id="fbde0-164">String</span></span>|<span data-ttu-id="fbde0-165">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="fbde0-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="fbde0-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="fbde0-166">qrCodeImage</span></span>|[<span data-ttu-id="fbde0-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fbde0-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fbde0-168">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="fbde0-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="fbde0-169">响应</span><span class="sxs-lookup"><span data-stu-id="fbde0-169">Response</span></span>
<span data-ttu-id="fbde0-170">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fbde0-170">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbde0-171">示例</span><span class="sxs-lookup"><span data-stu-id="fbde0-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbde0-172">请求</span><span class="sxs-lookup"><span data-stu-id="fbde0-172">Request</span></span>
<span data-ttu-id="fbde0-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbde0-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 555

{
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

### <a name="response"></a><span data-ttu-id="fbde0-174">响应</span><span class="sxs-lookup"><span data-stu-id="fbde0-174">Response</span></span>
<span data-ttu-id="fbde0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fbde0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





