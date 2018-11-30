---
title: 更新 eBookInstallSummary
description: 更新 eBookInstallSummary 对象的属性。
ms.openlocfilehash: a3484eed0a52278616039b7cc5e2427f4a0e1510
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049331"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="70bf9-103">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="70bf9-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="70bf9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="70bf9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70bf9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="70bf9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70bf9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="70bf9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70bf9-107">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="70bf9-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70bf9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="70bf9-108">Prerequisites</span></span>
<span data-ttu-id="70bf9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="70bf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70bf9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="70bf9-111">Permission type</span></span>|<span data-ttu-id="70bf9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="70bf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70bf9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70bf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70bf9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70bf9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70bf9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70bf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70bf9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70bf9-116">Not supported.</span></span>|
|<span data-ttu-id="70bf9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70bf9-117">Application</span></span>|<span data-ttu-id="70bf9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="70bf9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70bf9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70bf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="70bf9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70bf9-120">Request headers</span></span>
|<span data-ttu-id="70bf9-121">标头</span><span class="sxs-lookup"><span data-stu-id="70bf9-121">Header</span></span>|<span data-ttu-id="70bf9-122">值</span><span class="sxs-lookup"><span data-stu-id="70bf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70bf9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70bf9-123">Authorization</span></span>|<span data-ttu-id="70bf9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70bf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70bf9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70bf9-125">Accept</span></span>|<span data-ttu-id="70bf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70bf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70bf9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70bf9-127">Request body</span></span>
<span data-ttu-id="70bf9-128">在请求正文中，提供 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70bf9-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="70bf9-129">下表显示了创建 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="70bf9-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="70bf9-130">属性</span><span class="sxs-lookup"><span data-stu-id="70bf9-130">Property</span></span>|<span data-ttu-id="70bf9-131">类型</span><span class="sxs-lookup"><span data-stu-id="70bf9-131">Type</span></span>|<span data-ttu-id="70bf9-132">说明</span><span class="sxs-lookup"><span data-stu-id="70bf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70bf9-133">id</span><span class="sxs-lookup"><span data-stu-id="70bf9-133">id</span></span>|<span data-ttu-id="70bf9-134">String</span><span class="sxs-lookup"><span data-stu-id="70bf9-134">String</span></span>|<span data-ttu-id="70bf9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="70bf9-135">Key of the entity.</span></span>|
|<span data-ttu-id="70bf9-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70bf9-136">installedDeviceCount</span></span>|<span data-ttu-id="70bf9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="70bf9-137">Int32</span></span>|<span data-ttu-id="70bf9-138">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="70bf9-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="70bf9-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70bf9-139">failedDeviceCount</span></span>|<span data-ttu-id="70bf9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="70bf9-140">Int32</span></span>|<span data-ttu-id="70bf9-141">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="70bf9-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="70bf9-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70bf9-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="70bf9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="70bf9-143">Int32</span></span>|<span data-ttu-id="70bf9-144">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="70bf9-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="70bf9-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="70bf9-145">installedUserCount</span></span>|<span data-ttu-id="70bf9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="70bf9-146">Int32</span></span>|<span data-ttu-id="70bf9-147">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="70bf9-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="70bf9-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="70bf9-148">failedUserCount</span></span>|<span data-ttu-id="70bf9-149">Int32</span><span class="sxs-lookup"><span data-stu-id="70bf9-149">Int32</span></span>|<span data-ttu-id="70bf9-150">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="70bf9-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="70bf9-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="70bf9-151">notInstalledUserCount</span></span>|<span data-ttu-id="70bf9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="70bf9-152">Int32</span></span>|<span data-ttu-id="70bf9-153">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="70bf9-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="70bf9-154">响应</span><span class="sxs-lookup"><span data-stu-id="70bf9-154">Response</span></span>
<span data-ttu-id="70bf9-155">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70bf9-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70bf9-156">示例</span><span class="sxs-lookup"><span data-stu-id="70bf9-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="70bf9-157">请求</span><span class="sxs-lookup"><span data-stu-id="70bf9-157">Request</span></span>
<span data-ttu-id="70bf9-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70bf9-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70bf9-159">响应</span><span class="sxs-lookup"><span data-stu-id="70bf9-159">Response</span></span>
<span data-ttu-id="70bf9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70bf9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





