---
title: 创建 userInstallStateSummary
description: 创建新的 userInstallStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cb123adec686db29bdf1dfefc3c7a459a427833
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525010"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="b000f-103">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b000f-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="b000f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b000f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b000f-105">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b000f-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b000f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b000f-106">Prerequisites</span></span>
<span data-ttu-id="b000f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b000f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b000f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b000f-109">Permission type</span></span>|<span data-ttu-id="b000f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b000f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b000f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b000f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b000f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b000f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b000f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b000f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b000f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b000f-114">Not supported.</span></span>|
|<span data-ttu-id="b000f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b000f-115">Application</span></span>|<span data-ttu-id="b000f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b000f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b000f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b000f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="b000f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b000f-118">Request headers</span></span>
|<span data-ttu-id="b000f-119">标头</span><span class="sxs-lookup"><span data-stu-id="b000f-119">Header</span></span>|<span data-ttu-id="b000f-120">值</span><span class="sxs-lookup"><span data-stu-id="b000f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b000f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b000f-121">Authorization</span></span>|<span data-ttu-id="b000f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b000f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b000f-123">接受</span><span class="sxs-lookup"><span data-stu-id="b000f-123">Accept</span></span>|<span data-ttu-id="b000f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b000f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b000f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b000f-125">Request body</span></span>
<span data-ttu-id="b000f-126">在请求正文中，提供 userInstallStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b000f-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="b000f-127">下表显示创建 userInstallStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b000f-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="b000f-128">属性</span><span class="sxs-lookup"><span data-stu-id="b000f-128">Property</span></span>|<span data-ttu-id="b000f-129">类型</span><span class="sxs-lookup"><span data-stu-id="b000f-129">Type</span></span>|<span data-ttu-id="b000f-130">说明</span><span class="sxs-lookup"><span data-stu-id="b000f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b000f-131">id</span><span class="sxs-lookup"><span data-stu-id="b000f-131">id</span></span>|<span data-ttu-id="b000f-132">String</span><span class="sxs-lookup"><span data-stu-id="b000f-132">String</span></span>|<span data-ttu-id="b000f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b000f-133">Key of the entity.</span></span>|
|<span data-ttu-id="b000f-134">userName</span><span class="sxs-lookup"><span data-stu-id="b000f-134">userName</span></span>|<span data-ttu-id="b000f-135">String</span><span class="sxs-lookup"><span data-stu-id="b000f-135">String</span></span>|<span data-ttu-id="b000f-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="b000f-136">User name.</span></span>|
|<span data-ttu-id="b000f-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b000f-137">installedDeviceCount</span></span>|<span data-ttu-id="b000f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b000f-138">Int32</span></span>|<span data-ttu-id="b000f-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b000f-139">Installed Device Count.</span></span>|
|<span data-ttu-id="b000f-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b000f-140">failedDeviceCount</span></span>|<span data-ttu-id="b000f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b000f-141">Int32</span></span>|<span data-ttu-id="b000f-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b000f-142">Failed Device Count.</span></span>|
|<span data-ttu-id="b000f-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b000f-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="b000f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b000f-144">Int32</span></span>|<span data-ttu-id="b000f-145">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b000f-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="b000f-146">响应</span><span class="sxs-lookup"><span data-stu-id="b000f-146">Response</span></span>
<span data-ttu-id="b000f-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b000f-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b000f-148">示例</span><span class="sxs-lookup"><span data-stu-id="b000f-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b000f-149">请求</span><span class="sxs-lookup"><span data-stu-id="b000f-149">Request</span></span>
<span data-ttu-id="b000f-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b000f-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b000f-151">响应</span><span class="sxs-lookup"><span data-stu-id="b000f-151">Response</span></span>
<span data-ttu-id="b000f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b000f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



