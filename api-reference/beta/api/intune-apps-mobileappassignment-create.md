---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5a3894b183d8edae03091f65c535d504d9f9932
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761424"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="a664f-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a664f-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="a664f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a664f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a664f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a664f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a664f-106">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a664f-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a664f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a664f-107">Prerequisites</span></span>
<span data-ttu-id="a664f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a664f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a664f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a664f-110">Permission type</span></span>|<span data-ttu-id="a664f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a664f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a664f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a664f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a664f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a664f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a664f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a664f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a664f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a664f-115">Not supported.</span></span>|
|<span data-ttu-id="a664f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a664f-116">Application</span></span>|<span data-ttu-id="a664f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a664f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a664f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a664f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a664f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a664f-119">Request headers</span></span>
|<span data-ttu-id="a664f-120">标头</span><span class="sxs-lookup"><span data-stu-id="a664f-120">Header</span></span>|<span data-ttu-id="a664f-121">值</span><span class="sxs-lookup"><span data-stu-id="a664f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a664f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a664f-122">Authorization</span></span>|<span data-ttu-id="a664f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a664f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a664f-124">接受</span><span class="sxs-lookup"><span data-stu-id="a664f-124">Accept</span></span>|<span data-ttu-id="a664f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a664f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a664f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a664f-126">Request body</span></span>
<span data-ttu-id="a664f-127">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a664f-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="a664f-128">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a664f-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="a664f-129">属性</span><span class="sxs-lookup"><span data-stu-id="a664f-129">Property</span></span>|<span data-ttu-id="a664f-130">类型</span><span class="sxs-lookup"><span data-stu-id="a664f-130">Type</span></span>|<span data-ttu-id="a664f-131">说明</span><span class="sxs-lookup"><span data-stu-id="a664f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a664f-132">id</span><span class="sxs-lookup"><span data-stu-id="a664f-132">id</span></span>|<span data-ttu-id="a664f-133">String</span><span class="sxs-lookup"><span data-stu-id="a664f-133">String</span></span>|<span data-ttu-id="a664f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a664f-134">Key of the entity.</span></span>|
|<span data-ttu-id="a664f-135">intent</span><span class="sxs-lookup"><span data-stu-id="a664f-135">intent</span></span>|[<span data-ttu-id="a664f-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="a664f-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a664f-137">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="a664f-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="a664f-138">target</span><span class="sxs-lookup"><span data-stu-id="a664f-138">target</span></span>|[<span data-ttu-id="a664f-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a664f-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a664f-140">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="a664f-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="a664f-141">settings</span><span class="sxs-lookup"><span data-stu-id="a664f-141">settings</span></span>|[<span data-ttu-id="a664f-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a664f-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="a664f-143">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="a664f-143">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="a664f-144">source</span><span class="sxs-lookup"><span data-stu-id="a664f-144">source</span></span>|[<span data-ttu-id="a664f-145">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a664f-145">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a664f-146">资源类型，它是工作分配的源。</span><span class="sxs-lookup"><span data-stu-id="a664f-146">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="a664f-147">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="a664f-147">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a664f-148">sourceId</span><span class="sxs-lookup"><span data-stu-id="a664f-148">sourceId</span></span>|<span data-ttu-id="a664f-149">String</span><span class="sxs-lookup"><span data-stu-id="a664f-149">String</span></span>|<span data-ttu-id="a664f-150">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="a664f-150">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="a664f-151">响应</span><span class="sxs-lookup"><span data-stu-id="a664f-151">Response</span></span>
<span data-ttu-id="a664f-152">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a664f-152">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a664f-153">示例</span><span class="sxs-lookup"><span data-stu-id="a664f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a664f-154">请求</span><span class="sxs-lookup"><span data-stu-id="a664f-154">Request</span></span>
<span data-ttu-id="a664f-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a664f-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="a664f-156">响应</span><span class="sxs-lookup"><span data-stu-id="a664f-156">Response</span></span>
<span data-ttu-id="a664f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a664f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




