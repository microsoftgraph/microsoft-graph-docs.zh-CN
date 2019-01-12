---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d935f5a14453dd752601af3f773b9f298425caf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980830"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="05e77-103">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="05e77-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="05e77-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="05e77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05e77-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="05e77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05e77-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="05e77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05e77-107">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05e77-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05e77-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="05e77-108">Prerequisites</span></span>
<span data-ttu-id="05e77-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="05e77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05e77-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="05e77-111">Permission type</span></span>|<span data-ttu-id="05e77-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05e77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05e77-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05e77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05e77-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05e77-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05e77-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05e77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05e77-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05e77-116">Not supported.</span></span>|
|<span data-ttu-id="05e77-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="05e77-117">Application</span></span>|<span data-ttu-id="05e77-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="05e77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05e77-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05e77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="05e77-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05e77-120">Request headers</span></span>
|<span data-ttu-id="05e77-121">标头</span><span class="sxs-lookup"><span data-stu-id="05e77-121">Header</span></span>|<span data-ttu-id="05e77-122">值</span><span class="sxs-lookup"><span data-stu-id="05e77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05e77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05e77-123">Authorization</span></span>|<span data-ttu-id="05e77-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05e77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05e77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05e77-125">Accept</span></span>|<span data-ttu-id="05e77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05e77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05e77-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05e77-127">Request body</span></span>
<span data-ttu-id="05e77-128">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05e77-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="05e77-129">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="05e77-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="05e77-130">属性</span><span class="sxs-lookup"><span data-stu-id="05e77-130">Property</span></span>|<span data-ttu-id="05e77-131">类型</span><span class="sxs-lookup"><span data-stu-id="05e77-131">Type</span></span>|<span data-ttu-id="05e77-132">说明</span><span class="sxs-lookup"><span data-stu-id="05e77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05e77-133">id</span><span class="sxs-lookup"><span data-stu-id="05e77-133">id</span></span>|<span data-ttu-id="05e77-134">String</span><span class="sxs-lookup"><span data-stu-id="05e77-134">String</span></span>|<span data-ttu-id="05e77-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="05e77-135">Key of the entity.</span></span>|
|<span data-ttu-id="05e77-136">intent</span><span class="sxs-lookup"><span data-stu-id="05e77-136">intent</span></span>|[<span data-ttu-id="05e77-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="05e77-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="05e77-138">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="05e77-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="05e77-139">target</span><span class="sxs-lookup"><span data-stu-id="05e77-139">target</span></span>|[<span data-ttu-id="05e77-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="05e77-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="05e77-141">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="05e77-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="05e77-142">settings</span><span class="sxs-lookup"><span data-stu-id="05e77-142">settings</span></span>|[<span data-ttu-id="05e77-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="05e77-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="05e77-144">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="05e77-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="05e77-145">响应</span><span class="sxs-lookup"><span data-stu-id="05e77-145">Response</span></span>
<span data-ttu-id="05e77-146">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05e77-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05e77-147">示例</span><span class="sxs-lookup"><span data-stu-id="05e77-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="05e77-148">请求</span><span class="sxs-lookup"><span data-stu-id="05e77-148">Request</span></span>
<span data-ttu-id="05e77-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05e77-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05e77-150">响应</span><span class="sxs-lookup"><span data-stu-id="05e77-150">Response</span></span>
<span data-ttu-id="05e77-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05e77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





