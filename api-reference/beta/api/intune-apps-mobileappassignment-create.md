---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c37ebcb4aa5506f1be2119afef9a0f61a4da9d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329332"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="e8399-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="e8399-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="e8399-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8399-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8399-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8399-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8399-106">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8399-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8399-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8399-107">Prerequisites</span></span>
<span data-ttu-id="e8399-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8399-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8399-110">Permission type</span></span>|<span data-ttu-id="e8399-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8399-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8399-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8399-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8399-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8399-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e8399-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8399-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8399-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8399-115">Not supported.</span></span>|
|<span data-ttu-id="e8399-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8399-116">Application</span></span>|<span data-ttu-id="e8399-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8399-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8399-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8399-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e8399-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8399-119">Request headers</span></span>
|<span data-ttu-id="e8399-120">标头</span><span class="sxs-lookup"><span data-stu-id="e8399-120">Header</span></span>|<span data-ttu-id="e8399-121">值</span><span class="sxs-lookup"><span data-stu-id="e8399-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8399-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8399-122">Authorization</span></span>|<span data-ttu-id="e8399-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8399-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8399-124">接受</span><span class="sxs-lookup"><span data-stu-id="e8399-124">Accept</span></span>|<span data-ttu-id="e8399-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8399-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8399-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8399-126">Request body</span></span>
<span data-ttu-id="e8399-127">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8399-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="e8399-128">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e8399-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="e8399-129">属性</span><span class="sxs-lookup"><span data-stu-id="e8399-129">Property</span></span>|<span data-ttu-id="e8399-130">类型</span><span class="sxs-lookup"><span data-stu-id="e8399-130">Type</span></span>|<span data-ttu-id="e8399-131">说明</span><span class="sxs-lookup"><span data-stu-id="e8399-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8399-132">id</span><span class="sxs-lookup"><span data-stu-id="e8399-132">id</span></span>|<span data-ttu-id="e8399-133">String</span><span class="sxs-lookup"><span data-stu-id="e8399-133">String</span></span>|<span data-ttu-id="e8399-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e8399-134">Key of the entity.</span></span>|
|<span data-ttu-id="e8399-135">intent</span><span class="sxs-lookup"><span data-stu-id="e8399-135">intent</span></span>|[<span data-ttu-id="e8399-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="e8399-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="e8399-137">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="e8399-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="e8399-138">target</span><span class="sxs-lookup"><span data-stu-id="e8399-138">target</span></span>|[<span data-ttu-id="e8399-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e8399-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e8399-140">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="e8399-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="e8399-141">settings</span><span class="sxs-lookup"><span data-stu-id="e8399-141">settings</span></span>|[<span data-ttu-id="e8399-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e8399-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="e8399-143">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="e8399-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="e8399-144">响应</span><span class="sxs-lookup"><span data-stu-id="e8399-144">Response</span></span>
<span data-ttu-id="e8399-145">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8399-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8399-146">示例</span><span class="sxs-lookup"><span data-stu-id="e8399-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8399-147">请求</span><span class="sxs-lookup"><span data-stu-id="e8399-147">Request</span></span>
<span data-ttu-id="e8399-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8399-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8399-149">响应</span><span class="sxs-lookup"><span data-stu-id="e8399-149">Response</span></span>
<span data-ttu-id="e8399-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8399-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






