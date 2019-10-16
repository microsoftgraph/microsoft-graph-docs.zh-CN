---
title: 更新 mobileAppAssignment
description: 更新 mobileAppAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 005a6dcb32bee964a85023479cae5a35b6390443
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535161"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="66664-103">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="66664-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="66664-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66664-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66664-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66664-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66664-106">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="66664-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66664-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="66664-107">Prerequisites</span></span>
<span data-ttu-id="66664-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66664-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66664-110">Permission type</span></span>|<span data-ttu-id="66664-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66664-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66664-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66664-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66664-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66664-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66664-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66664-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66664-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66664-115">Not supported.</span></span>|
|<span data-ttu-id="66664-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66664-116">Application</span></span>|<span data-ttu-id="66664-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66664-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66664-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66664-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="66664-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="66664-119">Request headers</span></span>
|<span data-ttu-id="66664-120">标头</span><span class="sxs-lookup"><span data-stu-id="66664-120">Header</span></span>|<span data-ttu-id="66664-121">值</span><span class="sxs-lookup"><span data-stu-id="66664-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66664-122">授权</span><span class="sxs-lookup"><span data-stu-id="66664-122">Authorization</span></span>|<span data-ttu-id="66664-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66664-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66664-124">接受</span><span class="sxs-lookup"><span data-stu-id="66664-124">Accept</span></span>|<span data-ttu-id="66664-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66664-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66664-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66664-126">Request body</span></span>
<span data-ttu-id="66664-127">在请求正文中，提供 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66664-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="66664-128">下表显示创建 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66664-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="66664-129">属性</span><span class="sxs-lookup"><span data-stu-id="66664-129">Property</span></span>|<span data-ttu-id="66664-130">类型</span><span class="sxs-lookup"><span data-stu-id="66664-130">Type</span></span>|<span data-ttu-id="66664-131">说明</span><span class="sxs-lookup"><span data-stu-id="66664-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66664-132">id</span><span class="sxs-lookup"><span data-stu-id="66664-132">id</span></span>|<span data-ttu-id="66664-133">字符串</span><span class="sxs-lookup"><span data-stu-id="66664-133">String</span></span>|<span data-ttu-id="66664-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66664-134">Key of the entity.</span></span>|
|<span data-ttu-id="66664-135">intent</span><span class="sxs-lookup"><span data-stu-id="66664-135">intent</span></span>|[<span data-ttu-id="66664-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="66664-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="66664-137">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="66664-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="66664-138">target</span><span class="sxs-lookup"><span data-stu-id="66664-138">target</span></span>|[<span data-ttu-id="66664-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="66664-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="66664-140">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="66664-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="66664-141">settings</span><span class="sxs-lookup"><span data-stu-id="66664-141">settings</span></span>|[<span data-ttu-id="66664-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="66664-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="66664-143">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="66664-143">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="66664-144">source</span><span class="sxs-lookup"><span data-stu-id="66664-144">source</span></span>|[<span data-ttu-id="66664-145">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="66664-145">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="66664-146">资源类型，它是工作分配的源。</span><span class="sxs-lookup"><span data-stu-id="66664-146">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="66664-147">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="66664-147">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="66664-148">sourceId</span><span class="sxs-lookup"><span data-stu-id="66664-148">sourceId</span></span>|<span data-ttu-id="66664-149">字符串</span><span class="sxs-lookup"><span data-stu-id="66664-149">String</span></span>|<span data-ttu-id="66664-150">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="66664-150">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="66664-151">响应</span><span class="sxs-lookup"><span data-stu-id="66664-151">Response</span></span>
<span data-ttu-id="66664-152">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66664-152">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66664-153">示例</span><span class="sxs-lookup"><span data-stu-id="66664-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="66664-154">请求</span><span class="sxs-lookup"><span data-stu-id="66664-154">Request</span></span>
<span data-ttu-id="66664-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66664-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="66664-156">响应</span><span class="sxs-lookup"><span data-stu-id="66664-156">Response</span></span>
<span data-ttu-id="66664-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66664-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```






