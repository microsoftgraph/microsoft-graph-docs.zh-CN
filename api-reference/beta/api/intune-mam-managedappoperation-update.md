---
title: 更新 managedAppOperation
description: 更新 managedAppOperation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe8b89122eb56076f1b7bb19baea2bd121f85019
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701772"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="2972f-103">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="2972f-103">Update managedAppOperation</span></span>

<span data-ttu-id="2972f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2972f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2972f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2972f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2972f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2972f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2972f-107">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2972f-107">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2972f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2972f-108">Prerequisites</span></span>
<span data-ttu-id="2972f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2972f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2972f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2972f-111">Permission type</span></span>|<span data-ttu-id="2972f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2972f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2972f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2972f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2972f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2972f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2972f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2972f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2972f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2972f-116">Not supported.</span></span>|
|<span data-ttu-id="2972f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2972f-117">Application</span></span>|<span data-ttu-id="2972f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2972f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2972f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2972f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="2972f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2972f-120">Request headers</span></span>
|<span data-ttu-id="2972f-121">标头</span><span class="sxs-lookup"><span data-stu-id="2972f-121">Header</span></span>|<span data-ttu-id="2972f-122">值</span><span class="sxs-lookup"><span data-stu-id="2972f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2972f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2972f-123">Authorization</span></span>|<span data-ttu-id="2972f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2972f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2972f-125">接受</span><span class="sxs-lookup"><span data-stu-id="2972f-125">Accept</span></span>|<span data-ttu-id="2972f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2972f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2972f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2972f-127">Request body</span></span>
<span data-ttu-id="2972f-128">在请求正文中，提供 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2972f-128">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="2972f-129">下表显示创建 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2972f-129">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="2972f-130">属性</span><span class="sxs-lookup"><span data-stu-id="2972f-130">Property</span></span>|<span data-ttu-id="2972f-131">类型</span><span class="sxs-lookup"><span data-stu-id="2972f-131">Type</span></span>|<span data-ttu-id="2972f-132">说明</span><span class="sxs-lookup"><span data-stu-id="2972f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2972f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2972f-133">displayName</span></span>|<span data-ttu-id="2972f-134">String</span><span class="sxs-lookup"><span data-stu-id="2972f-134">String</span></span>|<span data-ttu-id="2972f-135">操作名称。</span><span class="sxs-lookup"><span data-stu-id="2972f-135">The operation name.</span></span>|
|<span data-ttu-id="2972f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2972f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2972f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2972f-137">DateTimeOffset</span></span>|<span data-ttu-id="2972f-138">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="2972f-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="2972f-139">state</span><span class="sxs-lookup"><span data-stu-id="2972f-139">state</span></span>|<span data-ttu-id="2972f-140">String</span><span class="sxs-lookup"><span data-stu-id="2972f-140">String</span></span>|<span data-ttu-id="2972f-141">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="2972f-141">The current state of the operation</span></span>|
|<span data-ttu-id="2972f-142">id</span><span class="sxs-lookup"><span data-stu-id="2972f-142">id</span></span>|<span data-ttu-id="2972f-143">String</span><span class="sxs-lookup"><span data-stu-id="2972f-143">String</span></span>|<span data-ttu-id="2972f-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2972f-144">Key of the entity.</span></span>|
|<span data-ttu-id="2972f-145">version</span><span class="sxs-lookup"><span data-stu-id="2972f-145">version</span></span>|<span data-ttu-id="2972f-146">String</span><span class="sxs-lookup"><span data-stu-id="2972f-146">String</span></span>|<span data-ttu-id="2972f-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="2972f-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2972f-148">响应</span><span class="sxs-lookup"><span data-stu-id="2972f-148">Response</span></span>
<span data-ttu-id="2972f-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2972f-149">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2972f-150">示例</span><span class="sxs-lookup"><span data-stu-id="2972f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="2972f-151">请求</span><span class="sxs-lookup"><span data-stu-id="2972f-151">Request</span></span>
<span data-ttu-id="2972f-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2972f-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="2972f-153">响应</span><span class="sxs-lookup"><span data-stu-id="2972f-153">Response</span></span>
<span data-ttu-id="2972f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2972f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





