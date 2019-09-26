---
title: 更新 iosVppAppAssignedDeviceLicense
description: 更新 iosVppAppAssignedDeviceLicense 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0eb6a7835ff280f0267824c6d838035a5bf8fa2d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173498"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="b1d72-103">更新 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="b1d72-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="b1d72-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1d72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1d72-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1d72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1d72-106">更新[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b1d72-106">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1d72-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1d72-107">Prerequisites</span></span>
<span data-ttu-id="b1d72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1d72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1d72-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1d72-110">Permission type</span></span>|<span data-ttu-id="b1d72-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1d72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1d72-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1d72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1d72-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d72-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1d72-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1d72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1d72-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1d72-115">Not supported.</span></span>|
|<span data-ttu-id="b1d72-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1d72-116">Application</span></span>|<span data-ttu-id="b1d72-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d72-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1d72-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1d72-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="b1d72-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1d72-119">Request headers</span></span>
|<span data-ttu-id="b1d72-120">标头</span><span class="sxs-lookup"><span data-stu-id="b1d72-120">Header</span></span>|<span data-ttu-id="b1d72-121">值</span><span class="sxs-lookup"><span data-stu-id="b1d72-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1d72-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1d72-122">Authorization</span></span>|<span data-ttu-id="b1d72-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1d72-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1d72-124">接受</span><span class="sxs-lookup"><span data-stu-id="b1d72-124">Accept</span></span>|<span data-ttu-id="b1d72-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1d72-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1d72-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1d72-126">Request body</span></span>
<span data-ttu-id="b1d72-127">在请求正文中，提供[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1d72-127">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="b1d72-128">下表显示创建[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1d72-128">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="b1d72-129">属性</span><span class="sxs-lookup"><span data-stu-id="b1d72-129">Property</span></span>|<span data-ttu-id="b1d72-130">类型</span><span class="sxs-lookup"><span data-stu-id="b1d72-130">Type</span></span>|<span data-ttu-id="b1d72-131">说明</span><span class="sxs-lookup"><span data-stu-id="b1d72-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1d72-132">id</span><span class="sxs-lookup"><span data-stu-id="b1d72-132">id</span></span>|<span data-ttu-id="b1d72-133">String</span><span class="sxs-lookup"><span data-stu-id="b1d72-133">String</span></span>|<span data-ttu-id="b1d72-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b1d72-134">Key of the entity.</span></span> <span data-ttu-id="b1d72-135">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="b1d72-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="b1d72-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b1d72-136">userEmailAddress</span></span>|<span data-ttu-id="b1d72-137">String</span><span class="sxs-lookup"><span data-stu-id="b1d72-137">String</span></span>|<span data-ttu-id="b1d72-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b1d72-138">The user email address.</span></span> <span data-ttu-id="b1d72-139">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="b1d72-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="b1d72-140">userId</span><span class="sxs-lookup"><span data-stu-id="b1d72-140">userId</span></span>|<span data-ttu-id="b1d72-141">String</span><span class="sxs-lookup"><span data-stu-id="b1d72-141">String</span></span>|<span data-ttu-id="b1d72-142">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="b1d72-142">The user ID.</span></span> <span data-ttu-id="b1d72-143">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="b1d72-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="b1d72-144">userName</span><span class="sxs-lookup"><span data-stu-id="b1d72-144">userName</span></span>|<span data-ttu-id="b1d72-145">String</span><span class="sxs-lookup"><span data-stu-id="b1d72-145">String</span></span>|<span data-ttu-id="b1d72-146">用户名。</span><span class="sxs-lookup"><span data-stu-id="b1d72-146">The user name.</span></span> <span data-ttu-id="b1d72-147">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="b1d72-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="b1d72-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1d72-148">userPrincipalName</span></span>|<span data-ttu-id="b1d72-149">字符串</span><span class="sxs-lookup"><span data-stu-id="b1d72-149">String</span></span>|<span data-ttu-id="b1d72-150">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b1d72-150">The user principal name.</span></span> <span data-ttu-id="b1d72-151">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="b1d72-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="b1d72-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b1d72-152">managedDeviceId</span></span>|<span data-ttu-id="b1d72-153">String</span><span class="sxs-lookup"><span data-stu-id="b1d72-153">String</span></span>|<span data-ttu-id="b1d72-154">托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="b1d72-154">The managed device ID.</span></span>|
|<span data-ttu-id="b1d72-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="b1d72-155">deviceName</span></span>|<span data-ttu-id="b1d72-156">String</span><span class="sxs-lookup"><span data-stu-id="b1d72-156">String</span></span>|<span data-ttu-id="b1d72-157">设备名称。</span><span class="sxs-lookup"><span data-stu-id="b1d72-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="b1d72-158">响应</span><span class="sxs-lookup"><span data-stu-id="b1d72-158">Response</span></span>
<span data-ttu-id="b1d72-159">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b1d72-159">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1d72-160">示例</span><span class="sxs-lookup"><span data-stu-id="b1d72-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1d72-161">请求</span><span class="sxs-lookup"><span data-stu-id="b1d72-161">Request</span></span>
<span data-ttu-id="b1d72-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1d72-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="b1d72-163">响应</span><span class="sxs-lookup"><span data-stu-id="b1d72-163">Response</span></span>
<span data-ttu-id="b1d72-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1d72-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```




