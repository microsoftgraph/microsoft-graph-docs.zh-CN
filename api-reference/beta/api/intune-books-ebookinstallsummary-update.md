---
title: 更新 eBookInstallSummary
description: 更新 eBookInstallSummary 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85e94a16799b9ee56c28041549b1d21692013599
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421163"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="e44be-103">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e44be-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="e44be-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e44be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e44be-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e44be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e44be-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e44be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e44be-107">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e44be-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e44be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e44be-108">Prerequisites</span></span>
<span data-ttu-id="e44be-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e44be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e44be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e44be-111">Permission type</span></span>|<span data-ttu-id="e44be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e44be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e44be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e44be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e44be-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e44be-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e44be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e44be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e44be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e44be-116">Not supported.</span></span>|
|<span data-ttu-id="e44be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e44be-117">Application</span></span>|<span data-ttu-id="e44be-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e44be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e44be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e44be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="e44be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e44be-120">Request headers</span></span>
|<span data-ttu-id="e44be-121">标头</span><span class="sxs-lookup"><span data-stu-id="e44be-121">Header</span></span>|<span data-ttu-id="e44be-122">值</span><span class="sxs-lookup"><span data-stu-id="e44be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e44be-123">授权</span><span class="sxs-lookup"><span data-stu-id="e44be-123">Authorization</span></span>|<span data-ttu-id="e44be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e44be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e44be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e44be-125">Accept</span></span>|<span data-ttu-id="e44be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e44be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e44be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e44be-127">Request body</span></span>
<span data-ttu-id="e44be-128">在请求正文中，提供 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e44be-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="e44be-129">下表显示了创建 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e44be-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="e44be-130">属性</span><span class="sxs-lookup"><span data-stu-id="e44be-130">Property</span></span>|<span data-ttu-id="e44be-131">类型</span><span class="sxs-lookup"><span data-stu-id="e44be-131">Type</span></span>|<span data-ttu-id="e44be-132">说明</span><span class="sxs-lookup"><span data-stu-id="e44be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44be-133">id</span><span class="sxs-lookup"><span data-stu-id="e44be-133">id</span></span>|<span data-ttu-id="e44be-134">String</span><span class="sxs-lookup"><span data-stu-id="e44be-134">String</span></span>|<span data-ttu-id="e44be-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e44be-135">Key of the entity.</span></span>|
|<span data-ttu-id="e44be-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e44be-136">installedDeviceCount</span></span>|<span data-ttu-id="e44be-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e44be-137">Int32</span></span>|<span data-ttu-id="e44be-138">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="e44be-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="e44be-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e44be-139">failedDeviceCount</span></span>|<span data-ttu-id="e44be-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e44be-140">Int32</span></span>|<span data-ttu-id="e44be-141">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="e44be-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="e44be-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e44be-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="e44be-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e44be-143">Int32</span></span>|<span data-ttu-id="e44be-144">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="e44be-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="e44be-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="e44be-145">installedUserCount</span></span>|<span data-ttu-id="e44be-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e44be-146">Int32</span></span>|<span data-ttu-id="e44be-147">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="e44be-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="e44be-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="e44be-148">failedUserCount</span></span>|<span data-ttu-id="e44be-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e44be-149">Int32</span></span>|<span data-ttu-id="e44be-150">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="e44be-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="e44be-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="e44be-151">notInstalledUserCount</span></span>|<span data-ttu-id="e44be-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e44be-152">Int32</span></span>|<span data-ttu-id="e44be-153">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="e44be-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="e44be-154">响应</span><span class="sxs-lookup"><span data-stu-id="e44be-154">Response</span></span>
<span data-ttu-id="e44be-155">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e44be-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e44be-156">示例</span><span class="sxs-lookup"><span data-stu-id="e44be-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="e44be-157">请求</span><span class="sxs-lookup"><span data-stu-id="e44be-157">Request</span></span>
<span data-ttu-id="e44be-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e44be-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e44be-159">响应</span><span class="sxs-lookup"><span data-stu-id="e44be-159">Response</span></span>
<span data-ttu-id="e44be-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e44be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




