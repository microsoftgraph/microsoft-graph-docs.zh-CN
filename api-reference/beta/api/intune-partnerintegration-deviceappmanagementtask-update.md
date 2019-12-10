---
title: 更新 deviceAppManagementTask
description: 更新 deviceAppManagementTask 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8132306e6e4047068aaead76c0e9297983e77d8d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941307"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="a884c-103">更新 deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="a884c-103">Update deviceAppManagementTask</span></span>

> <span data-ttu-id="a884c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a884c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a884c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a884c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a884c-106">更新[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a884c-106">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a884c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a884c-107">Prerequisites</span></span>
<span data-ttu-id="a884c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a884c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a884c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a884c-110">Permission type</span></span>|<span data-ttu-id="a884c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a884c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a884c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a884c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a884c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a884c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a884c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a884c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a884c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a884c-115">Not supported.</span></span>|
|<span data-ttu-id="a884c-116">Application</span><span class="sxs-lookup"><span data-stu-id="a884c-116">Application</span></span>|<span data-ttu-id="a884c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a884c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a884c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a884c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="a884c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a884c-119">Request headers</span></span>
|<span data-ttu-id="a884c-120">标头</span><span class="sxs-lookup"><span data-stu-id="a884c-120">Header</span></span>|<span data-ttu-id="a884c-121">值</span><span class="sxs-lookup"><span data-stu-id="a884c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a884c-122">授权</span><span class="sxs-lookup"><span data-stu-id="a884c-122">Authorization</span></span>|<span data-ttu-id="a884c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a884c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a884c-124">接受</span><span class="sxs-lookup"><span data-stu-id="a884c-124">Accept</span></span>|<span data-ttu-id="a884c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a884c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a884c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a884c-126">Request body</span></span>
<span data-ttu-id="a884c-127">在请求正文中，提供[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a884c-127">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="a884c-128">下表显示创建[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a884c-128">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="a884c-129">属性</span><span class="sxs-lookup"><span data-stu-id="a884c-129">Property</span></span>|<span data-ttu-id="a884c-130">类型</span><span class="sxs-lookup"><span data-stu-id="a884c-130">Type</span></span>|<span data-ttu-id="a884c-131">说明</span><span class="sxs-lookup"><span data-stu-id="a884c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a884c-132">id</span><span class="sxs-lookup"><span data-stu-id="a884c-132">id</span></span>|<span data-ttu-id="a884c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a884c-133">String</span></span>|<span data-ttu-id="a884c-134">实体键。</span><span class="sxs-lookup"><span data-stu-id="a884c-134">The entity key.</span></span>|
|<span data-ttu-id="a884c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a884c-135">displayName</span></span>|<span data-ttu-id="a884c-136">String</span><span class="sxs-lookup"><span data-stu-id="a884c-136">String</span></span>|<span data-ttu-id="a884c-137">名称。</span><span class="sxs-lookup"><span data-stu-id="a884c-137">The name.</span></span>|
|<span data-ttu-id="a884c-138">说明</span><span class="sxs-lookup"><span data-stu-id="a884c-138">description</span></span>|<span data-ttu-id="a884c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="a884c-139">String</span></span>|<span data-ttu-id="a884c-140">说明。</span><span class="sxs-lookup"><span data-stu-id="a884c-140">The description.</span></span>|
|<span data-ttu-id="a884c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a884c-141">createdDateTime</span></span>|<span data-ttu-id="a884c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a884c-142">DateTimeOffset</span></span>|<span data-ttu-id="a884c-143">创建日期。</span><span class="sxs-lookup"><span data-stu-id="a884c-143">The created date.</span></span>|
|<span data-ttu-id="a884c-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="a884c-144">dueDateTime</span></span>|<span data-ttu-id="a884c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a884c-145">DateTimeOffset</span></span>|<span data-ttu-id="a884c-146">到期日期。</span><span class="sxs-lookup"><span data-stu-id="a884c-146">The due date.</span></span>|
|<span data-ttu-id="a884c-147">“类别”</span><span class="sxs-lookup"><span data-stu-id="a884c-147">category</span></span>|[<span data-ttu-id="a884c-148">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="a884c-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="a884c-149">类别。</span><span class="sxs-lookup"><span data-stu-id="a884c-149">The category.</span></span> <span data-ttu-id="a884c-150">可取值为：`unknown`、`advancedThreatProtection`。</span><span class="sxs-lookup"><span data-stu-id="a884c-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="a884c-151">priority</span><span class="sxs-lookup"><span data-stu-id="a884c-151">priority</span></span>|[<span data-ttu-id="a884c-152">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="a884c-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="a884c-153">优先级。</span><span class="sxs-lookup"><span data-stu-id="a884c-153">The priority.</span></span> <span data-ttu-id="a884c-154">可取值为：`none`、`high`、`low`。</span><span class="sxs-lookup"><span data-stu-id="a884c-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="a884c-155">创建</span><span class="sxs-lookup"><span data-stu-id="a884c-155">creator</span></span>|<span data-ttu-id="a884c-156">字符串</span><span class="sxs-lookup"><span data-stu-id="a884c-156">String</span></span>|<span data-ttu-id="a884c-157">创建者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a884c-157">The email address of the creator.</span></span>|
|<span data-ttu-id="a884c-158">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="a884c-158">creatorNotes</span></span>|<span data-ttu-id="a884c-159">字符串</span><span class="sxs-lookup"><span data-stu-id="a884c-159">String</span></span>|<span data-ttu-id="a884c-160">来自创建者的注释。</span><span class="sxs-lookup"><span data-stu-id="a884c-160">Notes from the creator.</span></span>|
|<span data-ttu-id="a884c-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="a884c-161">assignedTo</span></span>|<span data-ttu-id="a884c-162">String</span><span class="sxs-lookup"><span data-stu-id="a884c-162">String</span></span>|<span data-ttu-id="a884c-163">将此任务分配到的管理员的姓名或电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a884c-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="a884c-164">状态</span><span class="sxs-lookup"><span data-stu-id="a884c-164">status</span></span>|[<span data-ttu-id="a884c-165">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="a884c-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="a884c-166">状态。</span><span class="sxs-lookup"><span data-stu-id="a884c-166">The status.</span></span> <span data-ttu-id="a884c-167">可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。</span><span class="sxs-lookup"><span data-stu-id="a884c-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="a884c-168">响应</span><span class="sxs-lookup"><span data-stu-id="a884c-168">Response</span></span>
<span data-ttu-id="a884c-169">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a884c-169">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a884c-170">示例</span><span class="sxs-lookup"><span data-stu-id="a884c-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="a884c-171">请求</span><span class="sxs-lookup"><span data-stu-id="a884c-171">Request</span></span>
<span data-ttu-id="a884c-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a884c-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a884c-173">响应</span><span class="sxs-lookup"><span data-stu-id="a884c-173">Response</span></span>
<span data-ttu-id="a884c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a884c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





