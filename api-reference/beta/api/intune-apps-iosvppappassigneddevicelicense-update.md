---
title: 更新 iosVppAppAssignedDeviceLicense
description: 更新 iosVppAppAssignedDeviceLicense 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6943f72e7af2d4dbcaaf3b55f04f918cd3abbe6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39925464"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="e15bb-103">更新 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="e15bb-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="e15bb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e15bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e15bb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e15bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e15bb-106">更新[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e15bb-106">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e15bb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e15bb-107">Prerequisites</span></span>
<span data-ttu-id="e15bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e15bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e15bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e15bb-110">Permission type</span></span>|<span data-ttu-id="e15bb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e15bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e15bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e15bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e15bb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15bb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e15bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e15bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e15bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e15bb-115">Not supported.</span></span>|
|<span data-ttu-id="e15bb-116">Application</span><span class="sxs-lookup"><span data-stu-id="e15bb-116">Application</span></span>|<span data-ttu-id="e15bb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15bb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e15bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e15bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="e15bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e15bb-119">Request headers</span></span>
|<span data-ttu-id="e15bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="e15bb-120">Header</span></span>|<span data-ttu-id="e15bb-121">值</span><span class="sxs-lookup"><span data-stu-id="e15bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e15bb-122">授权</span><span class="sxs-lookup"><span data-stu-id="e15bb-122">Authorization</span></span>|<span data-ttu-id="e15bb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e15bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e15bb-124">接受</span><span class="sxs-lookup"><span data-stu-id="e15bb-124">Accept</span></span>|<span data-ttu-id="e15bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e15bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e15bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e15bb-126">Request body</span></span>
<span data-ttu-id="e15bb-127">在请求正文中，提供[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e15bb-127">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="e15bb-128">下表显示创建[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e15bb-128">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="e15bb-129">属性</span><span class="sxs-lookup"><span data-stu-id="e15bb-129">Property</span></span>|<span data-ttu-id="e15bb-130">类型</span><span class="sxs-lookup"><span data-stu-id="e15bb-130">Type</span></span>|<span data-ttu-id="e15bb-131">说明</span><span class="sxs-lookup"><span data-stu-id="e15bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e15bb-132">id</span><span class="sxs-lookup"><span data-stu-id="e15bb-132">id</span></span>|<span data-ttu-id="e15bb-133">String</span><span class="sxs-lookup"><span data-stu-id="e15bb-133">String</span></span>|<span data-ttu-id="e15bb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e15bb-134">Key of the entity.</span></span> <span data-ttu-id="e15bb-135">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e15bb-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e15bb-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e15bb-136">userEmailAddress</span></span>|<span data-ttu-id="e15bb-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e15bb-137">String</span></span>|<span data-ttu-id="e15bb-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e15bb-138">The user email address.</span></span> <span data-ttu-id="e15bb-139">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e15bb-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e15bb-140">userId</span><span class="sxs-lookup"><span data-stu-id="e15bb-140">userId</span></span>|<span data-ttu-id="e15bb-141">String</span><span class="sxs-lookup"><span data-stu-id="e15bb-141">String</span></span>|<span data-ttu-id="e15bb-142">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="e15bb-142">The user ID.</span></span> <span data-ttu-id="e15bb-143">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e15bb-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e15bb-144">userName</span><span class="sxs-lookup"><span data-stu-id="e15bb-144">userName</span></span>|<span data-ttu-id="e15bb-145">String</span><span class="sxs-lookup"><span data-stu-id="e15bb-145">String</span></span>|<span data-ttu-id="e15bb-146">用户名。</span><span class="sxs-lookup"><span data-stu-id="e15bb-146">The user name.</span></span> <span data-ttu-id="e15bb-147">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e15bb-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e15bb-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e15bb-148">userPrincipalName</span></span>|<span data-ttu-id="e15bb-149">字符串</span><span class="sxs-lookup"><span data-stu-id="e15bb-149">String</span></span>|<span data-ttu-id="e15bb-150">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="e15bb-150">The user principal name.</span></span> <span data-ttu-id="e15bb-151">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e15bb-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e15bb-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="e15bb-152">managedDeviceId</span></span>|<span data-ttu-id="e15bb-153">字符串</span><span class="sxs-lookup"><span data-stu-id="e15bb-153">String</span></span>|<span data-ttu-id="e15bb-154">托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="e15bb-154">The managed device ID.</span></span>|
|<span data-ttu-id="e15bb-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="e15bb-155">deviceName</span></span>|<span data-ttu-id="e15bb-156">字符串</span><span class="sxs-lookup"><span data-stu-id="e15bb-156">String</span></span>|<span data-ttu-id="e15bb-157">设备名称。</span><span class="sxs-lookup"><span data-stu-id="e15bb-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="e15bb-158">响应</span><span class="sxs-lookup"><span data-stu-id="e15bb-158">Response</span></span>
<span data-ttu-id="e15bb-159">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e15bb-159">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e15bb-160">示例</span><span class="sxs-lookup"><span data-stu-id="e15bb-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="e15bb-161">请求</span><span class="sxs-lookup"><span data-stu-id="e15bb-161">Request</span></span>
<span data-ttu-id="e15bb-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e15bb-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e15bb-163">响应</span><span class="sxs-lookup"><span data-stu-id="e15bb-163">Response</span></span>
<span data-ttu-id="e15bb-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e15bb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





