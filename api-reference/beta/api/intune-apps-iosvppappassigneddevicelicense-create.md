---
title: 创建 iosVppAppAssignedDeviceLicense
description: 创建新的 iosVppAppAssignedDeviceLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ced922ee489e1f17f6b33df4a2807fee776fe0ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495636"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="79ece-103">创建 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="79ece-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="79ece-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79ece-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79ece-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79ece-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ece-106">创建新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79ece-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79ece-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="79ece-107">Prerequisites</span></span>
<span data-ttu-id="79ece-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79ece-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79ece-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79ece-110">Permission type</span></span>|<span data-ttu-id="79ece-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79ece-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79ece-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79ece-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79ece-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79ece-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79ece-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79ece-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79ece-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79ece-115">Not supported.</span></span>|
|<span data-ttu-id="79ece-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79ece-116">Application</span></span>|<span data-ttu-id="79ece-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="79ece-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79ece-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79ece-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="79ece-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="79ece-119">Request headers</span></span>
|<span data-ttu-id="79ece-120">标头</span><span class="sxs-lookup"><span data-stu-id="79ece-120">Header</span></span>|<span data-ttu-id="79ece-121">值</span><span class="sxs-lookup"><span data-stu-id="79ece-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79ece-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79ece-122">Authorization</span></span>|<span data-ttu-id="79ece-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79ece-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79ece-124">接受</span><span class="sxs-lookup"><span data-stu-id="79ece-124">Accept</span></span>|<span data-ttu-id="79ece-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79ece-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ece-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="79ece-126">Request body</span></span>
<span data-ttu-id="79ece-127">在请求正文中, 提供 iosVppAppAssignedDeviceLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79ece-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="79ece-128">下表显示创建 iosVppAppAssignedDeviceLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="79ece-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="79ece-129">属性</span><span class="sxs-lookup"><span data-stu-id="79ece-129">Property</span></span>|<span data-ttu-id="79ece-130">类型</span><span class="sxs-lookup"><span data-stu-id="79ece-130">Type</span></span>|<span data-ttu-id="79ece-131">说明</span><span class="sxs-lookup"><span data-stu-id="79ece-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ece-132">id</span><span class="sxs-lookup"><span data-stu-id="79ece-132">id</span></span>|<span data-ttu-id="79ece-133">String</span><span class="sxs-lookup"><span data-stu-id="79ece-133">String</span></span>|<span data-ttu-id="79ece-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="79ece-134">Key of the entity.</span></span> <span data-ttu-id="79ece-135">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79ece-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79ece-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="79ece-136">userEmailAddress</span></span>|<span data-ttu-id="79ece-137">字符串</span><span class="sxs-lookup"><span data-stu-id="79ece-137">String</span></span>|<span data-ttu-id="79ece-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="79ece-138">The user email address.</span></span> <span data-ttu-id="79ece-139">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79ece-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79ece-140">userId</span><span class="sxs-lookup"><span data-stu-id="79ece-140">userId</span></span>|<span data-ttu-id="79ece-141">字符串</span><span class="sxs-lookup"><span data-stu-id="79ece-141">String</span></span>|<span data-ttu-id="79ece-142">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="79ece-142">The user ID.</span></span> <span data-ttu-id="79ece-143">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79ece-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79ece-144">userName</span><span class="sxs-lookup"><span data-stu-id="79ece-144">userName</span></span>|<span data-ttu-id="79ece-145">String</span><span class="sxs-lookup"><span data-stu-id="79ece-145">String</span></span>|<span data-ttu-id="79ece-146">用户名。</span><span class="sxs-lookup"><span data-stu-id="79ece-146">The user name.</span></span> <span data-ttu-id="79ece-147">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79ece-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79ece-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79ece-148">userPrincipalName</span></span>|<span data-ttu-id="79ece-149">String</span><span class="sxs-lookup"><span data-stu-id="79ece-149">String</span></span>|<span data-ttu-id="79ece-150">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="79ece-150">The user principal name.</span></span> <span data-ttu-id="79ece-151">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79ece-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79ece-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="79ece-152">managedDeviceId</span></span>|<span data-ttu-id="79ece-153">字符串</span><span class="sxs-lookup"><span data-stu-id="79ece-153">String</span></span>|<span data-ttu-id="79ece-154">托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="79ece-154">The managed device ID.</span></span>|
|<span data-ttu-id="79ece-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="79ece-155">deviceName</span></span>|<span data-ttu-id="79ece-156">字符串</span><span class="sxs-lookup"><span data-stu-id="79ece-156">String</span></span>|<span data-ttu-id="79ece-157">设备名称。</span><span class="sxs-lookup"><span data-stu-id="79ece-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="79ece-158">响应</span><span class="sxs-lookup"><span data-stu-id="79ece-158">Response</span></span>
<span data-ttu-id="79ece-159">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79ece-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79ece-160">示例</span><span class="sxs-lookup"><span data-stu-id="79ece-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="79ece-161">请求</span><span class="sxs-lookup"><span data-stu-id="79ece-161">Request</span></span>
<span data-ttu-id="79ece-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79ece-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="79ece-163">响应</span><span class="sxs-lookup"><span data-stu-id="79ece-163">Response</span></span>
<span data-ttu-id="79ece-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79ece-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





