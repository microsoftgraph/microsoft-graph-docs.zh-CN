---
title: 更新 managedAppOperation
description: 更新 managedAppOperation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03d40f108b302e31720f97fac435001c09c6ef10
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760368"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="ef2da-103">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="ef2da-103">Update managedAppOperation</span></span>

<span data-ttu-id="ef2da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef2da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef2da-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef2da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef2da-106">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ef2da-106">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef2da-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef2da-107">Prerequisites</span></span>
<span data-ttu-id="ef2da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef2da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef2da-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef2da-110">Permission type</span></span>|<span data-ttu-id="ef2da-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef2da-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef2da-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef2da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef2da-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2da-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef2da-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef2da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef2da-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef2da-115">Not supported.</span></span>|
|<span data-ttu-id="ef2da-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef2da-116">Application</span></span>|<span data-ttu-id="ef2da-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2da-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef2da-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef2da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef2da-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef2da-119">Request headers</span></span>
|<span data-ttu-id="ef2da-120">标头</span><span class="sxs-lookup"><span data-stu-id="ef2da-120">Header</span></span>|<span data-ttu-id="ef2da-121">值</span><span class="sxs-lookup"><span data-stu-id="ef2da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef2da-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef2da-122">Authorization</span></span>|<span data-ttu-id="ef2da-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef2da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef2da-124">接受</span><span class="sxs-lookup"><span data-stu-id="ef2da-124">Accept</span></span>|<span data-ttu-id="ef2da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef2da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef2da-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef2da-126">Request body</span></span>
<span data-ttu-id="ef2da-127">在请求正文中，提供 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef2da-127">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="ef2da-128">下表显示创建 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef2da-128">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="ef2da-129">属性</span><span class="sxs-lookup"><span data-stu-id="ef2da-129">Property</span></span>|<span data-ttu-id="ef2da-130">类型</span><span class="sxs-lookup"><span data-stu-id="ef2da-130">Type</span></span>|<span data-ttu-id="ef2da-131">说明</span><span class="sxs-lookup"><span data-stu-id="ef2da-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef2da-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ef2da-132">displayName</span></span>|<span data-ttu-id="ef2da-133">String</span><span class="sxs-lookup"><span data-stu-id="ef2da-133">String</span></span>|<span data-ttu-id="ef2da-134">操作名称。</span><span class="sxs-lookup"><span data-stu-id="ef2da-134">The operation name.</span></span>|
|<span data-ttu-id="ef2da-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef2da-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ef2da-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef2da-136">DateTimeOffset</span></span>|<span data-ttu-id="ef2da-137">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="ef2da-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="ef2da-138">state</span><span class="sxs-lookup"><span data-stu-id="ef2da-138">state</span></span>|<span data-ttu-id="ef2da-139">String</span><span class="sxs-lookup"><span data-stu-id="ef2da-139">String</span></span>|<span data-ttu-id="ef2da-140">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="ef2da-140">The current state of the operation</span></span>|
|<span data-ttu-id="ef2da-141">id</span><span class="sxs-lookup"><span data-stu-id="ef2da-141">id</span></span>|<span data-ttu-id="ef2da-142">String</span><span class="sxs-lookup"><span data-stu-id="ef2da-142">String</span></span>|<span data-ttu-id="ef2da-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ef2da-143">Key of the entity.</span></span>|
|<span data-ttu-id="ef2da-144">version</span><span class="sxs-lookup"><span data-stu-id="ef2da-144">version</span></span>|<span data-ttu-id="ef2da-145">String</span><span class="sxs-lookup"><span data-stu-id="ef2da-145">String</span></span>|<span data-ttu-id="ef2da-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="ef2da-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ef2da-147">响应</span><span class="sxs-lookup"><span data-stu-id="ef2da-147">Response</span></span>
<span data-ttu-id="ef2da-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef2da-148">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef2da-149">示例</span><span class="sxs-lookup"><span data-stu-id="ef2da-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef2da-150">请求</span><span class="sxs-lookup"><span data-stu-id="ef2da-150">Request</span></span>
<span data-ttu-id="ef2da-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef2da-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ef2da-152">响应</span><span class="sxs-lookup"><span data-stu-id="ef2da-152">Response</span></span>
<span data-ttu-id="ef2da-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef2da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




