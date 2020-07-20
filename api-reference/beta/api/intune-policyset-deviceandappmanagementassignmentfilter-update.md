---
title: 更新 deviceAndAppManagementAssignmentFilter
description: 更新 deviceAndAppManagementAssignmentFilter 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5fd7242879c9a086b08895637ad811b5fd48160
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791726"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="4015d-103">更新 deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="4015d-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="4015d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4015d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4015d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4015d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4015d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4015d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4015d-107">更新[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4015d-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4015d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4015d-108">Prerequisites</span></span>
<span data-ttu-id="4015d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4015d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4015d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4015d-111">Permission type</span></span>|<span data-ttu-id="4015d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4015d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4015d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4015d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4015d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4015d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4015d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4015d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4015d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4015d-116">Not supported.</span></span>|
|<span data-ttu-id="4015d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4015d-117">Application</span></span>|<span data-ttu-id="4015d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4015d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4015d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4015d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="4015d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4015d-120">Request headers</span></span>
|<span data-ttu-id="4015d-121">标头</span><span class="sxs-lookup"><span data-stu-id="4015d-121">Header</span></span>|<span data-ttu-id="4015d-122">值</span><span class="sxs-lookup"><span data-stu-id="4015d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4015d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4015d-123">Authorization</span></span>|<span data-ttu-id="4015d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4015d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4015d-125">接受</span><span class="sxs-lookup"><span data-stu-id="4015d-125">Accept</span></span>|<span data-ttu-id="4015d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4015d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4015d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4015d-127">Request body</span></span>
<span data-ttu-id="4015d-128">在请求正文中，提供[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4015d-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="4015d-129">下表显示创建[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4015d-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="4015d-130">属性</span><span class="sxs-lookup"><span data-stu-id="4015d-130">Property</span></span>|<span data-ttu-id="4015d-131">类型</span><span class="sxs-lookup"><span data-stu-id="4015d-131">Type</span></span>|<span data-ttu-id="4015d-132">说明</span><span class="sxs-lookup"><span data-stu-id="4015d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4015d-133">id</span><span class="sxs-lookup"><span data-stu-id="4015d-133">id</span></span>|<span data-ttu-id="4015d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4015d-134">String</span></span>|<span data-ttu-id="4015d-135">工作分配筛选器的键。</span><span class="sxs-lookup"><span data-stu-id="4015d-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="4015d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4015d-136">createdDateTime</span></span>|<span data-ttu-id="4015d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4015d-137">DateTimeOffset</span></span>|<span data-ttu-id="4015d-138">工作分配筛选器的创建时间。</span><span class="sxs-lookup"><span data-stu-id="4015d-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="4015d-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4015d-139">lastModifiedDateTime</span></span>|<span data-ttu-id="4015d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4015d-140">DateTimeOffset</span></span>|<span data-ttu-id="4015d-141">工作分配筛选器的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="4015d-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="4015d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4015d-142">displayName</span></span>|<span data-ttu-id="4015d-143">String</span><span class="sxs-lookup"><span data-stu-id="4015d-143">String</span></span>|<span data-ttu-id="4015d-144">工作分配筛选器的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="4015d-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="4015d-145">说明</span><span class="sxs-lookup"><span data-stu-id="4015d-145">description</span></span>|<span data-ttu-id="4015d-146">String</span><span class="sxs-lookup"><span data-stu-id="4015d-146">String</span></span>|<span data-ttu-id="4015d-147">工作分配筛选器的说明。</span><span class="sxs-lookup"><span data-stu-id="4015d-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="4015d-148">platform</span><span class="sxs-lookup"><span data-stu-id="4015d-148">platform</span></span>|[<span data-ttu-id="4015d-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="4015d-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="4015d-150">工作分配筛选器将适用的设备的平台类型。</span><span class="sxs-lookup"><span data-stu-id="4015d-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="4015d-151">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="4015d-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="4015d-152">标尺</span><span class="sxs-lookup"><span data-stu-id="4015d-152">rule</span></span>|<span data-ttu-id="4015d-153">String</span><span class="sxs-lookup"><span data-stu-id="4015d-153">String</span></span>|<span data-ttu-id="4015d-154">工作分配筛选器的规则定义。</span><span class="sxs-lookup"><span data-stu-id="4015d-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="4015d-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="4015d-155">roleScopeTags</span></span>|<span data-ttu-id="4015d-156">String collection</span><span class="sxs-lookup"><span data-stu-id="4015d-156">String collection</span></span>|<span data-ttu-id="4015d-157">RoleScopeTags 的工作分配筛选器。</span><span class="sxs-lookup"><span data-stu-id="4015d-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="4015d-158">响应</span><span class="sxs-lookup"><span data-stu-id="4015d-158">Response</span></span>
<span data-ttu-id="4015d-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4015d-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4015d-160">示例</span><span class="sxs-lookup"><span data-stu-id="4015d-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="4015d-161">请求</span><span class="sxs-lookup"><span data-stu-id="4015d-161">Request</span></span>
<span data-ttu-id="4015d-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4015d-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4015d-163">响应</span><span class="sxs-lookup"><span data-stu-id="4015d-163">Response</span></span>
<span data-ttu-id="4015d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4015d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



