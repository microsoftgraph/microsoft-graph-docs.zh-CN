---
title: 更新 userInstallStateSummary
description: 更新 userInstallStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae7167dd1f7482d81478903c431efa2edfb9da7b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166932"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="b64cd-103">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b64cd-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="b64cd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b64cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b64cd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b64cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b64cd-106">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b64cd-106">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b64cd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b64cd-107">Prerequisites</span></span>
<span data-ttu-id="b64cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b64cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b64cd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b64cd-110">Permission type</span></span>|<span data-ttu-id="b64cd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b64cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b64cd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b64cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b64cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b64cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b64cd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b64cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b64cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b64cd-115">Not supported.</span></span>|
|<span data-ttu-id="b64cd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b64cd-116">Application</span></span>|<span data-ttu-id="b64cd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b64cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b64cd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b64cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b64cd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b64cd-119">Request headers</span></span>
|<span data-ttu-id="b64cd-120">标头</span><span class="sxs-lookup"><span data-stu-id="b64cd-120">Header</span></span>|<span data-ttu-id="b64cd-121">值</span><span class="sxs-lookup"><span data-stu-id="b64cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b64cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b64cd-122">Authorization</span></span>|<span data-ttu-id="b64cd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b64cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b64cd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b64cd-124">Accept</span></span>|<span data-ttu-id="b64cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b64cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b64cd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b64cd-126">Request body</span></span>
<span data-ttu-id="b64cd-127">在请求正文中，提供 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b64cd-127">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="b64cd-128">下表显示创建 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b64cd-128">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="b64cd-129">属性</span><span class="sxs-lookup"><span data-stu-id="b64cd-129">Property</span></span>|<span data-ttu-id="b64cd-130">类型</span><span class="sxs-lookup"><span data-stu-id="b64cd-130">Type</span></span>|<span data-ttu-id="b64cd-131">说明</span><span class="sxs-lookup"><span data-stu-id="b64cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b64cd-132">id</span><span class="sxs-lookup"><span data-stu-id="b64cd-132">id</span></span>|<span data-ttu-id="b64cd-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b64cd-133">String</span></span>|<span data-ttu-id="b64cd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b64cd-134">Key of the entity.</span></span>|
|<span data-ttu-id="b64cd-135">userName</span><span class="sxs-lookup"><span data-stu-id="b64cd-135">userName</span></span>|<span data-ttu-id="b64cd-136">String</span><span class="sxs-lookup"><span data-stu-id="b64cd-136">String</span></span>|<span data-ttu-id="b64cd-137">用户名。</span><span class="sxs-lookup"><span data-stu-id="b64cd-137">User name.</span></span>|
|<span data-ttu-id="b64cd-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b64cd-138">installedDeviceCount</span></span>|<span data-ttu-id="b64cd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b64cd-139">Int32</span></span>|<span data-ttu-id="b64cd-140">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b64cd-140">Installed Device Count.</span></span>|
|<span data-ttu-id="b64cd-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b64cd-141">failedDeviceCount</span></span>|<span data-ttu-id="b64cd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b64cd-142">Int32</span></span>|<span data-ttu-id="b64cd-143">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b64cd-143">Failed Device Count.</span></span>|
|<span data-ttu-id="b64cd-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b64cd-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="b64cd-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b64cd-145">Int32</span></span>|<span data-ttu-id="b64cd-146">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b64cd-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="b64cd-147">响应</span><span class="sxs-lookup"><span data-stu-id="b64cd-147">Response</span></span>
<span data-ttu-id="b64cd-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b64cd-148">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b64cd-149">示例</span><span class="sxs-lookup"><span data-stu-id="b64cd-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b64cd-150">请求</span><span class="sxs-lookup"><span data-stu-id="b64cd-150">Request</span></span>
<span data-ttu-id="b64cd-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b64cd-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="b64cd-152">响应</span><span class="sxs-lookup"><span data-stu-id="b64cd-152">Response</span></span>
<span data-ttu-id="b64cd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b64cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




