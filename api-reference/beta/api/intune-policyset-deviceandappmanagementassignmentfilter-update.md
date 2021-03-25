---
title: 更新 deviceAndAppManagementAssignmentFilter
description: 更新 deviceAndAppManagementAssignmentFilter 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa80ffa96fcd558ec7c89363406737ca538b6733
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158638"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="c1ca0-103">更新 deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="c1ca0-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="c1ca0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1ca0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1ca0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1ca0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ca0-107">更新 [deviceAndAppManagementAssignmentFilter 对象](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1ca0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1ca0-108">Prerequisites</span></span>
<span data-ttu-id="c1ca0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ca0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1ca0-111">Permission type</span></span>|<span data-ttu-id="c1ca0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1ca0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1ca0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ca0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1ca0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ca0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1ca0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ca0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ca0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-116">Not supported.</span></span>|
|<span data-ttu-id="c1ca0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1ca0-117">Application</span></span>|<span data-ttu-id="c1ca0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ca0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ca0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1ca0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="c1ca0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1ca0-120">Request headers</span></span>
|<span data-ttu-id="c1ca0-121">标头</span><span class="sxs-lookup"><span data-stu-id="c1ca0-121">Header</span></span>|<span data-ttu-id="c1ca0-122">值</span><span class="sxs-lookup"><span data-stu-id="c1ca0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1ca0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1ca0-123">Authorization</span></span>|<span data-ttu-id="c1ca0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1ca0-125">接受</span><span class="sxs-lookup"><span data-stu-id="c1ca0-125">Accept</span></span>|<span data-ttu-id="c1ca0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ca0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ca0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1ca0-127">Request body</span></span>
<span data-ttu-id="c1ca0-128">在请求正文中，提供 [deviceAndAppManagementAssignmentFilter 对象的](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="c1ca0-129">下表显示创建 [deviceAndAppManagementAssignmentFilter 时所需的属性](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="c1ca0-130">属性</span><span class="sxs-lookup"><span data-stu-id="c1ca0-130">Property</span></span>|<span data-ttu-id="c1ca0-131">类型</span><span class="sxs-lookup"><span data-stu-id="c1ca0-131">Type</span></span>|<span data-ttu-id="c1ca0-132">说明</span><span class="sxs-lookup"><span data-stu-id="c1ca0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ca0-133">id</span><span class="sxs-lookup"><span data-stu-id="c1ca0-133">id</span></span>|<span data-ttu-id="c1ca0-134">String</span><span class="sxs-lookup"><span data-stu-id="c1ca0-134">String</span></span>|<span data-ttu-id="c1ca0-135">工作分配筛选器的键。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="c1ca0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ca0-136">createdDateTime</span></span>|<span data-ttu-id="c1ca0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ca0-137">DateTimeOffset</span></span>|<span data-ttu-id="c1ca0-138">工作分配筛选器的创建时间。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="c1ca0-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ca0-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c1ca0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ca0-140">DateTimeOffset</span></span>|<span data-ttu-id="c1ca0-141">工作分配筛选器的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="c1ca0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c1ca0-142">displayName</span></span>|<span data-ttu-id="c1ca0-143">String</span><span class="sxs-lookup"><span data-stu-id="c1ca0-143">String</span></span>|<span data-ttu-id="c1ca0-144">工作分配筛选器的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="c1ca0-145">说明</span><span class="sxs-lookup"><span data-stu-id="c1ca0-145">description</span></span>|<span data-ttu-id="c1ca0-146">String</span><span class="sxs-lookup"><span data-stu-id="c1ca0-146">String</span></span>|<span data-ttu-id="c1ca0-147">工作分配筛选器的说明。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="c1ca0-148">平台</span><span class="sxs-lookup"><span data-stu-id="c1ca0-148">platform</span></span>|[<span data-ttu-id="c1ca0-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="c1ca0-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="c1ca0-150">工作分配筛选器适用的设备的平台类型。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="c1ca0-151">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="c1ca0-152">rule</span><span class="sxs-lookup"><span data-stu-id="c1ca0-152">rule</span></span>|<span data-ttu-id="c1ca0-153">String</span><span class="sxs-lookup"><span data-stu-id="c1ca0-153">String</span></span>|<span data-ttu-id="c1ca0-154">工作分配筛选器的规则定义。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="c1ca0-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1ca0-155">roleScopeTags</span></span>|<span data-ttu-id="c1ca0-156">String collection</span><span class="sxs-lookup"><span data-stu-id="c1ca0-156">String collection</span></span>|<span data-ttu-id="c1ca0-157">工作分配筛选器的 RoleScopeTags。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="c1ca0-158">响应</span><span class="sxs-lookup"><span data-stu-id="c1ca0-158">Response</span></span>
<span data-ttu-id="c1ca0-159">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ca0-160">示例</span><span class="sxs-lookup"><span data-stu-id="c1ca0-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1ca0-161">请求</span><span class="sxs-lookup"><span data-stu-id="c1ca0-161">Request</span></span>
<span data-ttu-id="c1ca0-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
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

### <a name="response"></a><span data-ttu-id="c1ca0-163">响应</span><span class="sxs-lookup"><span data-stu-id="c1ca0-163">Response</span></span>
<span data-ttu-id="c1ca0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1ca0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




