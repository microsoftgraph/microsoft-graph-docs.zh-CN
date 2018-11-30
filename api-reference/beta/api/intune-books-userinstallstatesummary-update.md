---
title: 更新 userInstallStateSummary
description: 更新 userInstallStateSummary 对象的属性。
ms.openlocfilehash: b161cac0cc2d3ee0fd31662318ef2bb94232dc63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047846"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="6f5fc-103">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="6f5fc-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="6f5fc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f5fc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f5fc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f5fc-107">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f5fc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f5fc-108">Prerequisites</span></span>
<span data-ttu-id="6f5fc-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6f5fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f5fc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f5fc-111">Permission type</span></span>|<span data-ttu-id="6f5fc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f5fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f5fc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f5fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f5fc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f5fc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f5fc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f5fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f5fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-116">Not supported.</span></span>|
|<span data-ttu-id="6f5fc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f5fc-117">Application</span></span>|<span data-ttu-id="6f5fc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f5fc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f5fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="6f5fc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f5fc-120">Request headers</span></span>
|<span data-ttu-id="6f5fc-121">标头</span><span class="sxs-lookup"><span data-stu-id="6f5fc-121">Header</span></span>|<span data-ttu-id="6f5fc-122">值</span><span class="sxs-lookup"><span data-stu-id="6f5fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f5fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f5fc-123">Authorization</span></span>|<span data-ttu-id="6f5fc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f5fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f5fc-125">Accept</span></span>|<span data-ttu-id="6f5fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f5fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f5fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f5fc-127">Request body</span></span>
<span data-ttu-id="6f5fc-128">在请求正文中，提供 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="6f5fc-129">下表显示创建 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="6f5fc-130">属性</span><span class="sxs-lookup"><span data-stu-id="6f5fc-130">Property</span></span>|<span data-ttu-id="6f5fc-131">类型</span><span class="sxs-lookup"><span data-stu-id="6f5fc-131">Type</span></span>|<span data-ttu-id="6f5fc-132">说明</span><span class="sxs-lookup"><span data-stu-id="6f5fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f5fc-133">id</span><span class="sxs-lookup"><span data-stu-id="6f5fc-133">id</span></span>|<span data-ttu-id="6f5fc-134">String</span><span class="sxs-lookup"><span data-stu-id="6f5fc-134">String</span></span>|<span data-ttu-id="6f5fc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-135">Key of the entity.</span></span>|
|<span data-ttu-id="6f5fc-136">userName</span><span class="sxs-lookup"><span data-stu-id="6f5fc-136">userName</span></span>|<span data-ttu-id="6f5fc-137">String</span><span class="sxs-lookup"><span data-stu-id="6f5fc-137">String</span></span>|<span data-ttu-id="6f5fc-138">用户名。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-138">User name.</span></span>|
|<span data-ttu-id="6f5fc-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6f5fc-139">installedDeviceCount</span></span>|<span data-ttu-id="6f5fc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5fc-140">Int32</span></span>|<span data-ttu-id="6f5fc-141">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-141">Installed Device Count.</span></span>|
|<span data-ttu-id="6f5fc-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6f5fc-142">failedDeviceCount</span></span>|<span data-ttu-id="6f5fc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5fc-143">Int32</span></span>|<span data-ttu-id="6f5fc-144">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-144">Failed Device Count.</span></span>|
|<span data-ttu-id="6f5fc-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6f5fc-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="6f5fc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5fc-146">Int32</span></span>|<span data-ttu-id="6f5fc-147">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="6f5fc-148">响应</span><span class="sxs-lookup"><span data-stu-id="6f5fc-148">Response</span></span>
<span data-ttu-id="6f5fc-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f5fc-150">示例</span><span class="sxs-lookup"><span data-stu-id="6f5fc-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f5fc-151">请求</span><span class="sxs-lookup"><span data-stu-id="6f5fc-151">Request</span></span>
<span data-ttu-id="6f5fc-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 127

{
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="6f5fc-153">响应</span><span class="sxs-lookup"><span data-stu-id="6f5fc-153">Response</span></span>
<span data-ttu-id="6f5fc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f5fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





