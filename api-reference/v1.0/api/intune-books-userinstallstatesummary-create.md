---
title: 创建 userInstallStateSummary
description: 创建新的 userInstallStateSummary 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 23060cad3191e2df69614c3f9238bd9fbdf56ca2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354649"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="50e68-103">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="50e68-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="50e68-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50e68-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e68-105">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50e68-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50e68-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="50e68-106">Prerequisites</span></span>
<span data-ttu-id="50e68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50e68-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="50e68-109">Permission type</span></span>|<span data-ttu-id="50e68-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50e68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50e68-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50e68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50e68-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50e68-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50e68-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50e68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50e68-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="50e68-114">Not supported.</span></span>|
|<span data-ttu-id="50e68-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="50e68-115">Application</span></span>|<span data-ttu-id="50e68-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="50e68-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50e68-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50e68-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="50e68-118">请求头</span><span class="sxs-lookup"><span data-stu-id="50e68-118">Request headers</span></span>
|<span data-ttu-id="50e68-119">标头</span><span class="sxs-lookup"><span data-stu-id="50e68-119">Header</span></span>|<span data-ttu-id="50e68-120">值</span><span class="sxs-lookup"><span data-stu-id="50e68-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50e68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50e68-121">Authorization</span></span>|<span data-ttu-id="50e68-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50e68-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50e68-123">接受</span><span class="sxs-lookup"><span data-stu-id="50e68-123">Accept</span></span>|<span data-ttu-id="50e68-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50e68-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50e68-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="50e68-125">Request body</span></span>
<span data-ttu-id="50e68-126">在请求正文中，提供 userInstallStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50e68-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="50e68-127">下表显示创建 userInstallStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50e68-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="50e68-128">属性</span><span class="sxs-lookup"><span data-stu-id="50e68-128">Property</span></span>|<span data-ttu-id="50e68-129">类型</span><span class="sxs-lookup"><span data-stu-id="50e68-129">Type</span></span>|<span data-ttu-id="50e68-130">说明</span><span class="sxs-lookup"><span data-stu-id="50e68-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50e68-131">id</span><span class="sxs-lookup"><span data-stu-id="50e68-131">id</span></span>|<span data-ttu-id="50e68-132">String</span><span class="sxs-lookup"><span data-stu-id="50e68-132">String</span></span>|<span data-ttu-id="50e68-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="50e68-133">Key of the entity.</span></span>|
|<span data-ttu-id="50e68-134">userName</span><span class="sxs-lookup"><span data-stu-id="50e68-134">userName</span></span>|<span data-ttu-id="50e68-135">String</span><span class="sxs-lookup"><span data-stu-id="50e68-135">String</span></span>|<span data-ttu-id="50e68-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="50e68-136">User name.</span></span>|
|<span data-ttu-id="50e68-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50e68-137">installedDeviceCount</span></span>|<span data-ttu-id="50e68-138">Int32</span><span class="sxs-lookup"><span data-stu-id="50e68-138">Int32</span></span>|<span data-ttu-id="50e68-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="50e68-139">Installed Device Count.</span></span>|
|<span data-ttu-id="50e68-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50e68-140">failedDeviceCount</span></span>|<span data-ttu-id="50e68-141">Int32</span><span class="sxs-lookup"><span data-stu-id="50e68-141">Int32</span></span>|<span data-ttu-id="50e68-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="50e68-142">Failed Device Count.</span></span>|
|<span data-ttu-id="50e68-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50e68-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="50e68-144">Int32</span><span class="sxs-lookup"><span data-stu-id="50e68-144">Int32</span></span>|<span data-ttu-id="50e68-145">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="50e68-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="50e68-146">响应</span><span class="sxs-lookup"><span data-stu-id="50e68-146">Response</span></span>
<span data-ttu-id="50e68-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50e68-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50e68-148">示例</span><span class="sxs-lookup"><span data-stu-id="50e68-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="50e68-149">请求</span><span class="sxs-lookup"><span data-stu-id="50e68-149">Request</span></span>
<span data-ttu-id="50e68-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50e68-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50e68-151">响应</span><span class="sxs-lookup"><span data-stu-id="50e68-151">Response</span></span>
<span data-ttu-id="50e68-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50e68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




