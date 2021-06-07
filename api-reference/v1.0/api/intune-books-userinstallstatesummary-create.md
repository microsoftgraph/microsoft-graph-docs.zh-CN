---
title: 创建 userInstallStateSummary
description: 创建新的 userInstallStateSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2d4f9508607a7b9dba368f5ba0db6efdd774f0b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750306"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="afdbe-103">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="afdbe-103">Create userInstallStateSummary</span></span>

<span data-ttu-id="afdbe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afdbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afdbe-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afdbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afdbe-106">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afdbe-106">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afdbe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="afdbe-107">Prerequisites</span></span>
<span data-ttu-id="afdbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afdbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afdbe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="afdbe-110">Permission type</span></span>|<span data-ttu-id="afdbe-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afdbe-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afdbe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afdbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afdbe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afdbe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="afdbe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afdbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afdbe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="afdbe-115">Not supported.</span></span>|
|<span data-ttu-id="afdbe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="afdbe-116">Application</span></span>|<span data-ttu-id="afdbe-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afdbe-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afdbe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afdbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="afdbe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="afdbe-119">Request headers</span></span>
|<span data-ttu-id="afdbe-120">标头</span><span class="sxs-lookup"><span data-stu-id="afdbe-120">Header</span></span>|<span data-ttu-id="afdbe-121">值</span><span class="sxs-lookup"><span data-stu-id="afdbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afdbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afdbe-122">Authorization</span></span>|<span data-ttu-id="afdbe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="afdbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afdbe-124">接受</span><span class="sxs-lookup"><span data-stu-id="afdbe-124">Accept</span></span>|<span data-ttu-id="afdbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afdbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afdbe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="afdbe-126">Request body</span></span>
<span data-ttu-id="afdbe-127">在请求正文中，提供 userInstallStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afdbe-127">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="afdbe-128">下表显示创建 userInstallStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="afdbe-128">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="afdbe-129">属性</span><span class="sxs-lookup"><span data-stu-id="afdbe-129">Property</span></span>|<span data-ttu-id="afdbe-130">类型</span><span class="sxs-lookup"><span data-stu-id="afdbe-130">Type</span></span>|<span data-ttu-id="afdbe-131">说明</span><span class="sxs-lookup"><span data-stu-id="afdbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afdbe-132">id</span><span class="sxs-lookup"><span data-stu-id="afdbe-132">id</span></span>|<span data-ttu-id="afdbe-133">String</span><span class="sxs-lookup"><span data-stu-id="afdbe-133">String</span></span>|<span data-ttu-id="afdbe-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="afdbe-134">Key of the entity.</span></span>|
|<span data-ttu-id="afdbe-135">userName</span><span class="sxs-lookup"><span data-stu-id="afdbe-135">userName</span></span>|<span data-ttu-id="afdbe-136">String</span><span class="sxs-lookup"><span data-stu-id="afdbe-136">String</span></span>|<span data-ttu-id="afdbe-137">用户名。</span><span class="sxs-lookup"><span data-stu-id="afdbe-137">User name.</span></span>|
|<span data-ttu-id="afdbe-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="afdbe-138">installedDeviceCount</span></span>|<span data-ttu-id="afdbe-139">Int32</span><span class="sxs-lookup"><span data-stu-id="afdbe-139">Int32</span></span>|<span data-ttu-id="afdbe-140">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="afdbe-140">Installed Device Count.</span></span>|
|<span data-ttu-id="afdbe-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="afdbe-141">failedDeviceCount</span></span>|<span data-ttu-id="afdbe-142">Int32</span><span class="sxs-lookup"><span data-stu-id="afdbe-142">Int32</span></span>|<span data-ttu-id="afdbe-143">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="afdbe-143">Failed Device Count.</span></span>|
|<span data-ttu-id="afdbe-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="afdbe-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="afdbe-145">Int32</span><span class="sxs-lookup"><span data-stu-id="afdbe-145">Int32</span></span>|<span data-ttu-id="afdbe-146">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="afdbe-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="afdbe-147">响应</span><span class="sxs-lookup"><span data-stu-id="afdbe-147">Response</span></span>
<span data-ttu-id="afdbe-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afdbe-148">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afdbe-149">示例</span><span class="sxs-lookup"><span data-stu-id="afdbe-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="afdbe-150">请求</span><span class="sxs-lookup"><span data-stu-id="afdbe-150">Request</span></span>
<span data-ttu-id="afdbe-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afdbe-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="afdbe-152">响应</span><span class="sxs-lookup"><span data-stu-id="afdbe-152">Response</span></span>
<span data-ttu-id="afdbe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afdbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




