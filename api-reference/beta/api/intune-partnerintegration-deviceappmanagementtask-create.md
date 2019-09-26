---
title: 创建 deviceAppManagementTask
description: 创建新的 deviceAppManagementTask 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee067956db1e078f05ce6bf3342dae648cad5bff
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189842"
---
# <a name="create-deviceappmanagementtask"></a><span data-ttu-id="b8b3d-103">创建 deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="b8b3d-103">Create deviceAppManagementTask</span></span>

> <span data-ttu-id="b8b3d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8b3d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8b3d-106">创建新的[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-106">Create a new [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8b3d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8b3d-107">Prerequisites</span></span>
<span data-ttu-id="b8b3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b3d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8b3d-110">Permission type</span></span>|<span data-ttu-id="b8b3d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8b3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8b3d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8b3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8b3d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8b3d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8b3d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8b3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8b3d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-115">Not supported.</span></span>|
|<span data-ttu-id="b8b3d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8b3d-116">Application</span></span>|<span data-ttu-id="b8b3d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8b3d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8b3d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8b3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="b8b3d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8b3d-119">Request headers</span></span>
|<span data-ttu-id="b8b3d-120">标头</span><span class="sxs-lookup"><span data-stu-id="b8b3d-120">Header</span></span>|<span data-ttu-id="b8b3d-121">值</span><span class="sxs-lookup"><span data-stu-id="b8b3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8b3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8b3d-122">Authorization</span></span>|<span data-ttu-id="b8b3d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8b3d-124">接受</span><span class="sxs-lookup"><span data-stu-id="b8b3d-124">Accept</span></span>|<span data-ttu-id="b8b3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8b3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8b3d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8b3d-126">Request body</span></span>
<span data-ttu-id="b8b3d-127">在请求正文中，提供 deviceAppManagementTask 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-127">In the request body, supply a JSON representation for the deviceAppManagementTask object.</span></span>

<span data-ttu-id="b8b3d-128">下表显示创建 deviceAppManagementTask 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-128">The following table shows the properties that are required when you create the deviceAppManagementTask.</span></span>

|<span data-ttu-id="b8b3d-129">属性</span><span class="sxs-lookup"><span data-stu-id="b8b3d-129">Property</span></span>|<span data-ttu-id="b8b3d-130">类型</span><span class="sxs-lookup"><span data-stu-id="b8b3d-130">Type</span></span>|<span data-ttu-id="b8b3d-131">说明</span><span class="sxs-lookup"><span data-stu-id="b8b3d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b3d-132">id</span><span class="sxs-lookup"><span data-stu-id="b8b3d-132">id</span></span>|<span data-ttu-id="b8b3d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b8b3d-133">String</span></span>|<span data-ttu-id="b8b3d-134">实体键。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-134">The entity key.</span></span>|
|<span data-ttu-id="b8b3d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b8b3d-135">displayName</span></span>|<span data-ttu-id="b8b3d-136">String</span><span class="sxs-lookup"><span data-stu-id="b8b3d-136">String</span></span>|<span data-ttu-id="b8b3d-137">名称。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-137">The name.</span></span>|
|<span data-ttu-id="b8b3d-138">说明</span><span class="sxs-lookup"><span data-stu-id="b8b3d-138">description</span></span>|<span data-ttu-id="b8b3d-139">字符串</span><span class="sxs-lookup"><span data-stu-id="b8b3d-139">String</span></span>|<span data-ttu-id="b8b3d-140">说明。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-140">The description.</span></span>|
|<span data-ttu-id="b8b3d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8b3d-141">createdDateTime</span></span>|<span data-ttu-id="b8b3d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8b3d-142">DateTimeOffset</span></span>|<span data-ttu-id="b8b3d-143">创建日期。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-143">The created date.</span></span>|
|<span data-ttu-id="b8b3d-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b8b3d-144">dueDateTime</span></span>|<span data-ttu-id="b8b3d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8b3d-145">DateTimeOffset</span></span>|<span data-ttu-id="b8b3d-146">到期日期。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-146">The due date.</span></span>|
|<span data-ttu-id="b8b3d-147">“类别”</span><span class="sxs-lookup"><span data-stu-id="b8b3d-147">category</span></span>|[<span data-ttu-id="b8b3d-148">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="b8b3d-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="b8b3d-149">类别。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-149">The category.</span></span> <span data-ttu-id="b8b3d-150">可取值为：`unknown`、`advancedThreatProtection`。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="b8b3d-151">priority</span><span class="sxs-lookup"><span data-stu-id="b8b3d-151">priority</span></span>|[<span data-ttu-id="b8b3d-152">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="b8b3d-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="b8b3d-153">优先级。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-153">The priority.</span></span> <span data-ttu-id="b8b3d-154">可取值为：`none`、`high`、`low`。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="b8b3d-155">创建</span><span class="sxs-lookup"><span data-stu-id="b8b3d-155">creator</span></span>|<span data-ttu-id="b8b3d-156">String</span><span class="sxs-lookup"><span data-stu-id="b8b3d-156">String</span></span>|<span data-ttu-id="b8b3d-157">创建者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-157">The email address of the creator.</span></span>|
|<span data-ttu-id="b8b3d-158">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="b8b3d-158">creatorNotes</span></span>|<span data-ttu-id="b8b3d-159">String</span><span class="sxs-lookup"><span data-stu-id="b8b3d-159">String</span></span>|<span data-ttu-id="b8b3d-160">来自创建者的注释。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-160">Notes from the creator.</span></span>|
|<span data-ttu-id="b8b3d-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b8b3d-161">assignedTo</span></span>|<span data-ttu-id="b8b3d-162">String</span><span class="sxs-lookup"><span data-stu-id="b8b3d-162">String</span></span>|<span data-ttu-id="b8b3d-163">将此任务分配到的管理员的姓名或电子邮件。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="b8b3d-164">status</span><span class="sxs-lookup"><span data-stu-id="b8b3d-164">status</span></span>|[<span data-ttu-id="b8b3d-165">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="b8b3d-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="b8b3d-166">状态。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-166">The status.</span></span> <span data-ttu-id="b8b3d-167">可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="b8b3d-168">响应</span><span class="sxs-lookup"><span data-stu-id="b8b3d-168">Response</span></span>
<span data-ttu-id="b8b3d-169">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-169">If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8b3d-170">示例</span><span class="sxs-lookup"><span data-stu-id="b8b3d-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8b3d-171">请求</span><span class="sxs-lookup"><span data-stu-id="b8b3d-171">Request</span></span>
<span data-ttu-id="b8b3d-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="b8b3d-173">响应</span><span class="sxs-lookup"><span data-stu-id="b8b3d-173">Response</span></span>
<span data-ttu-id="b8b3d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8b3d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 508

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "814545cc-45cc-8145-cc45-4581cc454581",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```




