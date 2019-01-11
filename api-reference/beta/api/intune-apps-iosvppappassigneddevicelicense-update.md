---
title: 更新 iosVppAppAssignedDeviceLicense
description: 更新 iosVppAppAssignedDeviceLicense 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8e22eed756a0c1946ae13ce6dac9cf2c63cd3a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828754"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="a7a06-103">更新 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="a7a06-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="a7a06-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a7a06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7a06-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a7a06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7a06-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7a06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7a06-107">更新[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7a06-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7a06-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7a06-108">Prerequisites</span></span>
<span data-ttu-id="a7a06-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a7a06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7a06-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7a06-111">Permission type</span></span>|<span data-ttu-id="a7a06-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7a06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7a06-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7a06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7a06-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7a06-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a7a06-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7a06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7a06-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7a06-116">Not supported.</span></span>|
|<span data-ttu-id="a7a06-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7a06-117">Application</span></span>|<span data-ttu-id="a7a06-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7a06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7a06-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7a06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="a7a06-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7a06-120">Request headers</span></span>
|<span data-ttu-id="a7a06-121">标头</span><span class="sxs-lookup"><span data-stu-id="a7a06-121">Header</span></span>|<span data-ttu-id="a7a06-122">值</span><span class="sxs-lookup"><span data-stu-id="a7a06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7a06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7a06-123">Authorization</span></span>|<span data-ttu-id="a7a06-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7a06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7a06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7a06-125">Accept</span></span>|<span data-ttu-id="a7a06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7a06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7a06-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7a06-127">Request body</span></span>
<span data-ttu-id="a7a06-128">在请求正文中，提供[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7a06-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="a7a06-129">下表显示时创建[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a7a06-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="a7a06-130">属性</span><span class="sxs-lookup"><span data-stu-id="a7a06-130">Property</span></span>|<span data-ttu-id="a7a06-131">类型</span><span class="sxs-lookup"><span data-stu-id="a7a06-131">Type</span></span>|<span data-ttu-id="a7a06-132">说明</span><span class="sxs-lookup"><span data-stu-id="a7a06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7a06-133">id</span><span class="sxs-lookup"><span data-stu-id="a7a06-133">id</span></span>|<span data-ttu-id="a7a06-134">String</span><span class="sxs-lookup"><span data-stu-id="a7a06-134">String</span></span>|<span data-ttu-id="a7a06-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a7a06-135">Key of the entity.</span></span> <span data-ttu-id="a7a06-136">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a7a06-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a7a06-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a7a06-137">userEmailAddress</span></span>|<span data-ttu-id="a7a06-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a7a06-138">String</span></span>|<span data-ttu-id="a7a06-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a7a06-139">The user email address.</span></span> <span data-ttu-id="a7a06-140">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a7a06-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a7a06-141">userId</span><span class="sxs-lookup"><span data-stu-id="a7a06-141">userId</span></span>|<span data-ttu-id="a7a06-142">String</span><span class="sxs-lookup"><span data-stu-id="a7a06-142">String</span></span>|<span data-ttu-id="a7a06-143">用户 id。</span><span class="sxs-lookup"><span data-stu-id="a7a06-143">The user ID.</span></span> <span data-ttu-id="a7a06-144">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a7a06-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a7a06-145">userName</span><span class="sxs-lookup"><span data-stu-id="a7a06-145">userName</span></span>|<span data-ttu-id="a7a06-146">String</span><span class="sxs-lookup"><span data-stu-id="a7a06-146">String</span></span>|<span data-ttu-id="a7a06-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="a7a06-147">The user name.</span></span> <span data-ttu-id="a7a06-148">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a7a06-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a7a06-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7a06-149">userPrincipalName</span></span>|<span data-ttu-id="a7a06-150">字符串</span><span class="sxs-lookup"><span data-stu-id="a7a06-150">String</span></span>|<span data-ttu-id="a7a06-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="a7a06-151">The user principal name.</span></span> <span data-ttu-id="a7a06-152">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a7a06-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a7a06-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a7a06-153">managedDeviceId</span></span>|<span data-ttu-id="a7a06-154">字符串</span><span class="sxs-lookup"><span data-stu-id="a7a06-154">String</span></span>|<span data-ttu-id="a7a06-155">托管的设备 id。</span><span class="sxs-lookup"><span data-stu-id="a7a06-155">The managed device ID.</span></span>|
|<span data-ttu-id="a7a06-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="a7a06-156">deviceName</span></span>|<span data-ttu-id="a7a06-157">String</span><span class="sxs-lookup"><span data-stu-id="a7a06-157">String</span></span>|<span data-ttu-id="a7a06-158">设备名称。</span><span class="sxs-lookup"><span data-stu-id="a7a06-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="a7a06-159">响应</span><span class="sxs-lookup"><span data-stu-id="a7a06-159">Response</span></span>
<span data-ttu-id="a7a06-160">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a7a06-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7a06-161">示例</span><span class="sxs-lookup"><span data-stu-id="a7a06-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7a06-162">请求</span><span class="sxs-lookup"><span data-stu-id="a7a06-162">Request</span></span>
<span data-ttu-id="a7a06-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7a06-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 258

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="a7a06-164">响应</span><span class="sxs-lookup"><span data-stu-id="a7a06-164">Response</span></span>
<span data-ttu-id="a7a06-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7a06-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





