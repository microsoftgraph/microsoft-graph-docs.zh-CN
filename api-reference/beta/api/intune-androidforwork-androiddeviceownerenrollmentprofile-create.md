---
title: 创建 androidDeviceOwnerEnrollmentProfile
description: 创建新的 androidDeviceOwnerEnrollmentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 888c20a0e8b409137501695b9363019d61c732b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142397"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="bcb53-103">创建 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bcb53-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="bcb53-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bcb53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcb53-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bcb53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcb53-106">创建新的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bcb53-106">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcb53-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bcb53-107">Prerequisites</span></span>
<span data-ttu-id="bcb53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bcb53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bcb53-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcb53-110">Permission type</span></span>|<span data-ttu-id="bcb53-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bcb53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcb53-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcb53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bcb53-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcb53-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcb53-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcb53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcb53-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcb53-115">Not supported.</span></span>|
|<span data-ttu-id="bcb53-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcb53-116">Application</span></span>|<span data-ttu-id="bcb53-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcb53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcb53-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcb53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="bcb53-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcb53-119">Request headers</span></span>
|<span data-ttu-id="bcb53-120">标头</span><span class="sxs-lookup"><span data-stu-id="bcb53-120">Header</span></span>|<span data-ttu-id="bcb53-121">值</span><span class="sxs-lookup"><span data-stu-id="bcb53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcb53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcb53-122">Authorization</span></span>|<span data-ttu-id="bcb53-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bcb53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcb53-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bcb53-124">Accept</span></span>|<span data-ttu-id="bcb53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bcb53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcb53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcb53-126">Request body</span></span>
<span data-ttu-id="bcb53-127">在请求正文中, 提供 androidDeviceOwnerEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcb53-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="bcb53-128">下表显示创建 androidDeviceOwnerEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bcb53-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="bcb53-129">属性</span><span class="sxs-lookup"><span data-stu-id="bcb53-129">Property</span></span>|<span data-ttu-id="bcb53-130">类型</span><span class="sxs-lookup"><span data-stu-id="bcb53-130">Type</span></span>|<span data-ttu-id="bcb53-131">说明</span><span class="sxs-lookup"><span data-stu-id="bcb53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcb53-132">accountId</span><span class="sxs-lookup"><span data-stu-id="bcb53-132">accountId</span></span>|<span data-ttu-id="bcb53-133">String</span><span class="sxs-lookup"><span data-stu-id="bcb53-133">String</span></span>|<span data-ttu-id="bcb53-134">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="bcb53-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="bcb53-135">id</span><span class="sxs-lookup"><span data-stu-id="bcb53-135">id</span></span>|<span data-ttu-id="bcb53-136">字串符号</span><span class="sxs-lookup"><span data-stu-id="bcb53-136">String</span></span>|<span data-ttu-id="bcb53-137">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="bcb53-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="bcb53-138">displayName</span><span class="sxs-lookup"><span data-stu-id="bcb53-138">displayName</span></span>|<span data-ttu-id="bcb53-139">字符串</span><span class="sxs-lookup"><span data-stu-id="bcb53-139">String</span></span>|<span data-ttu-id="bcb53-140">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bcb53-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="bcb53-141">description</span><span class="sxs-lookup"><span data-stu-id="bcb53-141">description</span></span>|<span data-ttu-id="bcb53-142">字符串</span><span class="sxs-lookup"><span data-stu-id="bcb53-142">String</span></span>|<span data-ttu-id="bcb53-143">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="bcb53-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="bcb53-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb53-144">createdDateTime</span></span>|<span data-ttu-id="bcb53-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcb53-145">DateTimeOffset</span></span>|<span data-ttu-id="bcb53-146">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bcb53-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="bcb53-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb53-147">lastModifiedDateTime</span></span>|<span data-ttu-id="bcb53-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcb53-148">DateTimeOffset</span></span>|<span data-ttu-id="bcb53-149">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bcb53-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="bcb53-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="bcb53-150">tokenValue</span></span>|<span data-ttu-id="bcb53-151">String</span><span class="sxs-lookup"><span data-stu-id="bcb53-151">String</span></span>|<span data-ttu-id="bcb53-152">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="bcb53-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="bcb53-153">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb53-153">tokenCreationDateTime</span></span>|<span data-ttu-id="bcb53-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcb53-154">DateTimeOffset</span></span>|<span data-ttu-id="bcb53-155">创建最近创建的令牌的日期时间。</span><span class="sxs-lookup"><span data-stu-id="bcb53-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="bcb53-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb53-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="bcb53-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcb53-157">DateTimeOffset</span></span>|<span data-ttu-id="bcb53-158">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bcb53-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="bcb53-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcb53-159">enrolledDeviceCount</span></span>|<span data-ttu-id="bcb53-160">Int32</span><span class="sxs-lookup"><span data-stu-id="bcb53-160">Int32</span></span>|<span data-ttu-id="bcb53-161">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="bcb53-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="bcb53-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="bcb53-162">qrCodeContent</span></span>|<span data-ttu-id="bcb53-163">字符串</span><span class="sxs-lookup"><span data-stu-id="bcb53-163">String</span></span>|<span data-ttu-id="bcb53-164">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="bcb53-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="bcb53-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="bcb53-165">qrCodeImage</span></span>|[<span data-ttu-id="bcb53-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bcb53-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bcb53-167">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="bcb53-167">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="bcb53-168">响应</span><span class="sxs-lookup"><span data-stu-id="bcb53-168">Response</span></span>
<span data-ttu-id="bcb53-169">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bcb53-169">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcb53-170">示例</span><span class="sxs-lookup"><span data-stu-id="bcb53-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcb53-171">请求</span><span class="sxs-lookup"><span data-stu-id="bcb53-171">Request</span></span>
<span data-ttu-id="bcb53-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bcb53-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="bcb53-173">响应</span><span class="sxs-lookup"><span data-stu-id="bcb53-173">Response</span></span>
<span data-ttu-id="bcb53-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bcb53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




