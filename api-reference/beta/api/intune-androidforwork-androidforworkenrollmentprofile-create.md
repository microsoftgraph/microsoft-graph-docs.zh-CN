---
title: 创建 androidForWorkEnrollmentProfile
description: 创建新的 androidForWorkEnrollmentProfile 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 87079cc940967f84ba66c14740b8c93f8f73ca9e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417509"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="e73ce-103">创建 androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e73ce-103">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="e73ce-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e73ce-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e73ce-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e73ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e73ce-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e73ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e73ce-107">创建新的 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e73ce-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e73ce-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e73ce-108">Prerequisites</span></span>
<span data-ttu-id="e73ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e73ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e73ce-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e73ce-111">Permission type</span></span>|<span data-ttu-id="e73ce-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e73ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e73ce-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e73ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e73ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e73ce-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e73ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e73ce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e73ce-116">Not supported.</span></span>|
|<span data-ttu-id="e73ce-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e73ce-117">Application</span></span>|<span data-ttu-id="e73ce-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e73ce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e73ce-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e73ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e73ce-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e73ce-120">Request headers</span></span>
|<span data-ttu-id="e73ce-121">标头</span><span class="sxs-lookup"><span data-stu-id="e73ce-121">Header</span></span>|<span data-ttu-id="e73ce-122">值</span><span class="sxs-lookup"><span data-stu-id="e73ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e73ce-123">授权</span><span class="sxs-lookup"><span data-stu-id="e73ce-123">Authorization</span></span>|<span data-ttu-id="e73ce-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e73ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e73ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e73ce-125">Accept</span></span>|<span data-ttu-id="e73ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e73ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e73ce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e73ce-127">Request body</span></span>
<span data-ttu-id="e73ce-128">在请求正文中，提供 androidForWorkEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e73ce-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="e73ce-129">下表显示创建 androidForWorkEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e73ce-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="e73ce-130">属性</span><span class="sxs-lookup"><span data-stu-id="e73ce-130">Property</span></span>|<span data-ttu-id="e73ce-131">类型</span><span class="sxs-lookup"><span data-stu-id="e73ce-131">Type</span></span>|<span data-ttu-id="e73ce-132">说明</span><span class="sxs-lookup"><span data-stu-id="e73ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e73ce-133">accountId</span><span class="sxs-lookup"><span data-stu-id="e73ce-133">accountId</span></span>|<span data-ttu-id="e73ce-134">String</span><span class="sxs-lookup"><span data-stu-id="e73ce-134">String</span></span>|<span data-ttu-id="e73ce-135">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="e73ce-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="e73ce-136">id</span><span class="sxs-lookup"><span data-stu-id="e73ce-136">id</span></span>|<span data-ttu-id="e73ce-137">String</span><span class="sxs-lookup"><span data-stu-id="e73ce-137">String</span></span>|<span data-ttu-id="e73ce-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="e73ce-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="e73ce-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e73ce-139">displayName</span></span>|<span data-ttu-id="e73ce-140">String</span><span class="sxs-lookup"><span data-stu-id="e73ce-140">String</span></span>|<span data-ttu-id="e73ce-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e73ce-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="e73ce-142">description</span><span class="sxs-lookup"><span data-stu-id="e73ce-142">description</span></span>|<span data-ttu-id="e73ce-143">String</span><span class="sxs-lookup"><span data-stu-id="e73ce-143">String</span></span>|<span data-ttu-id="e73ce-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="e73ce-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="e73ce-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e73ce-145">createdDateTime</span></span>|<span data-ttu-id="e73ce-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e73ce-146">DateTimeOffset</span></span>|<span data-ttu-id="e73ce-147">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e73ce-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="e73ce-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e73ce-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e73ce-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e73ce-149">DateTimeOffset</span></span>|<span data-ttu-id="e73ce-150">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e73ce-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="e73ce-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="e73ce-151">tokenValue</span></span>|<span data-ttu-id="e73ce-152">String</span><span class="sxs-lookup"><span data-stu-id="e73ce-152">String</span></span>|<span data-ttu-id="e73ce-153">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="e73ce-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="e73ce-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e73ce-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="e73ce-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e73ce-155">DateTimeOffset</span></span>|<span data-ttu-id="e73ce-156">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e73ce-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="e73ce-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e73ce-157">enrolledDeviceCount</span></span>|<span data-ttu-id="e73ce-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e73ce-158">Int32</span></span>|<span data-ttu-id="e73ce-159">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="e73ce-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="e73ce-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e73ce-160">qrCodeContent</span></span>|<span data-ttu-id="e73ce-161">String</span><span class="sxs-lookup"><span data-stu-id="e73ce-161">String</span></span>|<span data-ttu-id="e73ce-162">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="e73ce-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e73ce-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e73ce-163">qrCodeImage</span></span>|[<span data-ttu-id="e73ce-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e73ce-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e73ce-165">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="e73ce-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="e73ce-166">响应</span><span class="sxs-lookup"><span data-stu-id="e73ce-166">Response</span></span>
<span data-ttu-id="e73ce-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e73ce-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e73ce-168">示例</span><span class="sxs-lookup"><span data-stu-id="e73ce-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="e73ce-169">请求</span><span class="sxs-lookup"><span data-stu-id="e73ce-169">Request</span></span>
<span data-ttu-id="e73ce-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e73ce-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e73ce-171">响应</span><span class="sxs-lookup"><span data-stu-id="e73ce-171">Response</span></span>
<span data-ttu-id="e73ce-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e73ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




