---
title: 更新 eBookInstallSummary
description: 更新 eBookInstallSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d877e2c0af7df6c0d5c8743c1d43fd8c7d6298a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874632"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="ab6e5-103">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab6e5-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="ab6e5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab6e5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab6e5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab6e5-107">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab6e5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab6e5-108">Prerequisites</span></span>
<span data-ttu-id="ab6e5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ab6e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab6e5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab6e5-111">Permission type</span></span>|<span data-ttu-id="ab6e5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab6e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab6e5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab6e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab6e5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab6e5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab6e5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab6e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab6e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-116">Not supported.</span></span>|
|<span data-ttu-id="ab6e5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab6e5-117">Application</span></span>|<span data-ttu-id="ab6e5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab6e5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab6e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="ab6e5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab6e5-120">Request headers</span></span>
|<span data-ttu-id="ab6e5-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab6e5-121">Header</span></span>|<span data-ttu-id="ab6e5-122">值</span><span class="sxs-lookup"><span data-stu-id="ab6e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab6e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab6e5-123">Authorization</span></span>|<span data-ttu-id="ab6e5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab6e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab6e5-125">Accept</span></span>|<span data-ttu-id="ab6e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab6e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab6e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab6e5-127">Request body</span></span>
<span data-ttu-id="ab6e5-128">在请求正文中，提供 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="ab6e5-129">下表显示了创建 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="ab6e5-130">属性</span><span class="sxs-lookup"><span data-stu-id="ab6e5-130">Property</span></span>|<span data-ttu-id="ab6e5-131">类型</span><span class="sxs-lookup"><span data-stu-id="ab6e5-131">Type</span></span>|<span data-ttu-id="ab6e5-132">说明</span><span class="sxs-lookup"><span data-stu-id="ab6e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab6e5-133">id</span><span class="sxs-lookup"><span data-stu-id="ab6e5-133">id</span></span>|<span data-ttu-id="ab6e5-134">String</span><span class="sxs-lookup"><span data-stu-id="ab6e5-134">String</span></span>|<span data-ttu-id="ab6e5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-135">Key of the entity.</span></span>|
|<span data-ttu-id="ab6e5-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab6e5-136">installedDeviceCount</span></span>|<span data-ttu-id="ab6e5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ab6e5-137">Int32</span></span>|<span data-ttu-id="ab6e5-138">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ab6e5-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab6e5-139">failedDeviceCount</span></span>|<span data-ttu-id="ab6e5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ab6e5-140">Int32</span></span>|<span data-ttu-id="ab6e5-141">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ab6e5-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab6e5-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="ab6e5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ab6e5-143">Int32</span></span>|<span data-ttu-id="ab6e5-144">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ab6e5-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ab6e5-145">installedUserCount</span></span>|<span data-ttu-id="ab6e5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ab6e5-146">Int32</span></span>|<span data-ttu-id="ab6e5-147">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ab6e5-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ab6e5-148">failedUserCount</span></span>|<span data-ttu-id="ab6e5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ab6e5-149">Int32</span></span>|<span data-ttu-id="ab6e5-150">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ab6e5-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ab6e5-151">notInstalledUserCount</span></span>|<span data-ttu-id="ab6e5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ab6e5-152">Int32</span></span>|<span data-ttu-id="ab6e5-153">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="ab6e5-154">响应</span><span class="sxs-lookup"><span data-stu-id="ab6e5-154">Response</span></span>
<span data-ttu-id="ab6e5-155">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab6e5-156">示例</span><span class="sxs-lookup"><span data-stu-id="ab6e5-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab6e5-157">请求</span><span class="sxs-lookup"><span data-stu-id="ab6e5-157">Request</span></span>
<span data-ttu-id="ab6e5-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="ab6e5-159">响应</span><span class="sxs-lookup"><span data-stu-id="ab6e5-159">Response</span></span>
<span data-ttu-id="ab6e5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab6e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





