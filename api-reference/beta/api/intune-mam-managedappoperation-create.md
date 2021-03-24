---
title: 创建 managedAppOperation
description: 创建新的 managedAppOperation 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9cdef2642ee2a3158723cf286708dc21ad3d14e3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149301"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="8fda7-103">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="8fda7-103">Create managedAppOperation</span></span>

<span data-ttu-id="8fda7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fda7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fda7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8fda7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fda7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fda7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fda7-107">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8fda7-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fda7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8fda7-108">Prerequisites</span></span>
<span data-ttu-id="8fda7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8fda7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fda7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fda7-111">Permission type</span></span>|<span data-ttu-id="8fda7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8fda7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fda7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fda7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fda7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fda7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8fda7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fda7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fda7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fda7-116">Not supported.</span></span>|
|<span data-ttu-id="8fda7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fda7-117">Application</span></span>|<span data-ttu-id="8fda7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fda7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fda7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fda7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="8fda7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8fda7-120">Request headers</span></span>
|<span data-ttu-id="8fda7-121">标头</span><span class="sxs-lookup"><span data-stu-id="8fda7-121">Header</span></span>|<span data-ttu-id="8fda7-122">值</span><span class="sxs-lookup"><span data-stu-id="8fda7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fda7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fda7-123">Authorization</span></span>|<span data-ttu-id="8fda7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8fda7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fda7-125">接受</span><span class="sxs-lookup"><span data-stu-id="8fda7-125">Accept</span></span>|<span data-ttu-id="8fda7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fda7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fda7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fda7-127">Request body</span></span>
<span data-ttu-id="8fda7-128">在请求正文中，提供 managedAppOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fda7-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="8fda7-129">下表显示创建 managedAppOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8fda7-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="8fda7-130">属性</span><span class="sxs-lookup"><span data-stu-id="8fda7-130">Property</span></span>|<span data-ttu-id="8fda7-131">类型</span><span class="sxs-lookup"><span data-stu-id="8fda7-131">Type</span></span>|<span data-ttu-id="8fda7-132">说明</span><span class="sxs-lookup"><span data-stu-id="8fda7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fda7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8fda7-133">displayName</span></span>|<span data-ttu-id="8fda7-134">String</span><span class="sxs-lookup"><span data-stu-id="8fda7-134">String</span></span>|<span data-ttu-id="8fda7-135">操作名称。</span><span class="sxs-lookup"><span data-stu-id="8fda7-135">The operation name.</span></span>|
|<span data-ttu-id="8fda7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fda7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8fda7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fda7-137">DateTimeOffset</span></span>|<span data-ttu-id="8fda7-138">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="8fda7-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="8fda7-139">state</span><span class="sxs-lookup"><span data-stu-id="8fda7-139">state</span></span>|<span data-ttu-id="8fda7-140">String</span><span class="sxs-lookup"><span data-stu-id="8fda7-140">String</span></span>|<span data-ttu-id="8fda7-141">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="8fda7-141">The current state of the operation</span></span>|
|<span data-ttu-id="8fda7-142">id</span><span class="sxs-lookup"><span data-stu-id="8fda7-142">id</span></span>|<span data-ttu-id="8fda7-143">String</span><span class="sxs-lookup"><span data-stu-id="8fda7-143">String</span></span>|<span data-ttu-id="8fda7-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8fda7-144">Key of the entity.</span></span>|
|<span data-ttu-id="8fda7-145">version</span><span class="sxs-lookup"><span data-stu-id="8fda7-145">version</span></span>|<span data-ttu-id="8fda7-146">String</span><span class="sxs-lookup"><span data-stu-id="8fda7-146">String</span></span>|<span data-ttu-id="8fda7-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="8fda7-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8fda7-148">响应</span><span class="sxs-lookup"><span data-stu-id="8fda7-148">Response</span></span>
<span data-ttu-id="8fda7-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8fda7-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fda7-150">示例</span><span class="sxs-lookup"><span data-stu-id="8fda7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fda7-151">请求</span><span class="sxs-lookup"><span data-stu-id="8fda7-151">Request</span></span>
<span data-ttu-id="8fda7-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8fda7-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="8fda7-153">响应</span><span class="sxs-lookup"><span data-stu-id="8fda7-153">Response</span></span>
<span data-ttu-id="8fda7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8fda7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```




