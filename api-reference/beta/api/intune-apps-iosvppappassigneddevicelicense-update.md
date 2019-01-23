---
title: 更新 iosVppAppAssignedDeviceLicense
description: 更新 iosVppAppAssignedDeviceLicense 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2edd886b0ab9b302e7f224511bb329fe8269a7d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402123"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="48e2f-103">更新 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="48e2f-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="48e2f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="48e2f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48e2f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48e2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48e2f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48e2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48e2f-107">更新[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48e2f-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48e2f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="48e2f-108">Prerequisites</span></span>
<span data-ttu-id="48e2f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="48e2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48e2f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48e2f-111">Permission type</span></span>|<span data-ttu-id="48e2f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48e2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48e2f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48e2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48e2f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e2f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48e2f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48e2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48e2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48e2f-116">Not supported.</span></span>|
|<span data-ttu-id="48e2f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48e2f-117">Application</span></span>|<span data-ttu-id="48e2f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="48e2f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48e2f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48e2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="48e2f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="48e2f-120">Request headers</span></span>
|<span data-ttu-id="48e2f-121">标头</span><span class="sxs-lookup"><span data-stu-id="48e2f-121">Header</span></span>|<span data-ttu-id="48e2f-122">值</span><span class="sxs-lookup"><span data-stu-id="48e2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48e2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48e2f-123">Authorization</span></span>|<span data-ttu-id="48e2f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48e2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48e2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48e2f-125">Accept</span></span>|<span data-ttu-id="48e2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48e2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e2f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="48e2f-127">Request body</span></span>
<span data-ttu-id="48e2f-128">在请求正文中，提供[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48e2f-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="48e2f-129">下表显示时创建[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="48e2f-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="48e2f-130">属性</span><span class="sxs-lookup"><span data-stu-id="48e2f-130">Property</span></span>|<span data-ttu-id="48e2f-131">类型</span><span class="sxs-lookup"><span data-stu-id="48e2f-131">Type</span></span>|<span data-ttu-id="48e2f-132">说明</span><span class="sxs-lookup"><span data-stu-id="48e2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e2f-133">id</span><span class="sxs-lookup"><span data-stu-id="48e2f-133">id</span></span>|<span data-ttu-id="48e2f-134">String</span><span class="sxs-lookup"><span data-stu-id="48e2f-134">String</span></span>|<span data-ttu-id="48e2f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48e2f-135">Key of the entity.</span></span> <span data-ttu-id="48e2f-136">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="48e2f-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="48e2f-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="48e2f-137">userEmailAddress</span></span>|<span data-ttu-id="48e2f-138">String</span><span class="sxs-lookup"><span data-stu-id="48e2f-138">String</span></span>|<span data-ttu-id="48e2f-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="48e2f-139">The user email address.</span></span> <span data-ttu-id="48e2f-140">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="48e2f-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="48e2f-141">userId</span><span class="sxs-lookup"><span data-stu-id="48e2f-141">userId</span></span>|<span data-ttu-id="48e2f-142">String</span><span class="sxs-lookup"><span data-stu-id="48e2f-142">String</span></span>|<span data-ttu-id="48e2f-143">用户 id。</span><span class="sxs-lookup"><span data-stu-id="48e2f-143">The user ID.</span></span> <span data-ttu-id="48e2f-144">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="48e2f-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="48e2f-145">userName</span><span class="sxs-lookup"><span data-stu-id="48e2f-145">userName</span></span>|<span data-ttu-id="48e2f-146">String</span><span class="sxs-lookup"><span data-stu-id="48e2f-146">String</span></span>|<span data-ttu-id="48e2f-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="48e2f-147">The user name.</span></span> <span data-ttu-id="48e2f-148">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="48e2f-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="48e2f-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="48e2f-149">userPrincipalName</span></span>|<span data-ttu-id="48e2f-150">String</span><span class="sxs-lookup"><span data-stu-id="48e2f-150">String</span></span>|<span data-ttu-id="48e2f-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="48e2f-151">The user principal name.</span></span> <span data-ttu-id="48e2f-152">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="48e2f-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="48e2f-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="48e2f-153">managedDeviceId</span></span>|<span data-ttu-id="48e2f-154">String</span><span class="sxs-lookup"><span data-stu-id="48e2f-154">String</span></span>|<span data-ttu-id="48e2f-155">托管的设备 id。</span><span class="sxs-lookup"><span data-stu-id="48e2f-155">The managed device ID.</span></span>|
|<span data-ttu-id="48e2f-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="48e2f-156">deviceName</span></span>|<span data-ttu-id="48e2f-157">String</span><span class="sxs-lookup"><span data-stu-id="48e2f-157">String</span></span>|<span data-ttu-id="48e2f-158">设备名称。</span><span class="sxs-lookup"><span data-stu-id="48e2f-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="48e2f-159">响应</span><span class="sxs-lookup"><span data-stu-id="48e2f-159">Response</span></span>
<span data-ttu-id="48e2f-160">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="48e2f-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48e2f-161">示例</span><span class="sxs-lookup"><span data-stu-id="48e2f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="48e2f-162">请求</span><span class="sxs-lookup"><span data-stu-id="48e2f-162">Request</span></span>
<span data-ttu-id="48e2f-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48e2f-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48e2f-164">响应</span><span class="sxs-lookup"><span data-stu-id="48e2f-164">Response</span></span>
<span data-ttu-id="48e2f-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48e2f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




