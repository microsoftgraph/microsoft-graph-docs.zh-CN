---
title: 创建 deviceAppManagementTask
description: 创建新的 deviceAppManagementTask 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f90599d0feefaa7a40e8ced47ab1653eb2e4d97
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134905"
---
# <a name="create-deviceappmanagementtask"></a><span data-ttu-id="da336-103">创建 deviceAppManagementTask</span><span class="sxs-lookup"><span data-stu-id="da336-103">Create deviceAppManagementTask</span></span>

<span data-ttu-id="da336-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da336-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da336-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da336-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da336-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da336-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da336-107">创建新的 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da336-107">Create a new [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da336-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da336-108">Prerequisites</span></span>
<span data-ttu-id="da336-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da336-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da336-111">Permission type</span></span>|<span data-ttu-id="da336-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da336-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da336-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da336-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da336-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da336-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da336-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da336-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da336-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da336-116">Not supported.</span></span>|
|<span data-ttu-id="da336-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da336-117">Application</span></span>|<span data-ttu-id="da336-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da336-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da336-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da336-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="da336-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da336-120">Request headers</span></span>
|<span data-ttu-id="da336-121">标头</span><span class="sxs-lookup"><span data-stu-id="da336-121">Header</span></span>|<span data-ttu-id="da336-122">值</span><span class="sxs-lookup"><span data-stu-id="da336-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da336-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da336-123">Authorization</span></span>|<span data-ttu-id="da336-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da336-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da336-125">接受</span><span class="sxs-lookup"><span data-stu-id="da336-125">Accept</span></span>|<span data-ttu-id="da336-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da336-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da336-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da336-127">Request body</span></span>
<span data-ttu-id="da336-128">在请求正文中，提供 deviceAppManagementTask 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da336-128">In the request body, supply a JSON representation for the deviceAppManagementTask object.</span></span>

<span data-ttu-id="da336-129">下表显示创建 deviceAppManagementTask 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da336-129">The following table shows the properties that are required when you create the deviceAppManagementTask.</span></span>

|<span data-ttu-id="da336-130">属性</span><span class="sxs-lookup"><span data-stu-id="da336-130">Property</span></span>|<span data-ttu-id="da336-131">类型</span><span class="sxs-lookup"><span data-stu-id="da336-131">Type</span></span>|<span data-ttu-id="da336-132">说明</span><span class="sxs-lookup"><span data-stu-id="da336-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da336-133">id</span><span class="sxs-lookup"><span data-stu-id="da336-133">id</span></span>|<span data-ttu-id="da336-134">String</span><span class="sxs-lookup"><span data-stu-id="da336-134">String</span></span>|<span data-ttu-id="da336-135">实体键。</span><span class="sxs-lookup"><span data-stu-id="da336-135">The entity key.</span></span>|
|<span data-ttu-id="da336-136">displayName</span><span class="sxs-lookup"><span data-stu-id="da336-136">displayName</span></span>|<span data-ttu-id="da336-137">String</span><span class="sxs-lookup"><span data-stu-id="da336-137">String</span></span>|<span data-ttu-id="da336-138">名称。</span><span class="sxs-lookup"><span data-stu-id="da336-138">The name.</span></span>|
|<span data-ttu-id="da336-139">说明</span><span class="sxs-lookup"><span data-stu-id="da336-139">description</span></span>|<span data-ttu-id="da336-140">String</span><span class="sxs-lookup"><span data-stu-id="da336-140">String</span></span>|<span data-ttu-id="da336-141">说明。</span><span class="sxs-lookup"><span data-stu-id="da336-141">The description.</span></span>|
|<span data-ttu-id="da336-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da336-142">createdDateTime</span></span>|<span data-ttu-id="da336-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da336-143">DateTimeOffset</span></span>|<span data-ttu-id="da336-144">创建日期。</span><span class="sxs-lookup"><span data-stu-id="da336-144">The created date.</span></span>|
|<span data-ttu-id="da336-145">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="da336-145">dueDateTime</span></span>|<span data-ttu-id="da336-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da336-146">DateTimeOffset</span></span>|<span data-ttu-id="da336-147">截止日期。</span><span class="sxs-lookup"><span data-stu-id="da336-147">The due date.</span></span>|
|<span data-ttu-id="da336-148">“类别”</span><span class="sxs-lookup"><span data-stu-id="da336-148">category</span></span>|[<span data-ttu-id="da336-149">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="da336-149">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="da336-150">类别。</span><span class="sxs-lookup"><span data-stu-id="da336-150">The category.</span></span> <span data-ttu-id="da336-151">可取值为：`unknown`、`advancedThreatProtection`。</span><span class="sxs-lookup"><span data-stu-id="da336-151">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="da336-152">priority</span><span class="sxs-lookup"><span data-stu-id="da336-152">priority</span></span>|[<span data-ttu-id="da336-153">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="da336-153">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="da336-154">优先级。</span><span class="sxs-lookup"><span data-stu-id="da336-154">The priority.</span></span> <span data-ttu-id="da336-155">可取值为：`none`、`high`、`low`。</span><span class="sxs-lookup"><span data-stu-id="da336-155">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="da336-156">Creator</span><span class="sxs-lookup"><span data-stu-id="da336-156">creator</span></span>|<span data-ttu-id="da336-157">String</span><span class="sxs-lookup"><span data-stu-id="da336-157">String</span></span>|<span data-ttu-id="da336-158">创建者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="da336-158">The email address of the creator.</span></span>|
|<span data-ttu-id="da336-159">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="da336-159">creatorNotes</span></span>|<span data-ttu-id="da336-160">String</span><span class="sxs-lookup"><span data-stu-id="da336-160">String</span></span>|<span data-ttu-id="da336-161">创建者的备注。</span><span class="sxs-lookup"><span data-stu-id="da336-161">Notes from the creator.</span></span>|
|<span data-ttu-id="da336-162">assignedTo</span><span class="sxs-lookup"><span data-stu-id="da336-162">assignedTo</span></span>|<span data-ttu-id="da336-163">String</span><span class="sxs-lookup"><span data-stu-id="da336-163">String</span></span>|<span data-ttu-id="da336-164">分配此任务的管理员的姓名或电子邮件。</span><span class="sxs-lookup"><span data-stu-id="da336-164">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="da336-165">状态</span><span class="sxs-lookup"><span data-stu-id="da336-165">status</span></span>|[<span data-ttu-id="da336-166">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="da336-166">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="da336-167">状态。</span><span class="sxs-lookup"><span data-stu-id="da336-167">The status.</span></span> <span data-ttu-id="da336-168">可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。</span><span class="sxs-lookup"><span data-stu-id="da336-168">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="da336-169">响应</span><span class="sxs-lookup"><span data-stu-id="da336-169">Response</span></span>
<span data-ttu-id="da336-170">如果成功，此方法在响应 `201 Created` 正文中返回 响应 [代码和 deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da336-170">If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da336-171">示例</span><span class="sxs-lookup"><span data-stu-id="da336-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="da336-172">请求</span><span class="sxs-lookup"><span data-stu-id="da336-172">Request</span></span>
<span data-ttu-id="da336-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da336-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="da336-174">响应</span><span class="sxs-lookup"><span data-stu-id="da336-174">Response</span></span>
<span data-ttu-id="da336-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da336-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




