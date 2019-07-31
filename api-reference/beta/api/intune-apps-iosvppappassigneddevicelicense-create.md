---
title: 创建 iosVppAppAssignedDeviceLicense
description: 创建新的 iosVppAppAssignedDeviceLicense 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3905315c02163c3ddfeb7c8dcf92981686008af3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951489"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="7348d-103">创建 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="7348d-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="7348d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7348d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7348d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7348d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7348d-106">创建新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7348d-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7348d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7348d-107">Prerequisites</span></span>
<span data-ttu-id="7348d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7348d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7348d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7348d-110">Permission type</span></span>|<span data-ttu-id="7348d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7348d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7348d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7348d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7348d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7348d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7348d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7348d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7348d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7348d-115">Not supported.</span></span>|
|<span data-ttu-id="7348d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7348d-116">Application</span></span>|<span data-ttu-id="7348d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7348d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7348d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7348d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="7348d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7348d-119">Request headers</span></span>
|<span data-ttu-id="7348d-120">标头</span><span class="sxs-lookup"><span data-stu-id="7348d-120">Header</span></span>|<span data-ttu-id="7348d-121">值</span><span class="sxs-lookup"><span data-stu-id="7348d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7348d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7348d-122">Authorization</span></span>|<span data-ttu-id="7348d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7348d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7348d-124">接受</span><span class="sxs-lookup"><span data-stu-id="7348d-124">Accept</span></span>|<span data-ttu-id="7348d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7348d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7348d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7348d-126">Request body</span></span>
<span data-ttu-id="7348d-127">在请求正文中, 提供 iosVppAppAssignedDeviceLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7348d-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="7348d-128">下表显示创建 iosVppAppAssignedDeviceLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7348d-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="7348d-129">属性</span><span class="sxs-lookup"><span data-stu-id="7348d-129">Property</span></span>|<span data-ttu-id="7348d-130">类型</span><span class="sxs-lookup"><span data-stu-id="7348d-130">Type</span></span>|<span data-ttu-id="7348d-131">说明</span><span class="sxs-lookup"><span data-stu-id="7348d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7348d-132">id</span><span class="sxs-lookup"><span data-stu-id="7348d-132">id</span></span>|<span data-ttu-id="7348d-133">String</span><span class="sxs-lookup"><span data-stu-id="7348d-133">String</span></span>|<span data-ttu-id="7348d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7348d-134">Key of the entity.</span></span> <span data-ttu-id="7348d-135">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7348d-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7348d-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7348d-136">userEmailAddress</span></span>|<span data-ttu-id="7348d-137">String</span><span class="sxs-lookup"><span data-stu-id="7348d-137">String</span></span>|<span data-ttu-id="7348d-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7348d-138">The user email address.</span></span> <span data-ttu-id="7348d-139">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7348d-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7348d-140">userId</span><span class="sxs-lookup"><span data-stu-id="7348d-140">userId</span></span>|<span data-ttu-id="7348d-141">String</span><span class="sxs-lookup"><span data-stu-id="7348d-141">String</span></span>|<span data-ttu-id="7348d-142">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="7348d-142">The user ID.</span></span> <span data-ttu-id="7348d-143">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7348d-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7348d-144">userName</span><span class="sxs-lookup"><span data-stu-id="7348d-144">userName</span></span>|<span data-ttu-id="7348d-145">String</span><span class="sxs-lookup"><span data-stu-id="7348d-145">String</span></span>|<span data-ttu-id="7348d-146">用户名。</span><span class="sxs-lookup"><span data-stu-id="7348d-146">The user name.</span></span> <span data-ttu-id="7348d-147">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7348d-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7348d-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7348d-148">userPrincipalName</span></span>|<span data-ttu-id="7348d-149">字符串</span><span class="sxs-lookup"><span data-stu-id="7348d-149">String</span></span>|<span data-ttu-id="7348d-150">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="7348d-150">The user principal name.</span></span> <span data-ttu-id="7348d-151">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7348d-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7348d-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="7348d-152">managedDeviceId</span></span>|<span data-ttu-id="7348d-153">String</span><span class="sxs-lookup"><span data-stu-id="7348d-153">String</span></span>|<span data-ttu-id="7348d-154">托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="7348d-154">The managed device ID.</span></span>|
|<span data-ttu-id="7348d-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="7348d-155">deviceName</span></span>|<span data-ttu-id="7348d-156">String</span><span class="sxs-lookup"><span data-stu-id="7348d-156">String</span></span>|<span data-ttu-id="7348d-157">设备名称。</span><span class="sxs-lookup"><span data-stu-id="7348d-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="7348d-158">响应</span><span class="sxs-lookup"><span data-stu-id="7348d-158">Response</span></span>
<span data-ttu-id="7348d-159">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7348d-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7348d-160">示例</span><span class="sxs-lookup"><span data-stu-id="7348d-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="7348d-161">请求</span><span class="sxs-lookup"><span data-stu-id="7348d-161">Request</span></span>
<span data-ttu-id="7348d-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7348d-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7348d-163">响应</span><span class="sxs-lookup"><span data-stu-id="7348d-163">Response</span></span>
<span data-ttu-id="7348d-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7348d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





