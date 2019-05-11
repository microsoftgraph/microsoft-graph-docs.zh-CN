---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 097bc7cf01c243056711436a84eb0d56f2889f05
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935331"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="7fe9c-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="7fe9c-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="7fe9c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fe9c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fe9c-106">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fe9c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7fe9c-107">Prerequisites</span></span>
<span data-ttu-id="7fe9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe9c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fe9c-110">Permission type</span></span>|<span data-ttu-id="7fe9c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7fe9c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe9c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe9c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe9c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7fe9c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe9c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-115">Not supported.</span></span>|
|<span data-ttu-id="7fe9c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fe9c-116">Application</span></span>|<span data-ttu-id="7fe9c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe9c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fe9c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7fe9c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fe9c-119">Request headers</span></span>
|<span data-ttu-id="7fe9c-120">标头</span><span class="sxs-lookup"><span data-stu-id="7fe9c-120">Header</span></span>|<span data-ttu-id="7fe9c-121">值</span><span class="sxs-lookup"><span data-stu-id="7fe9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fe9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fe9c-122">Authorization</span></span>|<span data-ttu-id="7fe9c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fe9c-124">接受</span><span class="sxs-lookup"><span data-stu-id="7fe9c-124">Accept</span></span>|<span data-ttu-id="7fe9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe9c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fe9c-126">Request body</span></span>
<span data-ttu-id="7fe9c-127">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="7fe9c-128">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="7fe9c-129">属性</span><span class="sxs-lookup"><span data-stu-id="7fe9c-129">Property</span></span>|<span data-ttu-id="7fe9c-130">类型</span><span class="sxs-lookup"><span data-stu-id="7fe9c-130">Type</span></span>|<span data-ttu-id="7fe9c-131">说明</span><span class="sxs-lookup"><span data-stu-id="7fe9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fe9c-132">id</span><span class="sxs-lookup"><span data-stu-id="7fe9c-132">id</span></span>|<span data-ttu-id="7fe9c-133">String</span><span class="sxs-lookup"><span data-stu-id="7fe9c-133">String</span></span>|<span data-ttu-id="7fe9c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-134">Key of the entity.</span></span>|
|<span data-ttu-id="7fe9c-135">intent</span><span class="sxs-lookup"><span data-stu-id="7fe9c-135">intent</span></span>|[<span data-ttu-id="7fe9c-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="7fe9c-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7fe9c-137">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="7fe9c-138">target</span><span class="sxs-lookup"><span data-stu-id="7fe9c-138">target</span></span>|[<span data-ttu-id="7fe9c-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7fe9c-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7fe9c-140">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="7fe9c-141">settings</span><span class="sxs-lookup"><span data-stu-id="7fe9c-141">settings</span></span>|[<span data-ttu-id="7fe9c-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7fe9c-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="7fe9c-143">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="7fe9c-144">响应</span><span class="sxs-lookup"><span data-stu-id="7fe9c-144">Response</span></span>
<span data-ttu-id="7fe9c-145">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe9c-146">示例</span><span class="sxs-lookup"><span data-stu-id="7fe9c-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fe9c-147">请求</span><span class="sxs-lookup"><span data-stu-id="7fe9c-147">Request</span></span>
<span data-ttu-id="7fe9c-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="7fe9c-149">响应</span><span class="sxs-lookup"><span data-stu-id="7fe9c-149">Response</span></span>
<span data-ttu-id="7fe9c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7fe9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




