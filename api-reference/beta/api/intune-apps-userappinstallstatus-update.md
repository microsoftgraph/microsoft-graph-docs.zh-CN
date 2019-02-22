---
title: 更新 userAppInstallStatus
description: 更新 userAppInstallStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3baa0d23be3b004fe32049cee0efe08e8f7d36d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144903"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="2968f-103">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2968f-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="2968f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2968f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2968f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2968f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2968f-106">更新[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2968f-106">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2968f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2968f-107">Prerequisites</span></span>
<span data-ttu-id="2968f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2968f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2968f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2968f-110">Permission type</span></span>|<span data-ttu-id="2968f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2968f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2968f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2968f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2968f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2968f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2968f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2968f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2968f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2968f-115">Not supported.</span></span>|
|<span data-ttu-id="2968f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2968f-116">Application</span></span>|<span data-ttu-id="2968f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2968f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2968f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2968f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2968f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2968f-119">Request headers</span></span>
|<span data-ttu-id="2968f-120">标头</span><span class="sxs-lookup"><span data-stu-id="2968f-120">Header</span></span>|<span data-ttu-id="2968f-121">值</span><span class="sxs-lookup"><span data-stu-id="2968f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2968f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2968f-122">Authorization</span></span>|<span data-ttu-id="2968f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2968f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2968f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2968f-124">Accept</span></span>|<span data-ttu-id="2968f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2968f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2968f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2968f-126">Request body</span></span>
<span data-ttu-id="2968f-127">在请求正文中, 提供[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2968f-127">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="2968f-128">下表显示创建[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2968f-128">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="2968f-129">属性</span><span class="sxs-lookup"><span data-stu-id="2968f-129">Property</span></span>|<span data-ttu-id="2968f-130">类型</span><span class="sxs-lookup"><span data-stu-id="2968f-130">Type</span></span>|<span data-ttu-id="2968f-131">说明</span><span class="sxs-lookup"><span data-stu-id="2968f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2968f-132">id</span><span class="sxs-lookup"><span data-stu-id="2968f-132">id</span></span>|<span data-ttu-id="2968f-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="2968f-133">String</span></span>|<span data-ttu-id="2968f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2968f-134">Key of the entity.</span></span>|
|<span data-ttu-id="2968f-135">userName</span><span class="sxs-lookup"><span data-stu-id="2968f-135">userName</span></span>|<span data-ttu-id="2968f-136">String</span><span class="sxs-lookup"><span data-stu-id="2968f-136">String</span></span>|<span data-ttu-id="2968f-137">用户名。</span><span class="sxs-lookup"><span data-stu-id="2968f-137">User name.</span></span>|
|<span data-ttu-id="2968f-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2968f-138">userPrincipalName</span></span>|<span data-ttu-id="2968f-139">字符串</span><span class="sxs-lookup"><span data-stu-id="2968f-139">String</span></span>|<span data-ttu-id="2968f-140">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="2968f-140">User Principal Name.</span></span>|
|<span data-ttu-id="2968f-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2968f-141">installedDeviceCount</span></span>|<span data-ttu-id="2968f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2968f-142">Int32</span></span>|<span data-ttu-id="2968f-143">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="2968f-143">Installed Device Count.</span></span>|
|<span data-ttu-id="2968f-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2968f-144">failedDeviceCount</span></span>|<span data-ttu-id="2968f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2968f-145">Int32</span></span>|<span data-ttu-id="2968f-146">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="2968f-146">Failed Device Count.</span></span>|
|<span data-ttu-id="2968f-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2968f-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="2968f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2968f-148">Int32</span></span>|<span data-ttu-id="2968f-149">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="2968f-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="2968f-150">响应</span><span class="sxs-lookup"><span data-stu-id="2968f-150">Response</span></span>
<span data-ttu-id="2968f-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2968f-151">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2968f-152">示例</span><span class="sxs-lookup"><span data-stu-id="2968f-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2968f-153">请求</span><span class="sxs-lookup"><span data-stu-id="2968f-153">Request</span></span>
<span data-ttu-id="2968f-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2968f-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2968f-155">响应</span><span class="sxs-lookup"><span data-stu-id="2968f-155">Response</span></span>
<span data-ttu-id="2968f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2968f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




