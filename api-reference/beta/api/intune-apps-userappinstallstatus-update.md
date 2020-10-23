---
title: 更新 userAppInstallStatus
description: 更新 userAppInstallStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4a2f4a0c5d9ac75e8abf575913a21a18af571fd9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694870"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="1bd41-103">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="1bd41-103">Update userAppInstallStatus</span></span>

<span data-ttu-id="1bd41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bd41-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1bd41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bd41-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1bd41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd41-107">更新 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1bd41-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bd41-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bd41-108">Prerequisites</span></span>
<span data-ttu-id="1bd41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bd41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd41-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bd41-111">Permission type</span></span>|<span data-ttu-id="1bd41-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bd41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bd41-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bd41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bd41-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd41-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bd41-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bd41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bd41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bd41-116">Not supported.</span></span>|
|<span data-ttu-id="1bd41-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bd41-117">Application</span></span>|<span data-ttu-id="1bd41-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd41-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bd41-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bd41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1bd41-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bd41-120">Request headers</span></span>
|<span data-ttu-id="1bd41-121">标头</span><span class="sxs-lookup"><span data-stu-id="1bd41-121">Header</span></span>|<span data-ttu-id="1bd41-122">值</span><span class="sxs-lookup"><span data-stu-id="1bd41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bd41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bd41-123">Authorization</span></span>|<span data-ttu-id="1bd41-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bd41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bd41-125">接受</span><span class="sxs-lookup"><span data-stu-id="1bd41-125">Accept</span></span>|<span data-ttu-id="1bd41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bd41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bd41-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bd41-127">Request body</span></span>
<span data-ttu-id="1bd41-128">在请求正文中，提供 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bd41-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="1bd41-129">下表显示创建 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1bd41-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="1bd41-130">属性</span><span class="sxs-lookup"><span data-stu-id="1bd41-130">Property</span></span>|<span data-ttu-id="1bd41-131">类型</span><span class="sxs-lookup"><span data-stu-id="1bd41-131">Type</span></span>|<span data-ttu-id="1bd41-132">说明</span><span class="sxs-lookup"><span data-stu-id="1bd41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd41-133">id</span><span class="sxs-lookup"><span data-stu-id="1bd41-133">id</span></span>|<span data-ttu-id="1bd41-134">String</span><span class="sxs-lookup"><span data-stu-id="1bd41-134">String</span></span>|<span data-ttu-id="1bd41-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1bd41-135">Key of the entity.</span></span>|
|<span data-ttu-id="1bd41-136">userName</span><span class="sxs-lookup"><span data-stu-id="1bd41-136">userName</span></span>|<span data-ttu-id="1bd41-137">String</span><span class="sxs-lookup"><span data-stu-id="1bd41-137">String</span></span>|<span data-ttu-id="1bd41-138">用户名。</span><span class="sxs-lookup"><span data-stu-id="1bd41-138">User name.</span></span>|
|<span data-ttu-id="1bd41-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1bd41-139">userPrincipalName</span></span>|<span data-ttu-id="1bd41-140">String</span><span class="sxs-lookup"><span data-stu-id="1bd41-140">String</span></span>|<span data-ttu-id="1bd41-141">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="1bd41-141">User Principal Name.</span></span>|
|<span data-ttu-id="1bd41-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bd41-142">installedDeviceCount</span></span>|<span data-ttu-id="1bd41-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1bd41-143">Int32</span></span>|<span data-ttu-id="1bd41-144">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="1bd41-144">Installed Device Count.</span></span>|
|<span data-ttu-id="1bd41-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bd41-145">failedDeviceCount</span></span>|<span data-ttu-id="1bd41-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1bd41-146">Int32</span></span>|<span data-ttu-id="1bd41-147">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="1bd41-147">Failed Device Count.</span></span>|
|<span data-ttu-id="1bd41-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bd41-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="1bd41-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1bd41-149">Int32</span></span>|<span data-ttu-id="1bd41-150">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="1bd41-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="1bd41-151">响应</span><span class="sxs-lookup"><span data-stu-id="1bd41-151">Response</span></span>
<span data-ttu-id="1bd41-152">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1bd41-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bd41-153">示例</span><span class="sxs-lookup"><span data-stu-id="1bd41-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bd41-154">请求</span><span class="sxs-lookup"><span data-stu-id="1bd41-154">Request</span></span>
<span data-ttu-id="1bd41-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bd41-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1bd41-156">响应</span><span class="sxs-lookup"><span data-stu-id="1bd41-156">Response</span></span>
<span data-ttu-id="1bd41-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bd41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





