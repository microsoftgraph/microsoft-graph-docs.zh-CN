---
title: 更新 mobileAppAssignment
description: 更新 mobileAppAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14ee6a186a94a6c050250bd930e78e7f9e38bb3e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964547"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="f7087-103">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="f7087-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="f7087-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7087-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7087-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7087-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7087-106">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f7087-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7087-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7087-107">Prerequisites</span></span>
<span data-ttu-id="f7087-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7087-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7087-110">Permission type</span></span>|<span data-ttu-id="f7087-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7087-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7087-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7087-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7087-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7087-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7087-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7087-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7087-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7087-115">Not supported.</span></span>|
|<span data-ttu-id="f7087-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7087-116">Application</span></span>|<span data-ttu-id="f7087-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7087-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7087-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7087-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f7087-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7087-119">Request headers</span></span>
|<span data-ttu-id="f7087-120">标头</span><span class="sxs-lookup"><span data-stu-id="f7087-120">Header</span></span>|<span data-ttu-id="f7087-121">值</span><span class="sxs-lookup"><span data-stu-id="f7087-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7087-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7087-122">Authorization</span></span>|<span data-ttu-id="f7087-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7087-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7087-124">接受</span><span class="sxs-lookup"><span data-stu-id="f7087-124">Accept</span></span>|<span data-ttu-id="f7087-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7087-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7087-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7087-126">Request body</span></span>
<span data-ttu-id="f7087-127">在请求正文中，提供 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7087-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="f7087-128">下表显示创建 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f7087-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="f7087-129">属性</span><span class="sxs-lookup"><span data-stu-id="f7087-129">Property</span></span>|<span data-ttu-id="f7087-130">类型</span><span class="sxs-lookup"><span data-stu-id="f7087-130">Type</span></span>|<span data-ttu-id="f7087-131">说明</span><span class="sxs-lookup"><span data-stu-id="f7087-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7087-132">id</span><span class="sxs-lookup"><span data-stu-id="f7087-132">id</span></span>|<span data-ttu-id="f7087-133">String</span><span class="sxs-lookup"><span data-stu-id="f7087-133">String</span></span>|<span data-ttu-id="f7087-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f7087-134">Key of the entity.</span></span>|
|<span data-ttu-id="f7087-135">intent</span><span class="sxs-lookup"><span data-stu-id="f7087-135">intent</span></span>|[<span data-ttu-id="f7087-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="f7087-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="f7087-137">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="f7087-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="f7087-138">target</span><span class="sxs-lookup"><span data-stu-id="f7087-138">target</span></span>|[<span data-ttu-id="f7087-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f7087-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f7087-140">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="f7087-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="f7087-141">settings</span><span class="sxs-lookup"><span data-stu-id="f7087-141">settings</span></span>|[<span data-ttu-id="f7087-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f7087-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="f7087-143">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="f7087-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="f7087-144">响应</span><span class="sxs-lookup"><span data-stu-id="f7087-144">Response</span></span>
<span data-ttu-id="f7087-145">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7087-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7087-146">示例</span><span class="sxs-lookup"><span data-stu-id="f7087-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7087-147">请求</span><span class="sxs-lookup"><span data-stu-id="f7087-147">Request</span></span>
<span data-ttu-id="f7087-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7087-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7087-149">响应</span><span class="sxs-lookup"><span data-stu-id="f7087-149">Response</span></span>
<span data-ttu-id="f7087-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7087-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




