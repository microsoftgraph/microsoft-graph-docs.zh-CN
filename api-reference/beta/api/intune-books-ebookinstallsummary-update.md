---
title: 更新 eBookInstallSummary
description: 更新 eBookInstallSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0af85656faf26c5259f4d2d8d9804d17d655e3ba
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49245450"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="38d54-103">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="38d54-103">Update eBookInstallSummary</span></span>

<span data-ttu-id="38d54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38d54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38d54-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38d54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38d54-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38d54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38d54-107">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38d54-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38d54-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="38d54-108">Prerequisites</span></span>
<span data-ttu-id="38d54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38d54-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38d54-111">Permission type</span></span>|<span data-ttu-id="38d54-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38d54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38d54-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38d54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38d54-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38d54-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38d54-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38d54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38d54-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38d54-116">Not supported.</span></span>|
|<span data-ttu-id="38d54-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="38d54-117">Application</span></span>|<span data-ttu-id="38d54-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38d54-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38d54-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38d54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="38d54-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="38d54-120">Request headers</span></span>
|<span data-ttu-id="38d54-121">标头</span><span class="sxs-lookup"><span data-stu-id="38d54-121">Header</span></span>|<span data-ttu-id="38d54-122">值</span><span class="sxs-lookup"><span data-stu-id="38d54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38d54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38d54-123">Authorization</span></span>|<span data-ttu-id="38d54-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38d54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38d54-125">接受</span><span class="sxs-lookup"><span data-stu-id="38d54-125">Accept</span></span>|<span data-ttu-id="38d54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38d54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38d54-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38d54-127">Request body</span></span>
<span data-ttu-id="38d54-128">在请求正文中，提供 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38d54-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="38d54-129">下表显示了创建 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38d54-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="38d54-130">属性</span><span class="sxs-lookup"><span data-stu-id="38d54-130">Property</span></span>|<span data-ttu-id="38d54-131">类型</span><span class="sxs-lookup"><span data-stu-id="38d54-131">Type</span></span>|<span data-ttu-id="38d54-132">说明</span><span class="sxs-lookup"><span data-stu-id="38d54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38d54-133">id</span><span class="sxs-lookup"><span data-stu-id="38d54-133">id</span></span>|<span data-ttu-id="38d54-134">String</span><span class="sxs-lookup"><span data-stu-id="38d54-134">String</span></span>|<span data-ttu-id="38d54-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="38d54-135">Key of the entity.</span></span>|
|<span data-ttu-id="38d54-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="38d54-136">installedDeviceCount</span></span>|<span data-ttu-id="38d54-137">Int32</span><span class="sxs-lookup"><span data-stu-id="38d54-137">Int32</span></span>|<span data-ttu-id="38d54-138">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="38d54-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="38d54-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="38d54-139">failedDeviceCount</span></span>|<span data-ttu-id="38d54-140">Int32</span><span class="sxs-lookup"><span data-stu-id="38d54-140">Int32</span></span>|<span data-ttu-id="38d54-141">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="38d54-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="38d54-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="38d54-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="38d54-143">Int32</span><span class="sxs-lookup"><span data-stu-id="38d54-143">Int32</span></span>|<span data-ttu-id="38d54-144">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="38d54-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="38d54-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="38d54-145">installedUserCount</span></span>|<span data-ttu-id="38d54-146">Int32</span><span class="sxs-lookup"><span data-stu-id="38d54-146">Int32</span></span>|<span data-ttu-id="38d54-147">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="38d54-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="38d54-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="38d54-148">failedUserCount</span></span>|<span data-ttu-id="38d54-149">Int32</span><span class="sxs-lookup"><span data-stu-id="38d54-149">Int32</span></span>|<span data-ttu-id="38d54-150">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="38d54-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="38d54-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="38d54-151">notInstalledUserCount</span></span>|<span data-ttu-id="38d54-152">Int32</span><span class="sxs-lookup"><span data-stu-id="38d54-152">Int32</span></span>|<span data-ttu-id="38d54-153">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="38d54-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="38d54-154">响应</span><span class="sxs-lookup"><span data-stu-id="38d54-154">Response</span></span>
<span data-ttu-id="38d54-155">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38d54-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38d54-156">示例</span><span class="sxs-lookup"><span data-stu-id="38d54-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="38d54-157">请求</span><span class="sxs-lookup"><span data-stu-id="38d54-157">Request</span></span>
<span data-ttu-id="38d54-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38d54-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38d54-159">响应</span><span class="sxs-lookup"><span data-stu-id="38d54-159">Response</span></span>
<span data-ttu-id="38d54-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38d54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




