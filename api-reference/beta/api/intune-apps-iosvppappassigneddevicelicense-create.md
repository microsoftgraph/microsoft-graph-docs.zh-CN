---
title: 创建 iosVppAppAssignedDeviceLicense
description: 创建新的 iosVppAppAssignedDeviceLicense 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6ea8cf269a3b5735a366000fb49fd8479eebef2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140636"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="43843-103">创建 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="43843-103">Create iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="43843-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43843-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43843-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43843-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43843-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43843-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43843-107">创建新的 [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43843-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43843-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="43843-108">Prerequisites</span></span>
<span data-ttu-id="43843-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43843-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43843-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="43843-111">Permission type</span></span>|<span data-ttu-id="43843-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43843-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43843-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43843-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43843-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43843-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43843-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43843-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43843-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="43843-116">Not supported.</span></span>|
|<span data-ttu-id="43843-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="43843-117">Application</span></span>|<span data-ttu-id="43843-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43843-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43843-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43843-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="43843-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="43843-120">Request headers</span></span>
|<span data-ttu-id="43843-121">标头</span><span class="sxs-lookup"><span data-stu-id="43843-121">Header</span></span>|<span data-ttu-id="43843-122">值</span><span class="sxs-lookup"><span data-stu-id="43843-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43843-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43843-123">Authorization</span></span>|<span data-ttu-id="43843-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43843-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43843-125">接受</span><span class="sxs-lookup"><span data-stu-id="43843-125">Accept</span></span>|<span data-ttu-id="43843-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43843-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43843-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43843-127">Request body</span></span>
<span data-ttu-id="43843-128">在请求正文中，提供 iosVppAppAssignedDeviceLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43843-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="43843-129">下表显示创建 iosVppAppAssignedDeviceLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="43843-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="43843-130">属性</span><span class="sxs-lookup"><span data-stu-id="43843-130">Property</span></span>|<span data-ttu-id="43843-131">类型</span><span class="sxs-lookup"><span data-stu-id="43843-131">Type</span></span>|<span data-ttu-id="43843-132">说明</span><span class="sxs-lookup"><span data-stu-id="43843-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43843-133">id</span><span class="sxs-lookup"><span data-stu-id="43843-133">id</span></span>|<span data-ttu-id="43843-134">String</span><span class="sxs-lookup"><span data-stu-id="43843-134">String</span></span>|<span data-ttu-id="43843-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="43843-135">Key of the entity.</span></span> <span data-ttu-id="43843-136">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="43843-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="43843-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="43843-137">userEmailAddress</span></span>|<span data-ttu-id="43843-138">String</span><span class="sxs-lookup"><span data-stu-id="43843-138">String</span></span>|<span data-ttu-id="43843-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="43843-139">The user email address.</span></span> <span data-ttu-id="43843-140">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="43843-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="43843-141">userId</span><span class="sxs-lookup"><span data-stu-id="43843-141">userId</span></span>|<span data-ttu-id="43843-142">String</span><span class="sxs-lookup"><span data-stu-id="43843-142">String</span></span>|<span data-ttu-id="43843-143">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="43843-143">The user ID.</span></span> <span data-ttu-id="43843-144">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="43843-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="43843-145">userName</span><span class="sxs-lookup"><span data-stu-id="43843-145">userName</span></span>|<span data-ttu-id="43843-146">String</span><span class="sxs-lookup"><span data-stu-id="43843-146">String</span></span>|<span data-ttu-id="43843-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="43843-147">The user name.</span></span> <span data-ttu-id="43843-148">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="43843-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="43843-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43843-149">userPrincipalName</span></span>|<span data-ttu-id="43843-150">String</span><span class="sxs-lookup"><span data-stu-id="43843-150">String</span></span>|<span data-ttu-id="43843-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="43843-151">The user principal name.</span></span> <span data-ttu-id="43843-152">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="43843-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="43843-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="43843-153">managedDeviceId</span></span>|<span data-ttu-id="43843-154">String</span><span class="sxs-lookup"><span data-stu-id="43843-154">String</span></span>|<span data-ttu-id="43843-155">托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="43843-155">The managed device ID.</span></span>|
|<span data-ttu-id="43843-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="43843-156">deviceName</span></span>|<span data-ttu-id="43843-157">String</span><span class="sxs-lookup"><span data-stu-id="43843-157">String</span></span>|<span data-ttu-id="43843-158">设备名称。</span><span class="sxs-lookup"><span data-stu-id="43843-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="43843-159">响应</span><span class="sxs-lookup"><span data-stu-id="43843-159">Response</span></span>
<span data-ttu-id="43843-160">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43843-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43843-161">示例</span><span class="sxs-lookup"><span data-stu-id="43843-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="43843-162">请求</span><span class="sxs-lookup"><span data-stu-id="43843-162">Request</span></span>
<span data-ttu-id="43843-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43843-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43843-164">响应</span><span class="sxs-lookup"><span data-stu-id="43843-164">Response</span></span>
<span data-ttu-id="43843-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43843-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




