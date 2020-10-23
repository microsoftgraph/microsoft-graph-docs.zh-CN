---
title: 创建 iosVppAppAssignedDeviceLicense
description: 创建新的 iosVppAppAssignedDeviceLicense 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34493235d82c4c241f6c4652ca53abdd37848177
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700134"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="969cf-103">创建 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="969cf-103">Create iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="969cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="969cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="969cf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="969cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="969cf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="969cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="969cf-107">创建新的 [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="969cf-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="969cf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="969cf-108">Prerequisites</span></span>
<span data-ttu-id="969cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="969cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969cf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="969cf-111">Permission type</span></span>|<span data-ttu-id="969cf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="969cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="969cf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="969cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="969cf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969cf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="969cf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="969cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="969cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="969cf-116">Not supported.</span></span>|
|<span data-ttu-id="969cf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="969cf-117">Application</span></span>|<span data-ttu-id="969cf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969cf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="969cf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="969cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="969cf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="969cf-120">Request headers</span></span>
|<span data-ttu-id="969cf-121">标头</span><span class="sxs-lookup"><span data-stu-id="969cf-121">Header</span></span>|<span data-ttu-id="969cf-122">值</span><span class="sxs-lookup"><span data-stu-id="969cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="969cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="969cf-123">Authorization</span></span>|<span data-ttu-id="969cf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="969cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="969cf-125">接受</span><span class="sxs-lookup"><span data-stu-id="969cf-125">Accept</span></span>|<span data-ttu-id="969cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="969cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="969cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="969cf-127">Request body</span></span>
<span data-ttu-id="969cf-128">在请求正文中，提供 iosVppAppAssignedDeviceLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="969cf-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="969cf-129">下表显示创建 iosVppAppAssignedDeviceLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="969cf-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="969cf-130">属性</span><span class="sxs-lookup"><span data-stu-id="969cf-130">Property</span></span>|<span data-ttu-id="969cf-131">类型</span><span class="sxs-lookup"><span data-stu-id="969cf-131">Type</span></span>|<span data-ttu-id="969cf-132">说明</span><span class="sxs-lookup"><span data-stu-id="969cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="969cf-133">id</span><span class="sxs-lookup"><span data-stu-id="969cf-133">id</span></span>|<span data-ttu-id="969cf-134">String</span><span class="sxs-lookup"><span data-stu-id="969cf-134">String</span></span>|<span data-ttu-id="969cf-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="969cf-135">Key of the entity.</span></span> <span data-ttu-id="969cf-136">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="969cf-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="969cf-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="969cf-137">userEmailAddress</span></span>|<span data-ttu-id="969cf-138">String</span><span class="sxs-lookup"><span data-stu-id="969cf-138">String</span></span>|<span data-ttu-id="969cf-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="969cf-139">The user email address.</span></span> <span data-ttu-id="969cf-140">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="969cf-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="969cf-141">userId</span><span class="sxs-lookup"><span data-stu-id="969cf-141">userId</span></span>|<span data-ttu-id="969cf-142">String</span><span class="sxs-lookup"><span data-stu-id="969cf-142">String</span></span>|<span data-ttu-id="969cf-143">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="969cf-143">The user ID.</span></span> <span data-ttu-id="969cf-144">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="969cf-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="969cf-145">userName</span><span class="sxs-lookup"><span data-stu-id="969cf-145">userName</span></span>|<span data-ttu-id="969cf-146">String</span><span class="sxs-lookup"><span data-stu-id="969cf-146">String</span></span>|<span data-ttu-id="969cf-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="969cf-147">The user name.</span></span> <span data-ttu-id="969cf-148">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="969cf-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="969cf-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="969cf-149">userPrincipalName</span></span>|<span data-ttu-id="969cf-150">String</span><span class="sxs-lookup"><span data-stu-id="969cf-150">String</span></span>|<span data-ttu-id="969cf-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="969cf-151">The user principal name.</span></span> <span data-ttu-id="969cf-152">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="969cf-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="969cf-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="969cf-153">managedDeviceId</span></span>|<span data-ttu-id="969cf-154">String</span><span class="sxs-lookup"><span data-stu-id="969cf-154">String</span></span>|<span data-ttu-id="969cf-155">托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="969cf-155">The managed device ID.</span></span>|
|<span data-ttu-id="969cf-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="969cf-156">deviceName</span></span>|<span data-ttu-id="969cf-157">String</span><span class="sxs-lookup"><span data-stu-id="969cf-157">String</span></span>|<span data-ttu-id="969cf-158">设备名称。</span><span class="sxs-lookup"><span data-stu-id="969cf-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="969cf-159">响应</span><span class="sxs-lookup"><span data-stu-id="969cf-159">Response</span></span>
<span data-ttu-id="969cf-160">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="969cf-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969cf-161">示例</span><span class="sxs-lookup"><span data-stu-id="969cf-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="969cf-162">请求</span><span class="sxs-lookup"><span data-stu-id="969cf-162">Request</span></span>
<span data-ttu-id="969cf-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="969cf-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="969cf-164">响应</span><span class="sxs-lookup"><span data-stu-id="969cf-164">Response</span></span>
<span data-ttu-id="969cf-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="969cf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





