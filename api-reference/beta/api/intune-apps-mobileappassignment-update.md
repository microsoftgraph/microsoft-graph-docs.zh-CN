---
title: 更新 mobileAppAssignment
description: 更新 mobileAppAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bbedecc237e56022351fef82853fc3c2cb14bb91
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424320"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="f7b61-103">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b61-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="f7b61-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f7b61-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7b61-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f7b61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7b61-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7b61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7b61-107">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f7b61-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7b61-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7b61-108">Prerequisites</span></span>
<span data-ttu-id="f7b61-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f7b61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f7b61-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7b61-111">Permission type</span></span>|<span data-ttu-id="f7b61-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7b61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7b61-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7b61-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7b61-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7b61-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7b61-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b61-116">Not supported.</span></span>|
|<span data-ttu-id="f7b61-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7b61-117">Application</span></span>|<span data-ttu-id="f7b61-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b61-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7b61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7b61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f7b61-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7b61-120">Request headers</span></span>
|<span data-ttu-id="f7b61-121">标头</span><span class="sxs-lookup"><span data-stu-id="f7b61-121">Header</span></span>|<span data-ttu-id="f7b61-122">值</span><span class="sxs-lookup"><span data-stu-id="f7b61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7b61-123">授权</span><span class="sxs-lookup"><span data-stu-id="f7b61-123">Authorization</span></span>|<span data-ttu-id="f7b61-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7b61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7b61-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7b61-125">Accept</span></span>|<span data-ttu-id="f7b61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7b61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7b61-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7b61-127">Request body</span></span>
<span data-ttu-id="f7b61-128">在请求正文中，提供 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7b61-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="f7b61-129">下表显示创建 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f7b61-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="f7b61-130">属性</span><span class="sxs-lookup"><span data-stu-id="f7b61-130">Property</span></span>|<span data-ttu-id="f7b61-131">类型</span><span class="sxs-lookup"><span data-stu-id="f7b61-131">Type</span></span>|<span data-ttu-id="f7b61-132">说明</span><span class="sxs-lookup"><span data-stu-id="f7b61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7b61-133">id</span><span class="sxs-lookup"><span data-stu-id="f7b61-133">id</span></span>|<span data-ttu-id="f7b61-134">String</span><span class="sxs-lookup"><span data-stu-id="f7b61-134">String</span></span>|<span data-ttu-id="f7b61-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f7b61-135">Key of the entity.</span></span>|
|<span data-ttu-id="f7b61-136">intent</span><span class="sxs-lookup"><span data-stu-id="f7b61-136">intent</span></span>|[<span data-ttu-id="f7b61-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="f7b61-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="f7b61-138">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="f7b61-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="f7b61-139">target</span><span class="sxs-lookup"><span data-stu-id="f7b61-139">target</span></span>|[<span data-ttu-id="f7b61-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f7b61-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f7b61-141">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="f7b61-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="f7b61-142">settings</span><span class="sxs-lookup"><span data-stu-id="f7b61-142">settings</span></span>|[<span data-ttu-id="f7b61-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f7b61-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="f7b61-144">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="f7b61-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="f7b61-145">响应</span><span class="sxs-lookup"><span data-stu-id="f7b61-145">Response</span></span>
<span data-ttu-id="f7b61-146">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7b61-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7b61-147">示例</span><span class="sxs-lookup"><span data-stu-id="f7b61-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7b61-148">请求</span><span class="sxs-lookup"><span data-stu-id="f7b61-148">Request</span></span>
<span data-ttu-id="f7b61-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7b61-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
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

### <a name="response"></a><span data-ttu-id="f7b61-150">响应</span><span class="sxs-lookup"><span data-stu-id="f7b61-150">Response</span></span>
<span data-ttu-id="f7b61-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7b61-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




