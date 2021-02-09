---
title: 更新 mobileAppAssignment
description: 更新 mobileAppAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 811f86578531f23e42b09fe1a26c9bcc21c17168
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155354"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="50ea0-103">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="50ea0-103">Update mobileAppAssignment</span></span>

<span data-ttu-id="50ea0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50ea0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50ea0-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50ea0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50ea0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50ea0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50ea0-107">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="50ea0-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50ea0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="50ea0-108">Prerequisites</span></span>
<span data-ttu-id="50ea0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ea0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="50ea0-111">Permission type</span></span>|<span data-ttu-id="50ea0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50ea0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50ea0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50ea0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50ea0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50ea0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50ea0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50ea0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50ea0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="50ea0-116">Not supported.</span></span>|
|<span data-ttu-id="50ea0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="50ea0-117">Application</span></span>|<span data-ttu-id="50ea0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50ea0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50ea0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50ea0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="50ea0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="50ea0-120">Request headers</span></span>
|<span data-ttu-id="50ea0-121">标头</span><span class="sxs-lookup"><span data-stu-id="50ea0-121">Header</span></span>|<span data-ttu-id="50ea0-122">值</span><span class="sxs-lookup"><span data-stu-id="50ea0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50ea0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50ea0-123">Authorization</span></span>|<span data-ttu-id="50ea0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50ea0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50ea0-125">接受</span><span class="sxs-lookup"><span data-stu-id="50ea0-125">Accept</span></span>|<span data-ttu-id="50ea0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50ea0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50ea0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50ea0-127">Request body</span></span>
<span data-ttu-id="50ea0-128">在请求正文中，提供 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50ea0-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="50ea0-129">下表显示创建 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50ea0-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="50ea0-130">属性</span><span class="sxs-lookup"><span data-stu-id="50ea0-130">Property</span></span>|<span data-ttu-id="50ea0-131">类型</span><span class="sxs-lookup"><span data-stu-id="50ea0-131">Type</span></span>|<span data-ttu-id="50ea0-132">说明</span><span class="sxs-lookup"><span data-stu-id="50ea0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50ea0-133">id</span><span class="sxs-lookup"><span data-stu-id="50ea0-133">id</span></span>|<span data-ttu-id="50ea0-134">String</span><span class="sxs-lookup"><span data-stu-id="50ea0-134">String</span></span>|<span data-ttu-id="50ea0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="50ea0-135">Key of the entity.</span></span>|
|<span data-ttu-id="50ea0-136">intent</span><span class="sxs-lookup"><span data-stu-id="50ea0-136">intent</span></span>|[<span data-ttu-id="50ea0-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="50ea0-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="50ea0-138">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="50ea0-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="50ea0-139">target</span><span class="sxs-lookup"><span data-stu-id="50ea0-139">target</span></span>|[<span data-ttu-id="50ea0-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="50ea0-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="50ea0-141">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="50ea0-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="50ea0-142">settings</span><span class="sxs-lookup"><span data-stu-id="50ea0-142">settings</span></span>|[<span data-ttu-id="50ea0-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="50ea0-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="50ea0-144">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="50ea0-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="50ea0-145">source</span><span class="sxs-lookup"><span data-stu-id="50ea0-145">source</span></span>|[<span data-ttu-id="50ea0-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="50ea0-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="50ea0-147">作为工作分配源的资源类型。</span><span class="sxs-lookup"><span data-stu-id="50ea0-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="50ea0-148">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="50ea0-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="50ea0-149">sourceId</span><span class="sxs-lookup"><span data-stu-id="50ea0-149">sourceId</span></span>|<span data-ttu-id="50ea0-150">String</span><span class="sxs-lookup"><span data-stu-id="50ea0-150">String</span></span>|<span data-ttu-id="50ea0-151">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="50ea0-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="50ea0-152">响应</span><span class="sxs-lookup"><span data-stu-id="50ea0-152">Response</span></span>
<span data-ttu-id="50ea0-153">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50ea0-153">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ea0-154">示例</span><span class="sxs-lookup"><span data-stu-id="50ea0-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="50ea0-155">请求</span><span class="sxs-lookup"><span data-stu-id="50ea0-155">Request</span></span>
<span data-ttu-id="50ea0-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50ea0-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 617

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
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="50ea0-157">响应</span><span class="sxs-lookup"><span data-stu-id="50ea0-157">Response</span></span>
<span data-ttu-id="50ea0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50ea0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

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
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




