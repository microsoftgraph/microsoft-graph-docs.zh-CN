---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e0a1d5bb75374307362b5291233afb5b554b6fe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793337"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="b836b-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="b836b-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="b836b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b836b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b836b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b836b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b836b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b836b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b836b-107">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b836b-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b836b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b836b-108">Prerequisites</span></span>
<span data-ttu-id="b836b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b836b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b836b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b836b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b836b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b836b-111">Permission type</span></span>|<span data-ttu-id="b836b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b836b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b836b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b836b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b836b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b836b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b836b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b836b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b836b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b836b-116">Not supported.</span></span>|
|<span data-ttu-id="b836b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b836b-117">Application</span></span>|<span data-ttu-id="b836b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b836b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b836b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b836b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b836b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b836b-120">Request headers</span></span>
|<span data-ttu-id="b836b-121">标头</span><span class="sxs-lookup"><span data-stu-id="b836b-121">Header</span></span>|<span data-ttu-id="b836b-122">值</span><span class="sxs-lookup"><span data-stu-id="b836b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b836b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b836b-123">Authorization</span></span>|<span data-ttu-id="b836b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b836b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b836b-125">接受</span><span class="sxs-lookup"><span data-stu-id="b836b-125">Accept</span></span>|<span data-ttu-id="b836b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b836b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b836b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b836b-127">Request body</span></span>
<span data-ttu-id="b836b-128">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b836b-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="b836b-129">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b836b-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="b836b-130">属性</span><span class="sxs-lookup"><span data-stu-id="b836b-130">Property</span></span>|<span data-ttu-id="b836b-131">类型</span><span class="sxs-lookup"><span data-stu-id="b836b-131">Type</span></span>|<span data-ttu-id="b836b-132">说明</span><span class="sxs-lookup"><span data-stu-id="b836b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b836b-133">id</span><span class="sxs-lookup"><span data-stu-id="b836b-133">id</span></span>|<span data-ttu-id="b836b-134">String</span><span class="sxs-lookup"><span data-stu-id="b836b-134">String</span></span>|<span data-ttu-id="b836b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b836b-135">Key of the entity.</span></span>|
|<span data-ttu-id="b836b-136">intent</span><span class="sxs-lookup"><span data-stu-id="b836b-136">intent</span></span>|[<span data-ttu-id="b836b-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="b836b-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b836b-138">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="b836b-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="b836b-139">target</span><span class="sxs-lookup"><span data-stu-id="b836b-139">target</span></span>|[<span data-ttu-id="b836b-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b836b-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b836b-141">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="b836b-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="b836b-142">settings</span><span class="sxs-lookup"><span data-stu-id="b836b-142">settings</span></span>|[<span data-ttu-id="b836b-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b836b-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="b836b-144">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="b836b-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="b836b-145">source</span><span class="sxs-lookup"><span data-stu-id="b836b-145">source</span></span>|[<span data-ttu-id="b836b-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="b836b-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="b836b-147">资源类型，它是工作分配的源。</span><span class="sxs-lookup"><span data-stu-id="b836b-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="b836b-148">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="b836b-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="b836b-149">sourceId</span><span class="sxs-lookup"><span data-stu-id="b836b-149">sourceId</span></span>|<span data-ttu-id="b836b-150">String</span><span class="sxs-lookup"><span data-stu-id="b836b-150">String</span></span>|<span data-ttu-id="b836b-151">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="b836b-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="b836b-152">响应</span><span class="sxs-lookup"><span data-stu-id="b836b-152">Response</span></span>
<span data-ttu-id="b836b-153">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b836b-153">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b836b-154">示例</span><span class="sxs-lookup"><span data-stu-id="b836b-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="b836b-155">请求</span><span class="sxs-lookup"><span data-stu-id="b836b-155">Request</span></span>
<span data-ttu-id="b836b-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b836b-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="b836b-157">响应</span><span class="sxs-lookup"><span data-stu-id="b836b-157">Response</span></span>
<span data-ttu-id="b836b-158">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b836b-158">Here is an example of the response.</span></span> <span data-ttu-id="b836b-159">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b836b-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b836b-160">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b836b-160">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 640

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



