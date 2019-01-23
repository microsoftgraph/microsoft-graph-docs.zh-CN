---
title: 创建 iosVppAppAssignedDeviceLicense
description: 创建新的 iosVppAppAssignedDeviceLicense 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2806e6db550068f46e943f03baca96647176912a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410467"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="e0904-103">创建 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="e0904-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="e0904-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e0904-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0904-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0904-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0904-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0904-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0904-107">创建新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0904-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0904-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0904-108">Prerequisites</span></span>
<span data-ttu-id="e0904-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e0904-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e0904-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0904-111">Permission type</span></span>|<span data-ttu-id="e0904-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0904-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0904-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0904-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0904-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0904-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0904-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0904-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0904-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0904-116">Not supported.</span></span>|
|<span data-ttu-id="e0904-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0904-117">Application</span></span>|<span data-ttu-id="e0904-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0904-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0904-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0904-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="e0904-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0904-120">Request headers</span></span>
|<span data-ttu-id="e0904-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0904-121">Header</span></span>|<span data-ttu-id="e0904-122">值</span><span class="sxs-lookup"><span data-stu-id="e0904-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0904-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0904-123">Authorization</span></span>|<span data-ttu-id="e0904-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0904-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0904-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0904-125">Accept</span></span>|<span data-ttu-id="e0904-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0904-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0904-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0904-127">Request body</span></span>
<span data-ttu-id="e0904-128">在请求正文中，提供 iosVppAppAssignedDeviceLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0904-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="e0904-129">下表显示时创建 iosVppAppAssignedDeviceLicense 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0904-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="e0904-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0904-130">Property</span></span>|<span data-ttu-id="e0904-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0904-131">Type</span></span>|<span data-ttu-id="e0904-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0904-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0904-133">id</span><span class="sxs-lookup"><span data-stu-id="e0904-133">id</span></span>|<span data-ttu-id="e0904-134">String</span><span class="sxs-lookup"><span data-stu-id="e0904-134">String</span></span>|<span data-ttu-id="e0904-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0904-135">Key of the entity.</span></span> <span data-ttu-id="e0904-136">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e0904-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e0904-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e0904-137">userEmailAddress</span></span>|<span data-ttu-id="e0904-138">String</span><span class="sxs-lookup"><span data-stu-id="e0904-138">String</span></span>|<span data-ttu-id="e0904-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e0904-139">The user email address.</span></span> <span data-ttu-id="e0904-140">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e0904-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e0904-141">userId</span><span class="sxs-lookup"><span data-stu-id="e0904-141">userId</span></span>|<span data-ttu-id="e0904-142">String</span><span class="sxs-lookup"><span data-stu-id="e0904-142">String</span></span>|<span data-ttu-id="e0904-143">用户 id。</span><span class="sxs-lookup"><span data-stu-id="e0904-143">The user ID.</span></span> <span data-ttu-id="e0904-144">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e0904-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e0904-145">userName</span><span class="sxs-lookup"><span data-stu-id="e0904-145">userName</span></span>|<span data-ttu-id="e0904-146">String</span><span class="sxs-lookup"><span data-stu-id="e0904-146">String</span></span>|<span data-ttu-id="e0904-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="e0904-147">The user name.</span></span> <span data-ttu-id="e0904-148">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e0904-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e0904-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e0904-149">userPrincipalName</span></span>|<span data-ttu-id="e0904-150">String</span><span class="sxs-lookup"><span data-stu-id="e0904-150">String</span></span>|<span data-ttu-id="e0904-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="e0904-151">The user principal name.</span></span> <span data-ttu-id="e0904-152">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e0904-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e0904-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="e0904-153">managedDeviceId</span></span>|<span data-ttu-id="e0904-154">String</span><span class="sxs-lookup"><span data-stu-id="e0904-154">String</span></span>|<span data-ttu-id="e0904-155">托管的设备 id。</span><span class="sxs-lookup"><span data-stu-id="e0904-155">The managed device ID.</span></span>|
|<span data-ttu-id="e0904-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="e0904-156">deviceName</span></span>|<span data-ttu-id="e0904-157">String</span><span class="sxs-lookup"><span data-stu-id="e0904-157">String</span></span>|<span data-ttu-id="e0904-158">设备名称。</span><span class="sxs-lookup"><span data-stu-id="e0904-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="e0904-159">响应</span><span class="sxs-lookup"><span data-stu-id="e0904-159">Response</span></span>
<span data-ttu-id="e0904-160">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0904-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0904-161">示例</span><span class="sxs-lookup"><span data-stu-id="e0904-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0904-162">请求</span><span class="sxs-lookup"><span data-stu-id="e0904-162">Request</span></span>
<span data-ttu-id="e0904-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0904-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="e0904-164">响应</span><span class="sxs-lookup"><span data-stu-id="e0904-164">Response</span></span>
<span data-ttu-id="e0904-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0904-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




