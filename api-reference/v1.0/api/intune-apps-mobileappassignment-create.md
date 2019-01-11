---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b882c12de0be358d1a08611037662f3cd9246a43
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876207"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="7d54c-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="7d54c-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="7d54c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d54c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d54c-105">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d54c-105">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d54c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7d54c-106">Prerequisites</span></span>
<span data-ttu-id="7d54c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7d54c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d54c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d54c-109">Permission type</span></span>|<span data-ttu-id="7d54c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7d54c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d54c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d54c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d54c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d54c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d54c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d54c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d54c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d54c-114">Not supported.</span></span>|
|<span data-ttu-id="7d54c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d54c-115">Application</span></span>|<span data-ttu-id="7d54c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d54c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d54c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d54c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7d54c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d54c-118">Request headers</span></span>
|<span data-ttu-id="7d54c-119">标头</span><span class="sxs-lookup"><span data-stu-id="7d54c-119">Header</span></span>|<span data-ttu-id="7d54c-120">值</span><span class="sxs-lookup"><span data-stu-id="7d54c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d54c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d54c-121">Authorization</span></span>|<span data-ttu-id="7d54c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7d54c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d54c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7d54c-123">Accept</span></span>|<span data-ttu-id="7d54c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d54c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d54c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d54c-125">Request body</span></span>
<span data-ttu-id="7d54c-126">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d54c-126">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="7d54c-127">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7d54c-127">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="7d54c-128">属性</span><span class="sxs-lookup"><span data-stu-id="7d54c-128">Property</span></span>|<span data-ttu-id="7d54c-129">类型</span><span class="sxs-lookup"><span data-stu-id="7d54c-129">Type</span></span>|<span data-ttu-id="7d54c-130">说明</span><span class="sxs-lookup"><span data-stu-id="7d54c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d54c-131">id</span><span class="sxs-lookup"><span data-stu-id="7d54c-131">id</span></span>|<span data-ttu-id="7d54c-132">String</span><span class="sxs-lookup"><span data-stu-id="7d54c-132">String</span></span>|<span data-ttu-id="7d54c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7d54c-133">Key of the entity.</span></span>|
|<span data-ttu-id="7d54c-134">intent</span><span class="sxs-lookup"><span data-stu-id="7d54c-134">intent</span></span>|[<span data-ttu-id="7d54c-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="7d54c-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7d54c-136">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="7d54c-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="7d54c-137">target</span><span class="sxs-lookup"><span data-stu-id="7d54c-137">target</span></span>|[<span data-ttu-id="7d54c-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7d54c-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7d54c-139">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="7d54c-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="7d54c-140">settings</span><span class="sxs-lookup"><span data-stu-id="7d54c-140">settings</span></span>|[<span data-ttu-id="7d54c-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7d54c-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="7d54c-142">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="7d54c-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="7d54c-143">响应</span><span class="sxs-lookup"><span data-stu-id="7d54c-143">Response</span></span>
<span data-ttu-id="7d54c-144">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d54c-144">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d54c-145">示例</span><span class="sxs-lookup"><span data-stu-id="7d54c-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d54c-146">请求</span><span class="sxs-lookup"><span data-stu-id="7d54c-146">Request</span></span>
<span data-ttu-id="7d54c-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d54c-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d54c-148">响应</span><span class="sxs-lookup"><span data-stu-id="7d54c-148">Response</span></span>
<span data-ttu-id="7d54c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7d54c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



