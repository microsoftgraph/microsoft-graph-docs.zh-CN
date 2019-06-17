---
title: 创建 userInstallStateSummary
description: 创建新的 userInstallStateSummary 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 058e5d47773172cce3f91da04f1697aa2ded3e47
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972093"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="a6616-103">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a6616-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="a6616-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6616-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6616-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6616-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6616-106">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6616-106">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6616-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6616-107">Prerequisites</span></span>
<span data-ttu-id="a6616-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6616-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6616-110">Permission type</span></span>|<span data-ttu-id="a6616-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6616-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6616-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6616-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6616-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6616-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6616-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6616-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6616-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6616-115">Not supported.</span></span>|
|<span data-ttu-id="a6616-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6616-116">Application</span></span>|<span data-ttu-id="a6616-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6616-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6616-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6616-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="a6616-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6616-119">Request headers</span></span>
|<span data-ttu-id="a6616-120">标头</span><span class="sxs-lookup"><span data-stu-id="a6616-120">Header</span></span>|<span data-ttu-id="a6616-121">值</span><span class="sxs-lookup"><span data-stu-id="a6616-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6616-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6616-122">Authorization</span></span>|<span data-ttu-id="a6616-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6616-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6616-124">接受</span><span class="sxs-lookup"><span data-stu-id="a6616-124">Accept</span></span>|<span data-ttu-id="a6616-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6616-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6616-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6616-126">Request body</span></span>
<span data-ttu-id="a6616-127">在请求正文中，提供 userInstallStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6616-127">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="a6616-128">下表显示创建 userInstallStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6616-128">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="a6616-129">属性</span><span class="sxs-lookup"><span data-stu-id="a6616-129">Property</span></span>|<span data-ttu-id="a6616-130">类型</span><span class="sxs-lookup"><span data-stu-id="a6616-130">Type</span></span>|<span data-ttu-id="a6616-131">说明</span><span class="sxs-lookup"><span data-stu-id="a6616-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6616-132">id</span><span class="sxs-lookup"><span data-stu-id="a6616-132">id</span></span>|<span data-ttu-id="a6616-133">String</span><span class="sxs-lookup"><span data-stu-id="a6616-133">String</span></span>|<span data-ttu-id="a6616-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a6616-134">Key of the entity.</span></span>|
|<span data-ttu-id="a6616-135">userName</span><span class="sxs-lookup"><span data-stu-id="a6616-135">userName</span></span>|<span data-ttu-id="a6616-136">String</span><span class="sxs-lookup"><span data-stu-id="a6616-136">String</span></span>|<span data-ttu-id="a6616-137">用户名。</span><span class="sxs-lookup"><span data-stu-id="a6616-137">User name.</span></span>|
|<span data-ttu-id="a6616-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6616-138">installedDeviceCount</span></span>|<span data-ttu-id="a6616-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a6616-139">Int32</span></span>|<span data-ttu-id="a6616-140">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="a6616-140">Installed Device Count.</span></span>|
|<span data-ttu-id="a6616-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6616-141">failedDeviceCount</span></span>|<span data-ttu-id="a6616-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a6616-142">Int32</span></span>|<span data-ttu-id="a6616-143">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="a6616-143">Failed Device Count.</span></span>|
|<span data-ttu-id="a6616-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a6616-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="a6616-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a6616-145">Int32</span></span>|<span data-ttu-id="a6616-146">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="a6616-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="a6616-147">响应</span><span class="sxs-lookup"><span data-stu-id="a6616-147">Response</span></span>
<span data-ttu-id="a6616-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6616-148">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6616-149">示例</span><span class="sxs-lookup"><span data-stu-id="a6616-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6616-150">请求</span><span class="sxs-lookup"><span data-stu-id="a6616-150">Request</span></span>
<span data-ttu-id="a6616-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6616-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6616-152">响应</span><span class="sxs-lookup"><span data-stu-id="a6616-152">Response</span></span>
<span data-ttu-id="a6616-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6616-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





