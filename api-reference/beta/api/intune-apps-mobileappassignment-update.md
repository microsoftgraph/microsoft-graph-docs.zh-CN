---
title: 更新 mobileAppAssignment
description: 更新 mobileAppAssignment 对象的属性。
ms.openlocfilehash: 218197991a6bc1c7d80053159efd11d138052298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041627"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="fa9ac-103">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="fa9ac-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="fa9ac-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa9ac-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa9ac-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa9ac-107">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa9ac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa9ac-108">Prerequisites</span></span>
<span data-ttu-id="fa9ac-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fa9ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa9ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa9ac-111">Permission type</span></span>|<span data-ttu-id="fa9ac-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa9ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa9ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa9ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa9ac-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa9ac-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa9ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa9ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa9ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-116">Not supported.</span></span>|
|<span data-ttu-id="fa9ac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa9ac-117">Application</span></span>|<span data-ttu-id="fa9ac-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa9ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa9ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fa9ac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa9ac-120">Request headers</span></span>
|<span data-ttu-id="fa9ac-121">标头</span><span class="sxs-lookup"><span data-stu-id="fa9ac-121">Header</span></span>|<span data-ttu-id="fa9ac-122">值</span><span class="sxs-lookup"><span data-stu-id="fa9ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa9ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa9ac-123">Authorization</span></span>|<span data-ttu-id="fa9ac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa9ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa9ac-125">Accept</span></span>|<span data-ttu-id="fa9ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa9ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa9ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa9ac-127">Request body</span></span>
<span data-ttu-id="fa9ac-128">在请求正文中，提供 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="fa9ac-129">下表显示创建 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="fa9ac-130">属性</span><span class="sxs-lookup"><span data-stu-id="fa9ac-130">Property</span></span>|<span data-ttu-id="fa9ac-131">类型</span><span class="sxs-lookup"><span data-stu-id="fa9ac-131">Type</span></span>|<span data-ttu-id="fa9ac-132">说明</span><span class="sxs-lookup"><span data-stu-id="fa9ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa9ac-133">id</span><span class="sxs-lookup"><span data-stu-id="fa9ac-133">id</span></span>|<span data-ttu-id="fa9ac-134">String</span><span class="sxs-lookup"><span data-stu-id="fa9ac-134">String</span></span>|<span data-ttu-id="fa9ac-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-135">Key of the entity.</span></span>|
|<span data-ttu-id="fa9ac-136">intent</span><span class="sxs-lookup"><span data-stu-id="fa9ac-136">intent</span></span>|[<span data-ttu-id="fa9ac-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="fa9ac-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="fa9ac-138">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="fa9ac-139">target</span><span class="sxs-lookup"><span data-stu-id="fa9ac-139">target</span></span>|[<span data-ttu-id="fa9ac-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fa9ac-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fa9ac-141">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="fa9ac-142">settings</span><span class="sxs-lookup"><span data-stu-id="fa9ac-142">settings</span></span>|[<span data-ttu-id="fa9ac-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="fa9ac-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="fa9ac-144">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="fa9ac-145">响应</span><span class="sxs-lookup"><span data-stu-id="fa9ac-145">Response</span></span>
<span data-ttu-id="fa9ac-146">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa9ac-147">示例</span><span class="sxs-lookup"><span data-stu-id="fa9ac-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa9ac-148">请求</span><span class="sxs-lookup"><span data-stu-id="fa9ac-148">Request</span></span>
<span data-ttu-id="fa9ac-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 215

{
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="fa9ac-150">响应</span><span class="sxs-lookup"><span data-stu-id="fa9ac-150">Response</span></span>
<span data-ttu-id="fa9ac-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa9ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





