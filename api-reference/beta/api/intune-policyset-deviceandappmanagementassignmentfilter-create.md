---
title: 创建 deviceAndAppManagementAssignmentFilter
description: 创建新的 deviceAndAppManagementAssignmentFilter 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c72cb53c03c88843a252ebb8230800d1a4c7a5e1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791754"
---
# <a name="create-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="3aaca-103">创建 deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="3aaca-103">Create deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="3aaca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aaca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3aaca-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3aaca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3aaca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3aaca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3aaca-107">创建新的[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3aaca-107">Create a new [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3aaca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3aaca-108">Prerequisites</span></span>
<span data-ttu-id="3aaca-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3aaca-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3aaca-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aaca-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aaca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3aaca-111">Permission type</span></span>|<span data-ttu-id="3aaca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3aaca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3aaca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3aaca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3aaca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aaca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3aaca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3aaca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3aaca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3aaca-116">Not supported.</span></span>|
|<span data-ttu-id="3aaca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3aaca-117">Application</span></span>|<span data-ttu-id="3aaca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aaca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aaca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3aaca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters
```

## <a name="request-headers"></a><span data-ttu-id="3aaca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3aaca-120">Request headers</span></span>
|<span data-ttu-id="3aaca-121">标头</span><span class="sxs-lookup"><span data-stu-id="3aaca-121">Header</span></span>|<span data-ttu-id="3aaca-122">值</span><span class="sxs-lookup"><span data-stu-id="3aaca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3aaca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aaca-123">Authorization</span></span>|<span data-ttu-id="3aaca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3aaca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3aaca-125">接受</span><span class="sxs-lookup"><span data-stu-id="3aaca-125">Accept</span></span>|<span data-ttu-id="3aaca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3aaca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aaca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3aaca-127">Request body</span></span>
<span data-ttu-id="3aaca-128">在请求正文中，提供 deviceAndAppManagementAssignmentFilter 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3aaca-128">In the request body, supply a JSON representation for the deviceAndAppManagementAssignmentFilter object.</span></span>

<span data-ttu-id="3aaca-129">下表显示创建 deviceAndAppManagementAssignmentFilter 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3aaca-129">The following table shows the properties that are required when you create the deviceAndAppManagementAssignmentFilter.</span></span>

|<span data-ttu-id="3aaca-130">属性</span><span class="sxs-lookup"><span data-stu-id="3aaca-130">Property</span></span>|<span data-ttu-id="3aaca-131">类型</span><span class="sxs-lookup"><span data-stu-id="3aaca-131">Type</span></span>|<span data-ttu-id="3aaca-132">说明</span><span class="sxs-lookup"><span data-stu-id="3aaca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aaca-133">id</span><span class="sxs-lookup"><span data-stu-id="3aaca-133">id</span></span>|<span data-ttu-id="3aaca-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3aaca-134">String</span></span>|<span data-ttu-id="3aaca-135">工作分配筛选器的键。</span><span class="sxs-lookup"><span data-stu-id="3aaca-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="3aaca-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3aaca-136">createdDateTime</span></span>|<span data-ttu-id="3aaca-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aaca-137">DateTimeOffset</span></span>|<span data-ttu-id="3aaca-138">工作分配筛选器的创建时间。</span><span class="sxs-lookup"><span data-stu-id="3aaca-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="3aaca-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3aaca-139">lastModifiedDateTime</span></span>|<span data-ttu-id="3aaca-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aaca-140">DateTimeOffset</span></span>|<span data-ttu-id="3aaca-141">工作分配筛选器的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="3aaca-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="3aaca-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3aaca-142">displayName</span></span>|<span data-ttu-id="3aaca-143">String</span><span class="sxs-lookup"><span data-stu-id="3aaca-143">String</span></span>|<span data-ttu-id="3aaca-144">工作分配筛选器的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="3aaca-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="3aaca-145">说明</span><span class="sxs-lookup"><span data-stu-id="3aaca-145">description</span></span>|<span data-ttu-id="3aaca-146">String</span><span class="sxs-lookup"><span data-stu-id="3aaca-146">String</span></span>|<span data-ttu-id="3aaca-147">工作分配筛选器的说明。</span><span class="sxs-lookup"><span data-stu-id="3aaca-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="3aaca-148">platform</span><span class="sxs-lookup"><span data-stu-id="3aaca-148">platform</span></span>|[<span data-ttu-id="3aaca-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="3aaca-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="3aaca-150">工作分配筛选器将适用的设备的平台类型。</span><span class="sxs-lookup"><span data-stu-id="3aaca-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="3aaca-151">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="3aaca-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="3aaca-152">标尺</span><span class="sxs-lookup"><span data-stu-id="3aaca-152">rule</span></span>|<span data-ttu-id="3aaca-153">String</span><span class="sxs-lookup"><span data-stu-id="3aaca-153">String</span></span>|<span data-ttu-id="3aaca-154">工作分配筛选器的规则定义。</span><span class="sxs-lookup"><span data-stu-id="3aaca-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="3aaca-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="3aaca-155">roleScopeTags</span></span>|<span data-ttu-id="3aaca-156">String collection</span><span class="sxs-lookup"><span data-stu-id="3aaca-156">String collection</span></span>|<span data-ttu-id="3aaca-157">RoleScopeTags 的工作分配筛选器。</span><span class="sxs-lookup"><span data-stu-id="3aaca-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="3aaca-158">响应</span><span class="sxs-lookup"><span data-stu-id="3aaca-158">Response</span></span>
<span data-ttu-id="3aaca-159">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3aaca-159">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aaca-160">示例</span><span class="sxs-lookup"><span data-stu-id="3aaca-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="3aaca-161">请求</span><span class="sxs-lookup"><span data-stu-id="3aaca-161">Request</span></span>
<span data-ttu-id="3aaca-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3aaca-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/assignmentFilters
Content-type: application/json
Content-length: 274

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3aaca-163">响应</span><span class="sxs-lookup"><span data-stu-id="3aaca-163">Response</span></span>
<span data-ttu-id="3aaca-164">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3aaca-164">Here is an example of the response.</span></span> <span data-ttu-id="3aaca-165">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3aaca-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3aaca-166">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3aaca-166">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 446

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "819818db-18db-8198-db18-9881db189881",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```



