---
title: 更新 eBookInstallSummary
description: 更新 eBookInstallSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb5e5c0b14b41f4f3ea5c489f87f130d46b49bcd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959381"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="63a41-103">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="63a41-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="63a41-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63a41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63a41-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63a41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63a41-106">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="63a41-106">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63a41-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="63a41-107">Prerequisites</span></span>
<span data-ttu-id="63a41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63a41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a41-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="63a41-110">Permission type</span></span>|<span data-ttu-id="63a41-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63a41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63a41-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63a41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63a41-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a41-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="63a41-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63a41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63a41-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63a41-115">Not supported.</span></span>|
|<span data-ttu-id="63a41-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="63a41-116">Application</span></span>|<span data-ttu-id="63a41-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="63a41-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63a41-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63a41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="63a41-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="63a41-119">Request headers</span></span>
|<span data-ttu-id="63a41-120">标头</span><span class="sxs-lookup"><span data-stu-id="63a41-120">Header</span></span>|<span data-ttu-id="63a41-121">值</span><span class="sxs-lookup"><span data-stu-id="63a41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63a41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63a41-122">Authorization</span></span>|<span data-ttu-id="63a41-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63a41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63a41-124">接受</span><span class="sxs-lookup"><span data-stu-id="63a41-124">Accept</span></span>|<span data-ttu-id="63a41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63a41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63a41-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="63a41-126">Request body</span></span>
<span data-ttu-id="63a41-127">在请求正文中，提供 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63a41-127">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="63a41-128">下表显示了创建 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63a41-128">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="63a41-129">属性</span><span class="sxs-lookup"><span data-stu-id="63a41-129">Property</span></span>|<span data-ttu-id="63a41-130">类型</span><span class="sxs-lookup"><span data-stu-id="63a41-130">Type</span></span>|<span data-ttu-id="63a41-131">说明</span><span class="sxs-lookup"><span data-stu-id="63a41-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63a41-132">id</span><span class="sxs-lookup"><span data-stu-id="63a41-132">id</span></span>|<span data-ttu-id="63a41-133">String</span><span class="sxs-lookup"><span data-stu-id="63a41-133">String</span></span>|<span data-ttu-id="63a41-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63a41-134">Key of the entity.</span></span>|
|<span data-ttu-id="63a41-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63a41-135">installedDeviceCount</span></span>|<span data-ttu-id="63a41-136">Int32</span><span class="sxs-lookup"><span data-stu-id="63a41-136">Int32</span></span>|<span data-ttu-id="63a41-137">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="63a41-137">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="63a41-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63a41-138">failedDeviceCount</span></span>|<span data-ttu-id="63a41-139">Int32</span><span class="sxs-lookup"><span data-stu-id="63a41-139">Int32</span></span>|<span data-ttu-id="63a41-140">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="63a41-140">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="63a41-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63a41-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="63a41-142">Int32</span><span class="sxs-lookup"><span data-stu-id="63a41-142">Int32</span></span>|<span data-ttu-id="63a41-143">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="63a41-143">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="63a41-144">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="63a41-144">installedUserCount</span></span>|<span data-ttu-id="63a41-145">Int32</span><span class="sxs-lookup"><span data-stu-id="63a41-145">Int32</span></span>|<span data-ttu-id="63a41-146">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="63a41-146">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="63a41-147">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="63a41-147">failedUserCount</span></span>|<span data-ttu-id="63a41-148">Int32</span><span class="sxs-lookup"><span data-stu-id="63a41-148">Int32</span></span>|<span data-ttu-id="63a41-149">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="63a41-149">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="63a41-150">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="63a41-150">notInstalledUserCount</span></span>|<span data-ttu-id="63a41-151">Int32</span><span class="sxs-lookup"><span data-stu-id="63a41-151">Int32</span></span>|<span data-ttu-id="63a41-152">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="63a41-152">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="63a41-153">响应</span><span class="sxs-lookup"><span data-stu-id="63a41-153">Response</span></span>
<span data-ttu-id="63a41-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63a41-154">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63a41-155">示例</span><span class="sxs-lookup"><span data-stu-id="63a41-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="63a41-156">请求</span><span class="sxs-lookup"><span data-stu-id="63a41-156">Request</span></span>
<span data-ttu-id="63a41-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63a41-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="63a41-158">响应</span><span class="sxs-lookup"><span data-stu-id="63a41-158">Response</span></span>
<span data-ttu-id="63a41-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63a41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```





