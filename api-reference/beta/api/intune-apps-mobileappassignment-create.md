---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 94fb6e79077e687df11cda4b28b71b8e97360971
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397979"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="0b8b9-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="0b8b9-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="0b8b9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b8b9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b8b9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b8b9-107">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b8b9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b8b9-108">Prerequisites</span></span>
<span data-ttu-id="0b8b9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b8b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b8b9-111">Permission type</span></span>|<span data-ttu-id="0b8b9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b8b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b8b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b8b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b8b9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8b9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b8b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b8b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b8b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-116">Not supported.</span></span>|
|<span data-ttu-id="0b8b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b8b9-117">Application</span></span>|<span data-ttu-id="0b8b9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b8b9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b8b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0b8b9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b8b9-120">Request headers</span></span>
|<span data-ttu-id="0b8b9-121">标头</span><span class="sxs-lookup"><span data-stu-id="0b8b9-121">Header</span></span>|<span data-ttu-id="0b8b9-122">值</span><span class="sxs-lookup"><span data-stu-id="0b8b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b8b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b8b9-123">Authorization</span></span>|<span data-ttu-id="0b8b9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b8b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b8b9-125">Accept</span></span>|<span data-ttu-id="0b8b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b8b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b8b9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b8b9-127">Request body</span></span>
<span data-ttu-id="0b8b9-128">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="0b8b9-129">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="0b8b9-130">属性</span><span class="sxs-lookup"><span data-stu-id="0b8b9-130">Property</span></span>|<span data-ttu-id="0b8b9-131">类型</span><span class="sxs-lookup"><span data-stu-id="0b8b9-131">Type</span></span>|<span data-ttu-id="0b8b9-132">说明</span><span class="sxs-lookup"><span data-stu-id="0b8b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b8b9-133">id</span><span class="sxs-lookup"><span data-stu-id="0b8b9-133">id</span></span>|<span data-ttu-id="0b8b9-134">String</span><span class="sxs-lookup"><span data-stu-id="0b8b9-134">String</span></span>|<span data-ttu-id="0b8b9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-135">Key of the entity.</span></span>|
|<span data-ttu-id="0b8b9-136">intent</span><span class="sxs-lookup"><span data-stu-id="0b8b9-136">intent</span></span>|[<span data-ttu-id="0b8b9-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="0b8b9-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="0b8b9-138">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="0b8b9-139">target</span><span class="sxs-lookup"><span data-stu-id="0b8b9-139">target</span></span>|[<span data-ttu-id="0b8b9-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0b8b9-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0b8b9-141">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="0b8b9-142">settings</span><span class="sxs-lookup"><span data-stu-id="0b8b9-142">settings</span></span>|[<span data-ttu-id="0b8b9-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="0b8b9-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="0b8b9-144">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="0b8b9-145">响应</span><span class="sxs-lookup"><span data-stu-id="0b8b9-145">Response</span></span>
<span data-ttu-id="0b8b9-146">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b8b9-147">示例</span><span class="sxs-lookup"><span data-stu-id="0b8b9-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b8b9-148">请求</span><span class="sxs-lookup"><span data-stu-id="0b8b9-148">Request</span></span>
<span data-ttu-id="0b8b9-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b8b9-150">响应</span><span class="sxs-lookup"><span data-stu-id="0b8b9-150">Response</span></span>
<span data-ttu-id="0b8b9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b8b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




