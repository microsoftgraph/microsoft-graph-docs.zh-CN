---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bddcba906fe40becc9e3c32a4a2e31dc7277bba
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358345"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="3b7bc-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="3b7bc-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="3b7bc-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b7bc-105">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-105">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b7bc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b7bc-106">Prerequisites</span></span>
<span data-ttu-id="3b7bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b7bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b7bc-109">Permission type</span></span>|<span data-ttu-id="3b7bc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3b7bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b7bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b7bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b7bc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b7bc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b7bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b7bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b7bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-114">Not supported.</span></span>|
|<span data-ttu-id="3b7bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b7bc-115">Application</span></span>|<span data-ttu-id="3b7bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b7bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b7bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3b7bc-118">请求头</span><span class="sxs-lookup"><span data-stu-id="3b7bc-118">Request headers</span></span>
|<span data-ttu-id="3b7bc-119">标头</span><span class="sxs-lookup"><span data-stu-id="3b7bc-119">Header</span></span>|<span data-ttu-id="3b7bc-120">值</span><span class="sxs-lookup"><span data-stu-id="3b7bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b7bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b7bc-121">Authorization</span></span>|<span data-ttu-id="3b7bc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b7bc-123">接受</span><span class="sxs-lookup"><span data-stu-id="3b7bc-123">Accept</span></span>|<span data-ttu-id="3b7bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b7bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b7bc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b7bc-125">Request body</span></span>
<span data-ttu-id="3b7bc-126">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-126">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="3b7bc-127">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-127">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="3b7bc-128">属性</span><span class="sxs-lookup"><span data-stu-id="3b7bc-128">Property</span></span>|<span data-ttu-id="3b7bc-129">类型</span><span class="sxs-lookup"><span data-stu-id="3b7bc-129">Type</span></span>|<span data-ttu-id="3b7bc-130">说明</span><span class="sxs-lookup"><span data-stu-id="3b7bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b7bc-131">id</span><span class="sxs-lookup"><span data-stu-id="3b7bc-131">id</span></span>|<span data-ttu-id="3b7bc-132">String</span><span class="sxs-lookup"><span data-stu-id="3b7bc-132">String</span></span>|<span data-ttu-id="3b7bc-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-133">Key of the entity.</span></span>|
|<span data-ttu-id="3b7bc-134">intent</span><span class="sxs-lookup"><span data-stu-id="3b7bc-134">intent</span></span>|[<span data-ttu-id="3b7bc-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="3b7bc-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="3b7bc-136">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="3b7bc-137">target</span><span class="sxs-lookup"><span data-stu-id="3b7bc-137">target</span></span>|[<span data-ttu-id="3b7bc-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3b7bc-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3b7bc-139">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="3b7bc-140">settings</span><span class="sxs-lookup"><span data-stu-id="3b7bc-140">settings</span></span>|[<span data-ttu-id="3b7bc-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3b7bc-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="3b7bc-142">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="3b7bc-143">响应</span><span class="sxs-lookup"><span data-stu-id="3b7bc-143">Response</span></span>
<span data-ttu-id="3b7bc-144">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-144">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b7bc-145">示例</span><span class="sxs-lookup"><span data-stu-id="3b7bc-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b7bc-146">请求</span><span class="sxs-lookup"><span data-stu-id="3b7bc-146">Request</span></span>
<span data-ttu-id="3b7bc-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="3b7bc-148">响应</span><span class="sxs-lookup"><span data-stu-id="3b7bc-148">Response</span></span>
<span data-ttu-id="3b7bc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b7bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




