---
title: 创建 userInstallStateSummary
description: 创建新的 userInstallStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 32f7b427143c8fa1d31302d51417c330cd3ca32d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985905"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="06072-103">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="06072-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="06072-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="06072-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06072-105">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06072-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06072-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="06072-106">Prerequisites</span></span>
<span data-ttu-id="06072-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="06072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06072-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06072-109">Permission type</span></span>|<span data-ttu-id="06072-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06072-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06072-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06072-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06072-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06072-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06072-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06072-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06072-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06072-114">Not supported.</span></span>|
|<span data-ttu-id="06072-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06072-115">Application</span></span>|<span data-ttu-id="06072-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06072-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06072-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06072-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="06072-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="06072-118">Request headers</span></span>
|<span data-ttu-id="06072-119">标头</span><span class="sxs-lookup"><span data-stu-id="06072-119">Header</span></span>|<span data-ttu-id="06072-120">值</span><span class="sxs-lookup"><span data-stu-id="06072-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06072-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06072-121">Authorization</span></span>|<span data-ttu-id="06072-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06072-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06072-123">Accept</span><span class="sxs-lookup"><span data-stu-id="06072-123">Accept</span></span>|<span data-ttu-id="06072-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06072-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06072-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="06072-125">Request body</span></span>
<span data-ttu-id="06072-126">在请求正文中，提供 userInstallStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06072-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="06072-127">下表显示创建 userInstallStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06072-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="06072-128">属性</span><span class="sxs-lookup"><span data-stu-id="06072-128">Property</span></span>|<span data-ttu-id="06072-129">类型</span><span class="sxs-lookup"><span data-stu-id="06072-129">Type</span></span>|<span data-ttu-id="06072-130">说明</span><span class="sxs-lookup"><span data-stu-id="06072-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06072-131">id</span><span class="sxs-lookup"><span data-stu-id="06072-131">id</span></span>|<span data-ttu-id="06072-132">String</span><span class="sxs-lookup"><span data-stu-id="06072-132">String</span></span>|<span data-ttu-id="06072-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06072-133">Key of the entity.</span></span>|
|<span data-ttu-id="06072-134">userName</span><span class="sxs-lookup"><span data-stu-id="06072-134">userName</span></span>|<span data-ttu-id="06072-135">String</span><span class="sxs-lookup"><span data-stu-id="06072-135">String</span></span>|<span data-ttu-id="06072-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="06072-136">User name.</span></span>|
|<span data-ttu-id="06072-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06072-137">installedDeviceCount</span></span>|<span data-ttu-id="06072-138">Int32</span><span class="sxs-lookup"><span data-stu-id="06072-138">Int32</span></span>|<span data-ttu-id="06072-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="06072-139">Installed Device Count.</span></span>|
|<span data-ttu-id="06072-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06072-140">failedDeviceCount</span></span>|<span data-ttu-id="06072-141">Int32</span><span class="sxs-lookup"><span data-stu-id="06072-141">Int32</span></span>|<span data-ttu-id="06072-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="06072-142">Failed Device Count.</span></span>|
|<span data-ttu-id="06072-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06072-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="06072-144">Int32</span><span class="sxs-lookup"><span data-stu-id="06072-144">Int32</span></span>|<span data-ttu-id="06072-145">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="06072-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="06072-146">响应</span><span class="sxs-lookup"><span data-stu-id="06072-146">Response</span></span>
<span data-ttu-id="06072-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06072-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06072-148">示例</span><span class="sxs-lookup"><span data-stu-id="06072-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="06072-149">请求</span><span class="sxs-lookup"><span data-stu-id="06072-149">Request</span></span>
<span data-ttu-id="06072-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06072-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="06072-151">响应</span><span class="sxs-lookup"><span data-stu-id="06072-151">Response</span></span>
<span data-ttu-id="06072-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06072-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



