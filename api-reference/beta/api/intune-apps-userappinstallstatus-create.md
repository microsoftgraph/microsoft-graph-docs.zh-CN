---
title: 创建 userAppInstallStatus
description: 创建新的 userAppInstallStatus 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeecdc0acfe857cf79d50189dd4452e4c3e78399
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934934"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="90555-103">创建 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="90555-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="90555-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90555-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90555-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90555-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90555-106">创建新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90555-106">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90555-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="90555-107">Prerequisites</span></span>
<span data-ttu-id="90555-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90555-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90555-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="90555-110">Permission type</span></span>|<span data-ttu-id="90555-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90555-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90555-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90555-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90555-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90555-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90555-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90555-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90555-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90555-115">Not supported.</span></span>|
|<span data-ttu-id="90555-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="90555-116">Application</span></span>|<span data-ttu-id="90555-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="90555-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90555-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90555-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="90555-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="90555-119">Request headers</span></span>
|<span data-ttu-id="90555-120">标头</span><span class="sxs-lookup"><span data-stu-id="90555-120">Header</span></span>|<span data-ttu-id="90555-121">值</span><span class="sxs-lookup"><span data-stu-id="90555-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90555-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90555-122">Authorization</span></span>|<span data-ttu-id="90555-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90555-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90555-124">接受</span><span class="sxs-lookup"><span data-stu-id="90555-124">Accept</span></span>|<span data-ttu-id="90555-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90555-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90555-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90555-126">Request body</span></span>
<span data-ttu-id="90555-127">在请求正文中, 提供 userAppInstallStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90555-127">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="90555-128">下表显示创建 userAppInstallStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90555-128">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="90555-129">属性</span><span class="sxs-lookup"><span data-stu-id="90555-129">Property</span></span>|<span data-ttu-id="90555-130">类型</span><span class="sxs-lookup"><span data-stu-id="90555-130">Type</span></span>|<span data-ttu-id="90555-131">说明</span><span class="sxs-lookup"><span data-stu-id="90555-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90555-132">id</span><span class="sxs-lookup"><span data-stu-id="90555-132">id</span></span>|<span data-ttu-id="90555-133">String</span><span class="sxs-lookup"><span data-stu-id="90555-133">String</span></span>|<span data-ttu-id="90555-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="90555-134">Key of the entity.</span></span>|
|<span data-ttu-id="90555-135">userName</span><span class="sxs-lookup"><span data-stu-id="90555-135">userName</span></span>|<span data-ttu-id="90555-136">String</span><span class="sxs-lookup"><span data-stu-id="90555-136">String</span></span>|<span data-ttu-id="90555-137">用户名。</span><span class="sxs-lookup"><span data-stu-id="90555-137">User name.</span></span>|
|<span data-ttu-id="90555-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="90555-138">userPrincipalName</span></span>|<span data-ttu-id="90555-139">String</span><span class="sxs-lookup"><span data-stu-id="90555-139">String</span></span>|<span data-ttu-id="90555-140">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="90555-140">User Principal Name.</span></span>|
|<span data-ttu-id="90555-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90555-141">installedDeviceCount</span></span>|<span data-ttu-id="90555-142">Int32</span><span class="sxs-lookup"><span data-stu-id="90555-142">Int32</span></span>|<span data-ttu-id="90555-143">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="90555-143">Installed Device Count.</span></span>|
|<span data-ttu-id="90555-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90555-144">failedDeviceCount</span></span>|<span data-ttu-id="90555-145">Int32</span><span class="sxs-lookup"><span data-stu-id="90555-145">Int32</span></span>|<span data-ttu-id="90555-146">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="90555-146">Failed Device Count.</span></span>|
|<span data-ttu-id="90555-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90555-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="90555-148">Int32</span><span class="sxs-lookup"><span data-stu-id="90555-148">Int32</span></span>|<span data-ttu-id="90555-149">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="90555-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="90555-150">响应</span><span class="sxs-lookup"><span data-stu-id="90555-150">Response</span></span>
<span data-ttu-id="90555-151">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90555-151">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90555-152">示例</span><span class="sxs-lookup"><span data-stu-id="90555-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="90555-153">请求</span><span class="sxs-lookup"><span data-stu-id="90555-153">Request</span></span>
<span data-ttu-id="90555-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90555-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="90555-155">响应</span><span class="sxs-lookup"><span data-stu-id="90555-155">Response</span></span>
<span data-ttu-id="90555-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90555-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




