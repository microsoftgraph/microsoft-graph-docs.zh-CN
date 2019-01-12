---
title: 创建 iosVppAppAssignedDeviceLicense
description: 创建新的 iosVppAppAssignedDeviceLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c4eecadae91eb857a5b90c88d66af1721f268ddb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914379"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="60523-103">创建 iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="60523-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="60523-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="60523-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60523-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60523-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60523-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="60523-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60523-107">创建新的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="60523-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60523-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="60523-108">Prerequisites</span></span>
<span data-ttu-id="60523-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="60523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60523-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="60523-111">Permission type</span></span>|<span data-ttu-id="60523-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60523-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60523-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60523-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60523-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60523-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60523-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60523-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60523-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60523-116">Not supported.</span></span>|
|<span data-ttu-id="60523-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60523-117">Application</span></span>|<span data-ttu-id="60523-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="60523-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60523-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60523-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="60523-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60523-120">Request headers</span></span>
|<span data-ttu-id="60523-121">标头</span><span class="sxs-lookup"><span data-stu-id="60523-121">Header</span></span>|<span data-ttu-id="60523-122">值</span><span class="sxs-lookup"><span data-stu-id="60523-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60523-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60523-123">Authorization</span></span>|<span data-ttu-id="60523-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60523-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60523-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60523-125">Accept</span></span>|<span data-ttu-id="60523-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60523-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60523-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60523-127">Request body</span></span>
<span data-ttu-id="60523-128">在请求正文中，提供 iosVppAppAssignedDeviceLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60523-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="60523-129">下表显示时创建 iosVppAppAssignedDeviceLicense 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60523-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="60523-130">属性</span><span class="sxs-lookup"><span data-stu-id="60523-130">Property</span></span>|<span data-ttu-id="60523-131">类型</span><span class="sxs-lookup"><span data-stu-id="60523-131">Type</span></span>|<span data-ttu-id="60523-132">说明</span><span class="sxs-lookup"><span data-stu-id="60523-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60523-133">id</span><span class="sxs-lookup"><span data-stu-id="60523-133">id</span></span>|<span data-ttu-id="60523-134">String</span><span class="sxs-lookup"><span data-stu-id="60523-134">String</span></span>|<span data-ttu-id="60523-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60523-135">Key of the entity.</span></span> <span data-ttu-id="60523-136">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60523-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60523-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="60523-137">userEmailAddress</span></span>|<span data-ttu-id="60523-138">字符串</span><span class="sxs-lookup"><span data-stu-id="60523-138">String</span></span>|<span data-ttu-id="60523-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="60523-139">The user email address.</span></span> <span data-ttu-id="60523-140">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60523-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60523-141">userId</span><span class="sxs-lookup"><span data-stu-id="60523-141">userId</span></span>|<span data-ttu-id="60523-142">String</span><span class="sxs-lookup"><span data-stu-id="60523-142">String</span></span>|<span data-ttu-id="60523-143">用户 id。</span><span class="sxs-lookup"><span data-stu-id="60523-143">The user ID.</span></span> <span data-ttu-id="60523-144">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60523-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60523-145">userName</span><span class="sxs-lookup"><span data-stu-id="60523-145">userName</span></span>|<span data-ttu-id="60523-146">String</span><span class="sxs-lookup"><span data-stu-id="60523-146">String</span></span>|<span data-ttu-id="60523-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="60523-147">The user name.</span></span> <span data-ttu-id="60523-148">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60523-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60523-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="60523-149">userPrincipalName</span></span>|<span data-ttu-id="60523-150">字符串</span><span class="sxs-lookup"><span data-stu-id="60523-150">String</span></span>|<span data-ttu-id="60523-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="60523-151">The user principal name.</span></span> <span data-ttu-id="60523-152">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60523-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60523-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="60523-153">managedDeviceId</span></span>|<span data-ttu-id="60523-154">字符串</span><span class="sxs-lookup"><span data-stu-id="60523-154">String</span></span>|<span data-ttu-id="60523-155">托管的设备 id。</span><span class="sxs-lookup"><span data-stu-id="60523-155">The managed device ID.</span></span>|
|<span data-ttu-id="60523-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="60523-156">deviceName</span></span>|<span data-ttu-id="60523-157">String</span><span class="sxs-lookup"><span data-stu-id="60523-157">String</span></span>|<span data-ttu-id="60523-158">设备名称。</span><span class="sxs-lookup"><span data-stu-id="60523-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="60523-159">响应</span><span class="sxs-lookup"><span data-stu-id="60523-159">Response</span></span>
<span data-ttu-id="60523-160">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="60523-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60523-161">示例</span><span class="sxs-lookup"><span data-stu-id="60523-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="60523-162">请求</span><span class="sxs-lookup"><span data-stu-id="60523-162">Request</span></span>
<span data-ttu-id="60523-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60523-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60523-164">响应</span><span class="sxs-lookup"><span data-stu-id="60523-164">Response</span></span>
<span data-ttu-id="60523-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60523-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





