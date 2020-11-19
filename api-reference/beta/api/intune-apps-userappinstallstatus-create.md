---
title: 创建 userAppInstallStatus
description: 创建新的 userAppInstallStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c66c29d2529bb6b50a7a8b255c7c79fab77e8af4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247690"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="6eecc-103">创建 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6eecc-103">Create userAppInstallStatus</span></span>

<span data-ttu-id="6eecc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eecc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6eecc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6eecc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6eecc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6eecc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eecc-107">创建新的 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6eecc-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6eecc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6eecc-108">Prerequisites</span></span>
<span data-ttu-id="6eecc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6eecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eecc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eecc-111">Permission type</span></span>|<span data-ttu-id="6eecc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6eecc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eecc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eecc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6eecc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eecc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6eecc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eecc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eecc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eecc-116">Not supported.</span></span>|
|<span data-ttu-id="6eecc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6eecc-117">Application</span></span>|<span data-ttu-id="6eecc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eecc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eecc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eecc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6eecc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eecc-120">Request headers</span></span>
|<span data-ttu-id="6eecc-121">标头</span><span class="sxs-lookup"><span data-stu-id="6eecc-121">Header</span></span>|<span data-ttu-id="6eecc-122">值</span><span class="sxs-lookup"><span data-stu-id="6eecc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eecc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eecc-123">Authorization</span></span>|<span data-ttu-id="6eecc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6eecc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eecc-125">接受</span><span class="sxs-lookup"><span data-stu-id="6eecc-125">Accept</span></span>|<span data-ttu-id="6eecc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6eecc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eecc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6eecc-127">Request body</span></span>
<span data-ttu-id="6eecc-128">在请求正文中，提供 userAppInstallStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6eecc-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="6eecc-129">下表显示创建 userAppInstallStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6eecc-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="6eecc-130">属性</span><span class="sxs-lookup"><span data-stu-id="6eecc-130">Property</span></span>|<span data-ttu-id="6eecc-131">类型</span><span class="sxs-lookup"><span data-stu-id="6eecc-131">Type</span></span>|<span data-ttu-id="6eecc-132">说明</span><span class="sxs-lookup"><span data-stu-id="6eecc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eecc-133">id</span><span class="sxs-lookup"><span data-stu-id="6eecc-133">id</span></span>|<span data-ttu-id="6eecc-134">String</span><span class="sxs-lookup"><span data-stu-id="6eecc-134">String</span></span>|<span data-ttu-id="6eecc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6eecc-135">Key of the entity.</span></span>|
|<span data-ttu-id="6eecc-136">userName</span><span class="sxs-lookup"><span data-stu-id="6eecc-136">userName</span></span>|<span data-ttu-id="6eecc-137">String</span><span class="sxs-lookup"><span data-stu-id="6eecc-137">String</span></span>|<span data-ttu-id="6eecc-138">用户名。</span><span class="sxs-lookup"><span data-stu-id="6eecc-138">User name.</span></span>|
|<span data-ttu-id="6eecc-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6eecc-139">userPrincipalName</span></span>|<span data-ttu-id="6eecc-140">String</span><span class="sxs-lookup"><span data-stu-id="6eecc-140">String</span></span>|<span data-ttu-id="6eecc-141">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="6eecc-141">User Principal Name.</span></span>|
|<span data-ttu-id="6eecc-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6eecc-142">installedDeviceCount</span></span>|<span data-ttu-id="6eecc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6eecc-143">Int32</span></span>|<span data-ttu-id="6eecc-144">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="6eecc-144">Installed Device Count.</span></span>|
|<span data-ttu-id="6eecc-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6eecc-145">failedDeviceCount</span></span>|<span data-ttu-id="6eecc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6eecc-146">Int32</span></span>|<span data-ttu-id="6eecc-147">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="6eecc-147">Failed Device Count.</span></span>|
|<span data-ttu-id="6eecc-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6eecc-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="6eecc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6eecc-149">Int32</span></span>|<span data-ttu-id="6eecc-150">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="6eecc-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="6eecc-151">响应</span><span class="sxs-lookup"><span data-stu-id="6eecc-151">Response</span></span>
<span data-ttu-id="6eecc-152">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6eecc-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eecc-153">示例</span><span class="sxs-lookup"><span data-stu-id="6eecc-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="6eecc-154">请求</span><span class="sxs-lookup"><span data-stu-id="6eecc-154">Request</span></span>
<span data-ttu-id="6eecc-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6eecc-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6eecc-156">响应</span><span class="sxs-lookup"><span data-stu-id="6eecc-156">Response</span></span>
<span data-ttu-id="6eecc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6eecc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




