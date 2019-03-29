---
title: 更新 mobileAppAssignment
description: 更新 mobileAppAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 647a5a4bb7a89b0b44ce650c411b95c5c20c162c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977644"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="30a68-103">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="30a68-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="30a68-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="30a68-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30a68-105">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30a68-105">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30a68-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="30a68-106">Prerequisites</span></span>
<span data-ttu-id="30a68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30a68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a68-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="30a68-109">Permission type</span></span>|<span data-ttu-id="30a68-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="30a68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30a68-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30a68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30a68-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a68-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30a68-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30a68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30a68-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="30a68-114">Not supported.</span></span>|
|<span data-ttu-id="30a68-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="30a68-115">Application</span></span>|<span data-ttu-id="30a68-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30a68-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30a68-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30a68-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="30a68-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="30a68-118">Request headers</span></span>
|<span data-ttu-id="30a68-119">标头</span><span class="sxs-lookup"><span data-stu-id="30a68-119">Header</span></span>|<span data-ttu-id="30a68-120">值</span><span class="sxs-lookup"><span data-stu-id="30a68-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30a68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="30a68-121">Authorization</span></span>|<span data-ttu-id="30a68-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="30a68-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30a68-123">接受</span><span class="sxs-lookup"><span data-stu-id="30a68-123">Accept</span></span>|<span data-ttu-id="30a68-124">application/json</span><span class="sxs-lookup"><span data-stu-id="30a68-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30a68-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="30a68-125">Request body</span></span>
<span data-ttu-id="30a68-126">在请求正文中，提供 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30a68-126">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="30a68-127">下表显示创建 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="30a68-127">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="30a68-128">属性</span><span class="sxs-lookup"><span data-stu-id="30a68-128">Property</span></span>|<span data-ttu-id="30a68-129">类型</span><span class="sxs-lookup"><span data-stu-id="30a68-129">Type</span></span>|<span data-ttu-id="30a68-130">说明</span><span class="sxs-lookup"><span data-stu-id="30a68-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30a68-131">id</span><span class="sxs-lookup"><span data-stu-id="30a68-131">id</span></span>|<span data-ttu-id="30a68-132">String</span><span class="sxs-lookup"><span data-stu-id="30a68-132">String</span></span>|<span data-ttu-id="30a68-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="30a68-133">Key of the entity.</span></span>|
|<span data-ttu-id="30a68-134">intent</span><span class="sxs-lookup"><span data-stu-id="30a68-134">intent</span></span>|[<span data-ttu-id="30a68-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="30a68-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="30a68-136">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="30a68-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="30a68-137">target</span><span class="sxs-lookup"><span data-stu-id="30a68-137">target</span></span>|[<span data-ttu-id="30a68-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="30a68-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="30a68-139">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="30a68-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="30a68-140">settings</span><span class="sxs-lookup"><span data-stu-id="30a68-140">settings</span></span>|[<span data-ttu-id="30a68-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="30a68-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="30a68-142">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="30a68-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="30a68-143">响应</span><span class="sxs-lookup"><span data-stu-id="30a68-143">Response</span></span>
<span data-ttu-id="30a68-144">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30a68-144">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30a68-145">示例</span><span class="sxs-lookup"><span data-stu-id="30a68-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="30a68-146">请求</span><span class="sxs-lookup"><span data-stu-id="30a68-146">Request</span></span>
<span data-ttu-id="30a68-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30a68-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30a68-148">响应</span><span class="sxs-lookup"><span data-stu-id="30a68-148">Response</span></span>
<span data-ttu-id="30a68-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30a68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



