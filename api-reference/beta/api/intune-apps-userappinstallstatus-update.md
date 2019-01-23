---
title: 更新 userAppInstallStatus
description: 更新 userAppInstallStatus 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 237e9f28f36fb25ea5ddad46f5a6a75242767c6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413834"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="bf5be-103">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="bf5be-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="bf5be-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bf5be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf5be-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf5be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf5be-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf5be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf5be-107">更新[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf5be-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf5be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf5be-108">Prerequisites</span></span>
<span data-ttu-id="bf5be-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bf5be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bf5be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf5be-111">Permission type</span></span>|<span data-ttu-id="bf5be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf5be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf5be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf5be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf5be-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf5be-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bf5be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf5be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf5be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf5be-116">Not supported.</span></span>|
|<span data-ttu-id="bf5be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf5be-117">Application</span></span>|<span data-ttu-id="bf5be-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf5be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf5be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf5be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="bf5be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf5be-120">Request headers</span></span>
|<span data-ttu-id="bf5be-121">标头</span><span class="sxs-lookup"><span data-stu-id="bf5be-121">Header</span></span>|<span data-ttu-id="bf5be-122">值</span><span class="sxs-lookup"><span data-stu-id="bf5be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf5be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf5be-123">Authorization</span></span>|<span data-ttu-id="bf5be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf5be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf5be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf5be-125">Accept</span></span>|<span data-ttu-id="bf5be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf5be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf5be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf5be-127">Request body</span></span>
<span data-ttu-id="bf5be-128">在请求正文中，提供[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf5be-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="bf5be-129">下表显示时创建[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bf5be-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="bf5be-130">属性</span><span class="sxs-lookup"><span data-stu-id="bf5be-130">Property</span></span>|<span data-ttu-id="bf5be-131">类型</span><span class="sxs-lookup"><span data-stu-id="bf5be-131">Type</span></span>|<span data-ttu-id="bf5be-132">说明</span><span class="sxs-lookup"><span data-stu-id="bf5be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf5be-133">id</span><span class="sxs-lookup"><span data-stu-id="bf5be-133">id</span></span>|<span data-ttu-id="bf5be-134">String</span><span class="sxs-lookup"><span data-stu-id="bf5be-134">String</span></span>|<span data-ttu-id="bf5be-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bf5be-135">Key of the entity.</span></span>|
|<span data-ttu-id="bf5be-136">userName</span><span class="sxs-lookup"><span data-stu-id="bf5be-136">userName</span></span>|<span data-ttu-id="bf5be-137">String</span><span class="sxs-lookup"><span data-stu-id="bf5be-137">String</span></span>|<span data-ttu-id="bf5be-138">用户名。</span><span class="sxs-lookup"><span data-stu-id="bf5be-138">User name.</span></span>|
|<span data-ttu-id="bf5be-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bf5be-139">userPrincipalName</span></span>|<span data-ttu-id="bf5be-140">String</span><span class="sxs-lookup"><span data-stu-id="bf5be-140">String</span></span>|<span data-ttu-id="bf5be-141">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="bf5be-141">User Principal Name.</span></span>|
|<span data-ttu-id="bf5be-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf5be-142">installedDeviceCount</span></span>|<span data-ttu-id="bf5be-143">Int32</span><span class="sxs-lookup"><span data-stu-id="bf5be-143">Int32</span></span>|<span data-ttu-id="bf5be-144">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="bf5be-144">Installed Device Count.</span></span>|
|<span data-ttu-id="bf5be-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf5be-145">failedDeviceCount</span></span>|<span data-ttu-id="bf5be-146">Int32</span><span class="sxs-lookup"><span data-stu-id="bf5be-146">Int32</span></span>|<span data-ttu-id="bf5be-147">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="bf5be-147">Failed Device Count.</span></span>|
|<span data-ttu-id="bf5be-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf5be-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="bf5be-149">Int32</span><span class="sxs-lookup"><span data-stu-id="bf5be-149">Int32</span></span>|<span data-ttu-id="bf5be-150">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="bf5be-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="bf5be-151">响应</span><span class="sxs-lookup"><span data-stu-id="bf5be-151">Response</span></span>
<span data-ttu-id="bf5be-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bf5be-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf5be-153">示例</span><span class="sxs-lookup"><span data-stu-id="bf5be-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf5be-154">请求</span><span class="sxs-lookup"><span data-stu-id="bf5be-154">Request</span></span>
<span data-ttu-id="bf5be-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf5be-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
Content-type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="bf5be-156">响应</span><span class="sxs-lookup"><span data-stu-id="bf5be-156">Response</span></span>
<span data-ttu-id="bf5be-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf5be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




