---
title: 更新 userInstallStateSummary
description: 更新 userInstallStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fabf57da88e740eea1ac43dd7c24e2d6884e5bbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524524"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="899d2-103">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="899d2-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="899d2-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="899d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="899d2-105">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="899d2-105">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="899d2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="899d2-106">Prerequisites</span></span>
<span data-ttu-id="899d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="899d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="899d2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="899d2-109">Permission type</span></span>|<span data-ttu-id="899d2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="899d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="899d2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="899d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="899d2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="899d2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="899d2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="899d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="899d2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="899d2-114">Not supported.</span></span>|
|<span data-ttu-id="899d2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="899d2-115">Application</span></span>|<span data-ttu-id="899d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="899d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="899d2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="899d2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="899d2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="899d2-118">Request headers</span></span>
|<span data-ttu-id="899d2-119">标头</span><span class="sxs-lookup"><span data-stu-id="899d2-119">Header</span></span>|<span data-ttu-id="899d2-120">值</span><span class="sxs-lookup"><span data-stu-id="899d2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="899d2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="899d2-121">Authorization</span></span>|<span data-ttu-id="899d2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="899d2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="899d2-123">接受</span><span class="sxs-lookup"><span data-stu-id="899d2-123">Accept</span></span>|<span data-ttu-id="899d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="899d2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="899d2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="899d2-125">Request body</span></span>
<span data-ttu-id="899d2-126">在请求正文中，提供 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="899d2-126">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="899d2-127">下表显示创建 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="899d2-127">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="899d2-128">属性</span><span class="sxs-lookup"><span data-stu-id="899d2-128">Property</span></span>|<span data-ttu-id="899d2-129">类型</span><span class="sxs-lookup"><span data-stu-id="899d2-129">Type</span></span>|<span data-ttu-id="899d2-130">说明</span><span class="sxs-lookup"><span data-stu-id="899d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="899d2-131">id</span><span class="sxs-lookup"><span data-stu-id="899d2-131">id</span></span>|<span data-ttu-id="899d2-132">String</span><span class="sxs-lookup"><span data-stu-id="899d2-132">String</span></span>|<span data-ttu-id="899d2-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="899d2-133">Key of the entity.</span></span>|
|<span data-ttu-id="899d2-134">userName</span><span class="sxs-lookup"><span data-stu-id="899d2-134">userName</span></span>|<span data-ttu-id="899d2-135">String</span><span class="sxs-lookup"><span data-stu-id="899d2-135">String</span></span>|<span data-ttu-id="899d2-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="899d2-136">User name.</span></span>|
|<span data-ttu-id="899d2-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="899d2-137">installedDeviceCount</span></span>|<span data-ttu-id="899d2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="899d2-138">Int32</span></span>|<span data-ttu-id="899d2-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="899d2-139">Installed Device Count.</span></span>|
|<span data-ttu-id="899d2-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="899d2-140">failedDeviceCount</span></span>|<span data-ttu-id="899d2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="899d2-141">Int32</span></span>|<span data-ttu-id="899d2-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="899d2-142">Failed Device Count.</span></span>|
|<span data-ttu-id="899d2-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="899d2-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="899d2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="899d2-144">Int32</span></span>|<span data-ttu-id="899d2-145">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="899d2-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="899d2-146">响应</span><span class="sxs-lookup"><span data-stu-id="899d2-146">Response</span></span>
<span data-ttu-id="899d2-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="899d2-147">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="899d2-148">示例</span><span class="sxs-lookup"><span data-stu-id="899d2-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="899d2-149">请求</span><span class="sxs-lookup"><span data-stu-id="899d2-149">Request</span></span>
<span data-ttu-id="899d2-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="899d2-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="899d2-151">响应</span><span class="sxs-lookup"><span data-stu-id="899d2-151">Response</span></span>
<span data-ttu-id="899d2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="899d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



