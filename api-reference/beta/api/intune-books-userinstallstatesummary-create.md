---
title: 创建 userInstallStateSummary
description: 创建新的 userInstallStateSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4383e1e7d995d808215d3777638db7c77084b57c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975442"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="c8ed1-103">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8ed1-103">Create userInstallStateSummary</span></span>

<span data-ttu-id="c8ed1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8ed1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8ed1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8ed1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8ed1-107">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8ed1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c8ed1-108">Prerequisites</span></span>
<span data-ttu-id="c8ed1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8ed1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8ed1-111">Permission type</span></span>|<span data-ttu-id="c8ed1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8ed1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8ed1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8ed1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8ed1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ed1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8ed1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8ed1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8ed1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-116">Not supported.</span></span>|
|<span data-ttu-id="c8ed1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8ed1-117">Application</span></span>|<span data-ttu-id="c8ed1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ed1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8ed1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8ed1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c8ed1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8ed1-120">Request headers</span></span>
|<span data-ttu-id="c8ed1-121">标头</span><span class="sxs-lookup"><span data-stu-id="c8ed1-121">Header</span></span>|<span data-ttu-id="c8ed1-122">值</span><span class="sxs-lookup"><span data-stu-id="c8ed1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8ed1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8ed1-123">Authorization</span></span>|<span data-ttu-id="c8ed1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8ed1-125">接受</span><span class="sxs-lookup"><span data-stu-id="c8ed1-125">Accept</span></span>|<span data-ttu-id="c8ed1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8ed1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8ed1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8ed1-127">Request body</span></span>
<span data-ttu-id="c8ed1-128">在请求正文中，提供 userInstallStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="c8ed1-129">下表显示创建 userInstallStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="c8ed1-130">属性</span><span class="sxs-lookup"><span data-stu-id="c8ed1-130">Property</span></span>|<span data-ttu-id="c8ed1-131">类型</span><span class="sxs-lookup"><span data-stu-id="c8ed1-131">Type</span></span>|<span data-ttu-id="c8ed1-132">说明</span><span class="sxs-lookup"><span data-stu-id="c8ed1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8ed1-133">id</span><span class="sxs-lookup"><span data-stu-id="c8ed1-133">id</span></span>|<span data-ttu-id="c8ed1-134">String</span><span class="sxs-lookup"><span data-stu-id="c8ed1-134">String</span></span>|<span data-ttu-id="c8ed1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-135">Key of the entity.</span></span>|
|<span data-ttu-id="c8ed1-136">userName</span><span class="sxs-lookup"><span data-stu-id="c8ed1-136">userName</span></span>|<span data-ttu-id="c8ed1-137">String</span><span class="sxs-lookup"><span data-stu-id="c8ed1-137">String</span></span>|<span data-ttu-id="c8ed1-138">用户名。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-138">User name.</span></span>|
|<span data-ttu-id="c8ed1-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8ed1-139">installedDeviceCount</span></span>|<span data-ttu-id="c8ed1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c8ed1-140">Int32</span></span>|<span data-ttu-id="c8ed1-141">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-141">Installed Device Count.</span></span>|
|<span data-ttu-id="c8ed1-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8ed1-142">failedDeviceCount</span></span>|<span data-ttu-id="c8ed1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c8ed1-143">Int32</span></span>|<span data-ttu-id="c8ed1-144">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-144">Failed Device Count.</span></span>|
|<span data-ttu-id="c8ed1-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8ed1-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="c8ed1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c8ed1-146">Int32</span></span>|<span data-ttu-id="c8ed1-147">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="c8ed1-148">响应</span><span class="sxs-lookup"><span data-stu-id="c8ed1-148">Response</span></span>
<span data-ttu-id="c8ed1-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8ed1-150">示例</span><span class="sxs-lookup"><span data-stu-id="c8ed1-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8ed1-151">请求</span><span class="sxs-lookup"><span data-stu-id="c8ed1-151">Request</span></span>
<span data-ttu-id="c8ed1-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="c8ed1-153">响应</span><span class="sxs-lookup"><span data-stu-id="c8ed1-153">Response</span></span>
<span data-ttu-id="c8ed1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8ed1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






