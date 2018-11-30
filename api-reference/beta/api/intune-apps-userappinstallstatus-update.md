---
title: 更新 userAppInstallStatus
description: 更新 userAppInstallStatus 对象的属性。
ms.openlocfilehash: 352ba84a5829132c78d9a3c4636531978da95d41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042384"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="ab004-103">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ab004-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="ab004-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ab004-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab004-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab004-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab004-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ab004-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab004-107">更新[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ab004-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab004-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab004-108">Prerequisites</span></span>
<span data-ttu-id="ab004-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ab004-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab004-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab004-111">Permission type</span></span>|<span data-ttu-id="ab004-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab004-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab004-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab004-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab004-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab004-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab004-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab004-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab004-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab004-116">Not supported.</span></span>|
|<span data-ttu-id="ab004-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab004-117">Application</span></span>|<span data-ttu-id="ab004-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab004-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab004-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab004-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ab004-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab004-120">Request headers</span></span>
|<span data-ttu-id="ab004-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab004-121">Header</span></span>|<span data-ttu-id="ab004-122">值</span><span class="sxs-lookup"><span data-stu-id="ab004-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab004-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab004-123">Authorization</span></span>|<span data-ttu-id="ab004-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab004-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab004-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab004-125">Accept</span></span>|<span data-ttu-id="ab004-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab004-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab004-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab004-127">Request body</span></span>
<span data-ttu-id="ab004-128">在请求正文中，提供[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab004-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="ab004-129">下表显示时创建[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab004-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="ab004-130">属性</span><span class="sxs-lookup"><span data-stu-id="ab004-130">Property</span></span>|<span data-ttu-id="ab004-131">类型</span><span class="sxs-lookup"><span data-stu-id="ab004-131">Type</span></span>|<span data-ttu-id="ab004-132">说明</span><span class="sxs-lookup"><span data-stu-id="ab004-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab004-133">id</span><span class="sxs-lookup"><span data-stu-id="ab004-133">id</span></span>|<span data-ttu-id="ab004-134">String</span><span class="sxs-lookup"><span data-stu-id="ab004-134">String</span></span>|<span data-ttu-id="ab004-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ab004-135">Key of the entity.</span></span>|
|<span data-ttu-id="ab004-136">userName</span><span class="sxs-lookup"><span data-stu-id="ab004-136">userName</span></span>|<span data-ttu-id="ab004-137">String</span><span class="sxs-lookup"><span data-stu-id="ab004-137">String</span></span>|<span data-ttu-id="ab004-138">用户名。</span><span class="sxs-lookup"><span data-stu-id="ab004-138">User name.</span></span>|
|<span data-ttu-id="ab004-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ab004-139">userPrincipalName</span></span>|<span data-ttu-id="ab004-140">字符串</span><span class="sxs-lookup"><span data-stu-id="ab004-140">String</span></span>|<span data-ttu-id="ab004-141">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="ab004-141">User Principal Name.</span></span>|
|<span data-ttu-id="ab004-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab004-142">installedDeviceCount</span></span>|<span data-ttu-id="ab004-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ab004-143">Int32</span></span>|<span data-ttu-id="ab004-144">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="ab004-144">Installed Device Count.</span></span>|
|<span data-ttu-id="ab004-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab004-145">failedDeviceCount</span></span>|<span data-ttu-id="ab004-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ab004-146">Int32</span></span>|<span data-ttu-id="ab004-147">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="ab004-147">Failed Device Count.</span></span>|
|<span data-ttu-id="ab004-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab004-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="ab004-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ab004-149">Int32</span></span>|<span data-ttu-id="ab004-150">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="ab004-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="ab004-151">响应</span><span class="sxs-lookup"><span data-stu-id="ab004-151">Response</span></span>
<span data-ttu-id="ab004-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab004-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab004-153">示例</span><span class="sxs-lookup"><span data-stu-id="ab004-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab004-154">请求</span><span class="sxs-lookup"><span data-stu-id="ab004-154">Request</span></span>
<span data-ttu-id="ab004-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab004-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
Content-type: application/json
Content-length: 180

{
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="ab004-156">响应</span><span class="sxs-lookup"><span data-stu-id="ab004-156">Response</span></span>
<span data-ttu-id="ab004-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab004-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





