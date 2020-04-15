---
title: 更新 userInstallStateSummary
description: 更新 userInstallStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b03442d0ebd4e0a0379003eba72b44023b7db7ec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468951"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="10f37-103">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="10f37-103">Update userInstallStateSummary</span></span>

<span data-ttu-id="10f37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10f37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10f37-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10f37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10f37-106">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10f37-106">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10f37-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="10f37-107">Prerequisites</span></span>
<span data-ttu-id="10f37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10f37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f37-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="10f37-110">Permission type</span></span>|<span data-ttu-id="10f37-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10f37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10f37-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10f37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10f37-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f37-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10f37-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10f37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10f37-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="10f37-115">Not supported.</span></span>|
|<span data-ttu-id="10f37-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="10f37-116">Application</span></span>|<span data-ttu-id="10f37-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="10f37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10f37-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10f37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="10f37-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="10f37-119">Request headers</span></span>
|<span data-ttu-id="10f37-120">标头</span><span class="sxs-lookup"><span data-stu-id="10f37-120">Header</span></span>|<span data-ttu-id="10f37-121">值</span><span class="sxs-lookup"><span data-stu-id="10f37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10f37-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10f37-122">Authorization</span></span>|<span data-ttu-id="10f37-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10f37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10f37-124">接受</span><span class="sxs-lookup"><span data-stu-id="10f37-124">Accept</span></span>|<span data-ttu-id="10f37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10f37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10f37-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="10f37-126">Request body</span></span>
<span data-ttu-id="10f37-127">在请求正文中，提供 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10f37-127">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="10f37-128">下表显示创建 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="10f37-128">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="10f37-129">属性</span><span class="sxs-lookup"><span data-stu-id="10f37-129">Property</span></span>|<span data-ttu-id="10f37-130">类型</span><span class="sxs-lookup"><span data-stu-id="10f37-130">Type</span></span>|<span data-ttu-id="10f37-131">说明</span><span class="sxs-lookup"><span data-stu-id="10f37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10f37-132">id</span><span class="sxs-lookup"><span data-stu-id="10f37-132">id</span></span>|<span data-ttu-id="10f37-133">String</span><span class="sxs-lookup"><span data-stu-id="10f37-133">String</span></span>|<span data-ttu-id="10f37-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="10f37-134">Key of the entity.</span></span>|
|<span data-ttu-id="10f37-135">userName</span><span class="sxs-lookup"><span data-stu-id="10f37-135">userName</span></span>|<span data-ttu-id="10f37-136">String</span><span class="sxs-lookup"><span data-stu-id="10f37-136">String</span></span>|<span data-ttu-id="10f37-137">用户名。</span><span class="sxs-lookup"><span data-stu-id="10f37-137">User name.</span></span>|
|<span data-ttu-id="10f37-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10f37-138">installedDeviceCount</span></span>|<span data-ttu-id="10f37-139">Int32</span><span class="sxs-lookup"><span data-stu-id="10f37-139">Int32</span></span>|<span data-ttu-id="10f37-140">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="10f37-140">Installed Device Count.</span></span>|
|<span data-ttu-id="10f37-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10f37-141">failedDeviceCount</span></span>|<span data-ttu-id="10f37-142">Int32</span><span class="sxs-lookup"><span data-stu-id="10f37-142">Int32</span></span>|<span data-ttu-id="10f37-143">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="10f37-143">Failed Device Count.</span></span>|
|<span data-ttu-id="10f37-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10f37-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="10f37-145">Int32</span><span class="sxs-lookup"><span data-stu-id="10f37-145">Int32</span></span>|<span data-ttu-id="10f37-146">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="10f37-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="10f37-147">响应</span><span class="sxs-lookup"><span data-stu-id="10f37-147">Response</span></span>
<span data-ttu-id="10f37-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10f37-148">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f37-149">示例</span><span class="sxs-lookup"><span data-stu-id="10f37-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="10f37-150">请求</span><span class="sxs-lookup"><span data-stu-id="10f37-150">Request</span></span>
<span data-ttu-id="10f37-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10f37-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="10f37-152">响应</span><span class="sxs-lookup"><span data-stu-id="10f37-152">Response</span></span>
<span data-ttu-id="10f37-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10f37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```






