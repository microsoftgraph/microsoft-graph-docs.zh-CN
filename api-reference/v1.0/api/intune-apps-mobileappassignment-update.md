---
title: 更新 mobileAppAssignment
description: 更新 mobileAppAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 210001e95cadddf8c6c70ceeab7c54d650a0acfb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464885"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="7cfa9-103">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="7cfa9-103">Update mobileAppAssignment</span></span>

<span data-ttu-id="7cfa9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cfa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7cfa9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cfa9-106">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cfa9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7cfa9-107">Prerequisites</span></span>
<span data-ttu-id="7cfa9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cfa9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cfa9-110">Permission type</span></span>|<span data-ttu-id="7cfa9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7cfa9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cfa9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cfa9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cfa9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cfa9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7cfa9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cfa9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cfa9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-115">Not supported.</span></span>|
|<span data-ttu-id="7cfa9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cfa9-116">Application</span></span>|<span data-ttu-id="7cfa9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cfa9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cfa9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7cfa9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cfa9-119">Request headers</span></span>
|<span data-ttu-id="7cfa9-120">标头</span><span class="sxs-lookup"><span data-stu-id="7cfa9-120">Header</span></span>|<span data-ttu-id="7cfa9-121">值</span><span class="sxs-lookup"><span data-stu-id="7cfa9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cfa9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cfa9-122">Authorization</span></span>|<span data-ttu-id="7cfa9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cfa9-124">接受</span><span class="sxs-lookup"><span data-stu-id="7cfa9-124">Accept</span></span>|<span data-ttu-id="7cfa9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7cfa9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cfa9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cfa9-126">Request body</span></span>
<span data-ttu-id="7cfa9-127">在请求正文中，提供 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="7cfa9-128">下表显示创建 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="7cfa9-129">属性</span><span class="sxs-lookup"><span data-stu-id="7cfa9-129">Property</span></span>|<span data-ttu-id="7cfa9-130">类型</span><span class="sxs-lookup"><span data-stu-id="7cfa9-130">Type</span></span>|<span data-ttu-id="7cfa9-131">说明</span><span class="sxs-lookup"><span data-stu-id="7cfa9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cfa9-132">id</span><span class="sxs-lookup"><span data-stu-id="7cfa9-132">id</span></span>|<span data-ttu-id="7cfa9-133">String</span><span class="sxs-lookup"><span data-stu-id="7cfa9-133">String</span></span>|<span data-ttu-id="7cfa9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-134">Key of the entity.</span></span>|
|<span data-ttu-id="7cfa9-135">intent</span><span class="sxs-lookup"><span data-stu-id="7cfa9-135">intent</span></span>|[<span data-ttu-id="7cfa9-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="7cfa9-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7cfa9-137">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="7cfa9-138">target</span><span class="sxs-lookup"><span data-stu-id="7cfa9-138">target</span></span>|[<span data-ttu-id="7cfa9-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7cfa9-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7cfa9-140">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="7cfa9-141">settings</span><span class="sxs-lookup"><span data-stu-id="7cfa9-141">settings</span></span>|[<span data-ttu-id="7cfa9-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7cfa9-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="7cfa9-143">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="7cfa9-144">响应</span><span class="sxs-lookup"><span data-stu-id="7cfa9-144">Response</span></span>
<span data-ttu-id="7cfa9-145">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cfa9-146">示例</span><span class="sxs-lookup"><span data-stu-id="7cfa9-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cfa9-147">请求</span><span class="sxs-lookup"><span data-stu-id="7cfa9-147">Request</span></span>
<span data-ttu-id="7cfa9-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="7cfa9-149">响应</span><span class="sxs-lookup"><span data-stu-id="7cfa9-149">Response</span></span>
<span data-ttu-id="7cfa9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7cfa9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```






