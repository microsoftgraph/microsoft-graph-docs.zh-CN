---
title: 更新 userInstallStateSummary
description: 更新 userInstallStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a924db2f3dd97921eddd3c092c60c7f87e1b8b12
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985905"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="b42bd-103">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b42bd-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="b42bd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b42bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b42bd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b42bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b42bd-106">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b42bd-106">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b42bd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b42bd-107">Prerequisites</span></span>
<span data-ttu-id="b42bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b42bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b42bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b42bd-110">Permission type</span></span>|<span data-ttu-id="b42bd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b42bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b42bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b42bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b42bd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b42bd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b42bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b42bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b42bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b42bd-115">Not supported.</span></span>|
|<span data-ttu-id="b42bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b42bd-116">Application</span></span>|<span data-ttu-id="b42bd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b42bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b42bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b42bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b42bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b42bd-119">Request headers</span></span>
|<span data-ttu-id="b42bd-120">标头</span><span class="sxs-lookup"><span data-stu-id="b42bd-120">Header</span></span>|<span data-ttu-id="b42bd-121">值</span><span class="sxs-lookup"><span data-stu-id="b42bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b42bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b42bd-122">Authorization</span></span>|<span data-ttu-id="b42bd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b42bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b42bd-124">接受</span><span class="sxs-lookup"><span data-stu-id="b42bd-124">Accept</span></span>|<span data-ttu-id="b42bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b42bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b42bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b42bd-126">Request body</span></span>
<span data-ttu-id="b42bd-127">在请求正文中，提供 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b42bd-127">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="b42bd-128">下表显示创建 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b42bd-128">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="b42bd-129">属性</span><span class="sxs-lookup"><span data-stu-id="b42bd-129">Property</span></span>|<span data-ttu-id="b42bd-130">类型</span><span class="sxs-lookup"><span data-stu-id="b42bd-130">Type</span></span>|<span data-ttu-id="b42bd-131">说明</span><span class="sxs-lookup"><span data-stu-id="b42bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b42bd-132">id</span><span class="sxs-lookup"><span data-stu-id="b42bd-132">id</span></span>|<span data-ttu-id="b42bd-133">String</span><span class="sxs-lookup"><span data-stu-id="b42bd-133">String</span></span>|<span data-ttu-id="b42bd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b42bd-134">Key of the entity.</span></span>|
|<span data-ttu-id="b42bd-135">userName</span><span class="sxs-lookup"><span data-stu-id="b42bd-135">userName</span></span>|<span data-ttu-id="b42bd-136">String</span><span class="sxs-lookup"><span data-stu-id="b42bd-136">String</span></span>|<span data-ttu-id="b42bd-137">用户名。</span><span class="sxs-lookup"><span data-stu-id="b42bd-137">User name.</span></span>|
|<span data-ttu-id="b42bd-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b42bd-138">installedDeviceCount</span></span>|<span data-ttu-id="b42bd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b42bd-139">Int32</span></span>|<span data-ttu-id="b42bd-140">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b42bd-140">Installed Device Count.</span></span>|
|<span data-ttu-id="b42bd-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b42bd-141">failedDeviceCount</span></span>|<span data-ttu-id="b42bd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b42bd-142">Int32</span></span>|<span data-ttu-id="b42bd-143">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b42bd-143">Failed Device Count.</span></span>|
|<span data-ttu-id="b42bd-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b42bd-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="b42bd-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b42bd-145">Int32</span></span>|<span data-ttu-id="b42bd-146">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b42bd-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="b42bd-147">响应</span><span class="sxs-lookup"><span data-stu-id="b42bd-147">Response</span></span>
<span data-ttu-id="b42bd-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b42bd-148">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b42bd-149">示例</span><span class="sxs-lookup"><span data-stu-id="b42bd-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b42bd-150">请求</span><span class="sxs-lookup"><span data-stu-id="b42bd-150">Request</span></span>
<span data-ttu-id="b42bd-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b42bd-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b42bd-152">响应</span><span class="sxs-lookup"><span data-stu-id="b42bd-152">Response</span></span>
<span data-ttu-id="b42bd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b42bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




