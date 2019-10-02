---
title: 更新 eBookInstallSummary
description: 更新 eBookInstallSummary 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a432d9e341f83d85f487e4fe1f4ef32d806d2f7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354810"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="1aed7-103">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1aed7-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="1aed7-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1aed7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aed7-105">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1aed7-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1aed7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1aed7-106">Prerequisites</span></span>
<span data-ttu-id="1aed7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1aed7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aed7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1aed7-109">Permission type</span></span>|<span data-ttu-id="1aed7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1aed7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aed7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1aed7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1aed7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aed7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1aed7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1aed7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aed7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1aed7-114">Not supported.</span></span>|
|<span data-ttu-id="1aed7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1aed7-115">Application</span></span>|<span data-ttu-id="1aed7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1aed7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aed7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1aed7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="1aed7-118">请求头</span><span class="sxs-lookup"><span data-stu-id="1aed7-118">Request headers</span></span>
|<span data-ttu-id="1aed7-119">标头</span><span class="sxs-lookup"><span data-stu-id="1aed7-119">Header</span></span>|<span data-ttu-id="1aed7-120">值</span><span class="sxs-lookup"><span data-stu-id="1aed7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aed7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aed7-121">Authorization</span></span>|<span data-ttu-id="1aed7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1aed7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aed7-123">接受</span><span class="sxs-lookup"><span data-stu-id="1aed7-123">Accept</span></span>|<span data-ttu-id="1aed7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1aed7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aed7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1aed7-125">Request body</span></span>
<span data-ttu-id="1aed7-126">在请求正文中，提供 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aed7-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="1aed7-127">下表显示了创建 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1aed7-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="1aed7-128">属性</span><span class="sxs-lookup"><span data-stu-id="1aed7-128">Property</span></span>|<span data-ttu-id="1aed7-129">类型</span><span class="sxs-lookup"><span data-stu-id="1aed7-129">Type</span></span>|<span data-ttu-id="1aed7-130">说明</span><span class="sxs-lookup"><span data-stu-id="1aed7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aed7-131">id</span><span class="sxs-lookup"><span data-stu-id="1aed7-131">id</span></span>|<span data-ttu-id="1aed7-132">String</span><span class="sxs-lookup"><span data-stu-id="1aed7-132">String</span></span>|<span data-ttu-id="1aed7-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1aed7-133">Key of the entity.</span></span>|
|<span data-ttu-id="1aed7-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1aed7-134">installedDeviceCount</span></span>|<span data-ttu-id="1aed7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="1aed7-135">Int32</span></span>|<span data-ttu-id="1aed7-136">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="1aed7-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="1aed7-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1aed7-137">failedDeviceCount</span></span>|<span data-ttu-id="1aed7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1aed7-138">Int32</span></span>|<span data-ttu-id="1aed7-139">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="1aed7-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="1aed7-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1aed7-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="1aed7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1aed7-141">Int32</span></span>|<span data-ttu-id="1aed7-142">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="1aed7-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="1aed7-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="1aed7-143">installedUserCount</span></span>|<span data-ttu-id="1aed7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1aed7-144">Int32</span></span>|<span data-ttu-id="1aed7-145">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="1aed7-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="1aed7-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="1aed7-146">failedUserCount</span></span>|<span data-ttu-id="1aed7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1aed7-147">Int32</span></span>|<span data-ttu-id="1aed7-148">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="1aed7-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="1aed7-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="1aed7-149">notInstalledUserCount</span></span>|<span data-ttu-id="1aed7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1aed7-150">Int32</span></span>|<span data-ttu-id="1aed7-151">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="1aed7-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="1aed7-152">响应</span><span class="sxs-lookup"><span data-stu-id="1aed7-152">Response</span></span>
<span data-ttu-id="1aed7-153">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1aed7-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aed7-154">示例</span><span class="sxs-lookup"><span data-stu-id="1aed7-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aed7-155">请求</span><span class="sxs-lookup"><span data-stu-id="1aed7-155">Request</span></span>
<span data-ttu-id="1aed7-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1aed7-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
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

### <a name="response"></a><span data-ttu-id="1aed7-157">响应</span><span class="sxs-lookup"><span data-stu-id="1aed7-157">Response</span></span>
<span data-ttu-id="1aed7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1aed7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




