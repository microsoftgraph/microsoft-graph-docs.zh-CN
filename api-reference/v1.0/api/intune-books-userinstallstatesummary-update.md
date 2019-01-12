---
title: 更新 userInstallStateSummary
description: 更新 userInstallStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 67e1ced8cf96c4b3ac51eee314cfd092dcaca8da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972689"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="3de96-103">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="3de96-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="3de96-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3de96-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3de96-105">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3de96-105">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3de96-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3de96-106">Prerequisites</span></span>
<span data-ttu-id="3de96-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3de96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3de96-109">Permission type</span></span>|<span data-ttu-id="3de96-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3de96-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3de96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3de96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3de96-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de96-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3de96-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3de96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3de96-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3de96-114">Not supported.</span></span>|
|<span data-ttu-id="3de96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3de96-115">Application</span></span>|<span data-ttu-id="3de96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3de96-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3de96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3de96-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3de96-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3de96-118">Request headers</span></span>
|<span data-ttu-id="3de96-119">标头</span><span class="sxs-lookup"><span data-stu-id="3de96-119">Header</span></span>|<span data-ttu-id="3de96-120">值</span><span class="sxs-lookup"><span data-stu-id="3de96-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3de96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3de96-121">Authorization</span></span>|<span data-ttu-id="3de96-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3de96-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3de96-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3de96-123">Accept</span></span>|<span data-ttu-id="3de96-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3de96-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de96-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3de96-125">Request body</span></span>
<span data-ttu-id="3de96-126">在请求正文中，提供 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3de96-126">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="3de96-127">下表显示创建 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3de96-127">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="3de96-128">属性</span><span class="sxs-lookup"><span data-stu-id="3de96-128">Property</span></span>|<span data-ttu-id="3de96-129">类型</span><span class="sxs-lookup"><span data-stu-id="3de96-129">Type</span></span>|<span data-ttu-id="3de96-130">说明</span><span class="sxs-lookup"><span data-stu-id="3de96-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de96-131">id</span><span class="sxs-lookup"><span data-stu-id="3de96-131">id</span></span>|<span data-ttu-id="3de96-132">String</span><span class="sxs-lookup"><span data-stu-id="3de96-132">String</span></span>|<span data-ttu-id="3de96-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3de96-133">Key of the entity.</span></span>|
|<span data-ttu-id="3de96-134">userName</span><span class="sxs-lookup"><span data-stu-id="3de96-134">userName</span></span>|<span data-ttu-id="3de96-135">String</span><span class="sxs-lookup"><span data-stu-id="3de96-135">String</span></span>|<span data-ttu-id="3de96-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="3de96-136">User name.</span></span>|
|<span data-ttu-id="3de96-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3de96-137">installedDeviceCount</span></span>|<span data-ttu-id="3de96-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3de96-138">Int32</span></span>|<span data-ttu-id="3de96-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="3de96-139">Installed Device Count.</span></span>|
|<span data-ttu-id="3de96-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3de96-140">failedDeviceCount</span></span>|<span data-ttu-id="3de96-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3de96-141">Int32</span></span>|<span data-ttu-id="3de96-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="3de96-142">Failed Device Count.</span></span>|
|<span data-ttu-id="3de96-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3de96-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="3de96-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3de96-144">Int32</span></span>|<span data-ttu-id="3de96-145">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="3de96-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3de96-146">响应</span><span class="sxs-lookup"><span data-stu-id="3de96-146">Response</span></span>
<span data-ttu-id="3de96-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3de96-147">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de96-148">示例</span><span class="sxs-lookup"><span data-stu-id="3de96-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="3de96-149">请求</span><span class="sxs-lookup"><span data-stu-id="3de96-149">Request</span></span>
<span data-ttu-id="3de96-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3de96-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="3de96-151">响应</span><span class="sxs-lookup"><span data-stu-id="3de96-151">Response</span></span>
<span data-ttu-id="3de96-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3de96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



