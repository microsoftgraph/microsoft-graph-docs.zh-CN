---
title: 更新 androidDeviceOwnerEnrollmentProfile
description: 更新 androidDeviceOwnerEnrollmentProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 966b538b161dca2bc5c85390cab5cd8bd371b236
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413827"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="0b34a-103">更新 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0b34a-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="0b34a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0b34a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b34a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b34a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b34a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b34a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b34a-107">更新[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b34a-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b34a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b34a-108">Prerequisites</span></span>
<span data-ttu-id="0b34a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0b34a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b34a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b34a-111">Permission type</span></span>|<span data-ttu-id="0b34a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b34a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b34a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b34a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b34a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b34a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b34a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b34a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b34a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b34a-116">Not supported.</span></span>|
|<span data-ttu-id="0b34a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b34a-117">Application</span></span>|<span data-ttu-id="0b34a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b34a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b34a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b34a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0b34a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b34a-120">Request headers</span></span>
|<span data-ttu-id="0b34a-121">标头</span><span class="sxs-lookup"><span data-stu-id="0b34a-121">Header</span></span>|<span data-ttu-id="0b34a-122">值</span><span class="sxs-lookup"><span data-stu-id="0b34a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b34a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b34a-123">Authorization</span></span>|<span data-ttu-id="0b34a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b34a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b34a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b34a-125">Accept</span></span>|<span data-ttu-id="0b34a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b34a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b34a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b34a-127">Request body</span></span>
<span data-ttu-id="0b34a-128">在请求正文中，提供[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b34a-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="0b34a-129">下表显示时创建[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b34a-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="0b34a-130">属性</span><span class="sxs-lookup"><span data-stu-id="0b34a-130">Property</span></span>|<span data-ttu-id="0b34a-131">类型</span><span class="sxs-lookup"><span data-stu-id="0b34a-131">Type</span></span>|<span data-ttu-id="0b34a-132">说明</span><span class="sxs-lookup"><span data-stu-id="0b34a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b34a-133">accountId</span><span class="sxs-lookup"><span data-stu-id="0b34a-133">accountId</span></span>|<span data-ttu-id="0b34a-134">String</span><span class="sxs-lookup"><span data-stu-id="0b34a-134">String</span></span>|<span data-ttu-id="0b34a-135">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="0b34a-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="0b34a-136">id</span><span class="sxs-lookup"><span data-stu-id="0b34a-136">id</span></span>|<span data-ttu-id="0b34a-137">String</span><span class="sxs-lookup"><span data-stu-id="0b34a-137">String</span></span>|<span data-ttu-id="0b34a-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="0b34a-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="0b34a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0b34a-139">displayName</span></span>|<span data-ttu-id="0b34a-140">String</span><span class="sxs-lookup"><span data-stu-id="0b34a-140">String</span></span>|<span data-ttu-id="0b34a-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0b34a-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="0b34a-142">description</span><span class="sxs-lookup"><span data-stu-id="0b34a-142">description</span></span>|<span data-ttu-id="0b34a-143">String</span><span class="sxs-lookup"><span data-stu-id="0b34a-143">String</span></span>|<span data-ttu-id="0b34a-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="0b34a-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="0b34a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b34a-145">createdDateTime</span></span>|<span data-ttu-id="0b34a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b34a-146">DateTimeOffset</span></span>|<span data-ttu-id="0b34a-147">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b34a-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="0b34a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b34a-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0b34a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b34a-149">DateTimeOffset</span></span>|<span data-ttu-id="0b34a-150">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b34a-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="0b34a-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="0b34a-151">tokenValue</span></span>|<span data-ttu-id="0b34a-152">String</span><span class="sxs-lookup"><span data-stu-id="0b34a-152">String</span></span>|<span data-ttu-id="0b34a-153">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="0b34a-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="0b34a-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="0b34a-154">tokenCreationDateTime</span></span>|<span data-ttu-id="0b34a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b34a-155">DateTimeOffset</span></span>|<span data-ttu-id="0b34a-156">创建日期时间最近创建的令牌。</span><span class="sxs-lookup"><span data-stu-id="0b34a-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="0b34a-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0b34a-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="0b34a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b34a-158">DateTimeOffset</span></span>|<span data-ttu-id="0b34a-159">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b34a-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="0b34a-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b34a-160">enrolledDeviceCount</span></span>|<span data-ttu-id="0b34a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0b34a-161">Int32</span></span>|<span data-ttu-id="0b34a-162">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="0b34a-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="0b34a-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="0b34a-163">qrCodeContent</span></span>|<span data-ttu-id="0b34a-164">String</span><span class="sxs-lookup"><span data-stu-id="0b34a-164">String</span></span>|<span data-ttu-id="0b34a-165">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="0b34a-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="0b34a-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="0b34a-166">qrCodeImage</span></span>|[<span data-ttu-id="0b34a-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0b34a-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0b34a-168">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="0b34a-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="0b34a-169">响应</span><span class="sxs-lookup"><span data-stu-id="0b34a-169">Response</span></span>
<span data-ttu-id="0b34a-170">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b34a-170">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b34a-171">示例</span><span class="sxs-lookup"><span data-stu-id="0b34a-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b34a-172">请求</span><span class="sxs-lookup"><span data-stu-id="0b34a-172">Request</span></span>
<span data-ttu-id="0b34a-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b34a-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
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

### <a name="response"></a><span data-ttu-id="0b34a-174">响应</span><span class="sxs-lookup"><span data-stu-id="0b34a-174">Response</span></span>
<span data-ttu-id="0b34a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b34a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




