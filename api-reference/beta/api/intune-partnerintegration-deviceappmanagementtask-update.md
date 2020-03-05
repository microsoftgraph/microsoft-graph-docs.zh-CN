---
title: 更新 deviceAppManagementTask
description: 更新 deviceAppManagementTask 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 814ac463d788ffe6749ac1c472ba945be4d58c2b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461243"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="7ecd6-103">更新 deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="7ecd6-103">Update deviceAppManagementTask</span></span>

<span data-ttu-id="7ecd6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7ecd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ecd6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ecd6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ecd6-107">更新[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-107">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ecd6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ecd6-108">Prerequisites</span></span>
<span data-ttu-id="7ecd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ecd6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ecd6-111">Permission type</span></span>|<span data-ttu-id="7ecd6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ecd6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ecd6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ecd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ecd6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ecd6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ecd6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ecd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ecd6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-116">Not supported.</span></span>|
|<span data-ttu-id="7ecd6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ecd6-117">Application</span></span>|<span data-ttu-id="7ecd6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ecd6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ecd6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ecd6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="7ecd6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ecd6-120">Request headers</span></span>
|<span data-ttu-id="7ecd6-121">标头</span><span class="sxs-lookup"><span data-stu-id="7ecd6-121">Header</span></span>|<span data-ttu-id="7ecd6-122">值</span><span class="sxs-lookup"><span data-stu-id="7ecd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ecd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ecd6-123">Authorization</span></span>|<span data-ttu-id="7ecd6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ecd6-125">接受</span><span class="sxs-lookup"><span data-stu-id="7ecd6-125">Accept</span></span>|<span data-ttu-id="7ecd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ecd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ecd6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ecd6-127">Request body</span></span>
<span data-ttu-id="7ecd6-128">在请求正文中，提供[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-128">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="7ecd6-129">下表显示创建[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-129">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="7ecd6-130">属性</span><span class="sxs-lookup"><span data-stu-id="7ecd6-130">Property</span></span>|<span data-ttu-id="7ecd6-131">类型</span><span class="sxs-lookup"><span data-stu-id="7ecd6-131">Type</span></span>|<span data-ttu-id="7ecd6-132">说明</span><span class="sxs-lookup"><span data-stu-id="7ecd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ecd6-133">id</span><span class="sxs-lookup"><span data-stu-id="7ecd6-133">id</span></span>|<span data-ttu-id="7ecd6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7ecd6-134">String</span></span>|<span data-ttu-id="7ecd6-135">实体键。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-135">The entity key.</span></span>|
|<span data-ttu-id="7ecd6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ecd6-136">displayName</span></span>|<span data-ttu-id="7ecd6-137">String</span><span class="sxs-lookup"><span data-stu-id="7ecd6-137">String</span></span>|<span data-ttu-id="7ecd6-138">名称。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-138">The name.</span></span>|
|<span data-ttu-id="7ecd6-139">说明</span><span class="sxs-lookup"><span data-stu-id="7ecd6-139">description</span></span>|<span data-ttu-id="7ecd6-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7ecd6-140">String</span></span>|<span data-ttu-id="7ecd6-141">说明。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-141">The description.</span></span>|
|<span data-ttu-id="7ecd6-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ecd6-142">createdDateTime</span></span>|<span data-ttu-id="7ecd6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ecd6-143">DateTimeOffset</span></span>|<span data-ttu-id="7ecd6-144">创建日期。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-144">The created date.</span></span>|
|<span data-ttu-id="7ecd6-145">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="7ecd6-145">dueDateTime</span></span>|<span data-ttu-id="7ecd6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ecd6-146">DateTimeOffset</span></span>|<span data-ttu-id="7ecd6-147">到期日期。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-147">The due date.</span></span>|
|<span data-ttu-id="7ecd6-148">“类别”</span><span class="sxs-lookup"><span data-stu-id="7ecd6-148">category</span></span>|[<span data-ttu-id="7ecd6-149">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="7ecd6-149">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="7ecd6-150">类别。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-150">The category.</span></span> <span data-ttu-id="7ecd6-151">可取值为：`unknown`、`advancedThreatProtection`。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-151">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="7ecd6-152">priority</span><span class="sxs-lookup"><span data-stu-id="7ecd6-152">priority</span></span>|[<span data-ttu-id="7ecd6-153">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="7ecd6-153">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="7ecd6-154">优先级。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-154">The priority.</span></span> <span data-ttu-id="7ecd6-155">可取值为：`none`、`high`、`low`。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-155">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="7ecd6-156">创建</span><span class="sxs-lookup"><span data-stu-id="7ecd6-156">creator</span></span>|<span data-ttu-id="7ecd6-157">String</span><span class="sxs-lookup"><span data-stu-id="7ecd6-157">String</span></span>|<span data-ttu-id="7ecd6-158">创建者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-158">The email address of the creator.</span></span>|
|<span data-ttu-id="7ecd6-159">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="7ecd6-159">creatorNotes</span></span>|<span data-ttu-id="7ecd6-160">String</span><span class="sxs-lookup"><span data-stu-id="7ecd6-160">String</span></span>|<span data-ttu-id="7ecd6-161">来自创建者的注释。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-161">Notes from the creator.</span></span>|
|<span data-ttu-id="7ecd6-162">assignedTo</span><span class="sxs-lookup"><span data-stu-id="7ecd6-162">assignedTo</span></span>|<span data-ttu-id="7ecd6-163">String</span><span class="sxs-lookup"><span data-stu-id="7ecd6-163">String</span></span>|<span data-ttu-id="7ecd6-164">将此任务分配到的管理员的姓名或电子邮件。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-164">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="7ecd6-165">status</span><span class="sxs-lookup"><span data-stu-id="7ecd6-165">status</span></span>|[<span data-ttu-id="7ecd6-166">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="7ecd6-166">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="7ecd6-167">状态。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-167">The status.</span></span> <span data-ttu-id="7ecd6-168">可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-168">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="7ecd6-169">响应</span><span class="sxs-lookup"><span data-stu-id="7ecd6-169">Response</span></span>
<span data-ttu-id="7ecd6-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-170">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ecd6-171">示例</span><span class="sxs-lookup"><span data-stu-id="7ecd6-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ecd6-172">请求</span><span class="sxs-lookup"><span data-stu-id="7ecd6-172">Request</span></span>
<span data-ttu-id="7ecd6-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
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

### <a name="response"></a><span data-ttu-id="7ecd6-174">响应</span><span class="sxs-lookup"><span data-stu-id="7ecd6-174">Response</span></span>
<span data-ttu-id="7ecd6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ecd6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





