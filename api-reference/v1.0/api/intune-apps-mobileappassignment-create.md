---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e2eea5bd9caa01430daa5e85a3fe7483d4e40aa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759740"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="76b0b-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="76b0b-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="76b0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76b0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76b0b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76b0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76b0b-106">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76b0b-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76b0b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="76b0b-107">Prerequisites</span></span>
<span data-ttu-id="76b0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76b0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76b0b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="76b0b-110">Permission type</span></span>|<span data-ttu-id="76b0b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76b0b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76b0b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76b0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76b0b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b0b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76b0b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76b0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76b0b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="76b0b-115">Not supported.</span></span>|
|<span data-ttu-id="76b0b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="76b0b-116">Application</span></span>|<span data-ttu-id="76b0b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b0b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76b0b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76b0b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="76b0b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="76b0b-119">Request headers</span></span>
|<span data-ttu-id="76b0b-120">标头</span><span class="sxs-lookup"><span data-stu-id="76b0b-120">Header</span></span>|<span data-ttu-id="76b0b-121">值</span><span class="sxs-lookup"><span data-stu-id="76b0b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76b0b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76b0b-122">Authorization</span></span>|<span data-ttu-id="76b0b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76b0b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76b0b-124">接受</span><span class="sxs-lookup"><span data-stu-id="76b0b-124">Accept</span></span>|<span data-ttu-id="76b0b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76b0b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76b0b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="76b0b-126">Request body</span></span>
<span data-ttu-id="76b0b-127">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76b0b-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="76b0b-128">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="76b0b-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="76b0b-129">属性</span><span class="sxs-lookup"><span data-stu-id="76b0b-129">Property</span></span>|<span data-ttu-id="76b0b-130">类型</span><span class="sxs-lookup"><span data-stu-id="76b0b-130">Type</span></span>|<span data-ttu-id="76b0b-131">说明</span><span class="sxs-lookup"><span data-stu-id="76b0b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b0b-132">id</span><span class="sxs-lookup"><span data-stu-id="76b0b-132">id</span></span>|<span data-ttu-id="76b0b-133">String</span><span class="sxs-lookup"><span data-stu-id="76b0b-133">String</span></span>|<span data-ttu-id="76b0b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="76b0b-134">Key of the entity.</span></span>|
|<span data-ttu-id="76b0b-135">intent</span><span class="sxs-lookup"><span data-stu-id="76b0b-135">intent</span></span>|[<span data-ttu-id="76b0b-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="76b0b-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="76b0b-137">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="76b0b-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="76b0b-138">target</span><span class="sxs-lookup"><span data-stu-id="76b0b-138">target</span></span>|[<span data-ttu-id="76b0b-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="76b0b-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="76b0b-140">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="76b0b-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="76b0b-141">settings</span><span class="sxs-lookup"><span data-stu-id="76b0b-141">settings</span></span>|[<span data-ttu-id="76b0b-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="76b0b-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="76b0b-143">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="76b0b-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="76b0b-144">响应</span><span class="sxs-lookup"><span data-stu-id="76b0b-144">Response</span></span>
<span data-ttu-id="76b0b-145">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76b0b-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76b0b-146">示例</span><span class="sxs-lookup"><span data-stu-id="76b0b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="76b0b-147">请求</span><span class="sxs-lookup"><span data-stu-id="76b0b-147">Request</span></span>
<span data-ttu-id="76b0b-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76b0b-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="76b0b-149">响应</span><span class="sxs-lookup"><span data-stu-id="76b0b-149">Response</span></span>
<span data-ttu-id="76b0b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76b0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 373

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value"
  }
}
```




