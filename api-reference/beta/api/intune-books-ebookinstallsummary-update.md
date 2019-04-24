---
title: 更新 eBookInstallSummary
description: 更新 eBookInstallSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0864a6c2a6a3dfa8be534f1102d2f292e25e6e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483787"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="d1910-103">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d1910-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="d1910-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1910-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1910-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1910-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1910-106">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d1910-106">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1910-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1910-107">Prerequisites</span></span>
<span data-ttu-id="d1910-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1910-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1910-110">Permission type</span></span>|<span data-ttu-id="d1910-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1910-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1910-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1910-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1910-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1910-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1910-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1910-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1910-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1910-115">Not supported.</span></span>|
|<span data-ttu-id="d1910-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1910-116">Application</span></span>|<span data-ttu-id="d1910-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1910-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1910-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1910-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="d1910-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1910-119">Request headers</span></span>
|<span data-ttu-id="d1910-120">标头</span><span class="sxs-lookup"><span data-stu-id="d1910-120">Header</span></span>|<span data-ttu-id="d1910-121">值</span><span class="sxs-lookup"><span data-stu-id="d1910-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1910-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1910-122">Authorization</span></span>|<span data-ttu-id="d1910-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1910-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1910-124">接受</span><span class="sxs-lookup"><span data-stu-id="d1910-124">Accept</span></span>|<span data-ttu-id="d1910-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1910-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1910-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1910-126">Request body</span></span>
<span data-ttu-id="d1910-127">在请求正文中，提供 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1910-127">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="d1910-128">下表显示了创建 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d1910-128">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="d1910-129">属性</span><span class="sxs-lookup"><span data-stu-id="d1910-129">Property</span></span>|<span data-ttu-id="d1910-130">类型</span><span class="sxs-lookup"><span data-stu-id="d1910-130">Type</span></span>|<span data-ttu-id="d1910-131">说明</span><span class="sxs-lookup"><span data-stu-id="d1910-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1910-132">id</span><span class="sxs-lookup"><span data-stu-id="d1910-132">id</span></span>|<span data-ttu-id="d1910-133">String</span><span class="sxs-lookup"><span data-stu-id="d1910-133">String</span></span>|<span data-ttu-id="d1910-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d1910-134">Key of the entity.</span></span>|
|<span data-ttu-id="d1910-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1910-135">installedDeviceCount</span></span>|<span data-ttu-id="d1910-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d1910-136">Int32</span></span>|<span data-ttu-id="d1910-137">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d1910-137">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="d1910-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1910-138">failedDeviceCount</span></span>|<span data-ttu-id="d1910-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d1910-139">Int32</span></span>|<span data-ttu-id="d1910-140">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d1910-140">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="d1910-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1910-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="d1910-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d1910-142">Int32</span></span>|<span data-ttu-id="d1910-143">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d1910-143">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="d1910-144">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="d1910-144">installedUserCount</span></span>|<span data-ttu-id="d1910-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d1910-145">Int32</span></span>|<span data-ttu-id="d1910-146">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d1910-146">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="d1910-147">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="d1910-147">failedUserCount</span></span>|<span data-ttu-id="d1910-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d1910-148">Int32</span></span>|<span data-ttu-id="d1910-149">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d1910-149">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="d1910-150">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="d1910-150">notInstalledUserCount</span></span>|<span data-ttu-id="d1910-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d1910-151">Int32</span></span>|<span data-ttu-id="d1910-152">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d1910-152">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="d1910-153">响应</span><span class="sxs-lookup"><span data-stu-id="d1910-153">Response</span></span>
<span data-ttu-id="d1910-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1910-154">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1910-155">示例</span><span class="sxs-lookup"><span data-stu-id="d1910-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1910-156">请求</span><span class="sxs-lookup"><span data-stu-id="d1910-156">Request</span></span>
<span data-ttu-id="d1910-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1910-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1910-158">响应</span><span class="sxs-lookup"><span data-stu-id="d1910-158">Response</span></span>
<span data-ttu-id="d1910-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1910-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





