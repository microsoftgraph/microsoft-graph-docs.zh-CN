---
title: 更新 managedAppOperation
description: 更新 managedAppOperation 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2af0440e8778860e6c70b2ad965ea96c9808ba9b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164657"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="04c9e-103">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="04c9e-103">Update managedAppOperation</span></span>

> <span data-ttu-id="04c9e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04c9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04c9e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04c9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04c9e-106">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04c9e-106">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04c9e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="04c9e-107">Prerequisites</span></span>
<span data-ttu-id="04c9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="04c9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04c9e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04c9e-110">Permission type</span></span>|<span data-ttu-id="04c9e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04c9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04c9e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04c9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04c9e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04c9e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04c9e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04c9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04c9e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="04c9e-115">Not supported.</span></span>|
|<span data-ttu-id="04c9e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04c9e-116">Application</span></span>|<span data-ttu-id="04c9e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="04c9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04c9e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04c9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="04c9e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="04c9e-119">Request headers</span></span>
|<span data-ttu-id="04c9e-120">标头</span><span class="sxs-lookup"><span data-stu-id="04c9e-120">Header</span></span>|<span data-ttu-id="04c9e-121">值</span><span class="sxs-lookup"><span data-stu-id="04c9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04c9e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04c9e-122">Authorization</span></span>|<span data-ttu-id="04c9e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04c9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04c9e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04c9e-124">Accept</span></span>|<span data-ttu-id="04c9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04c9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04c9e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="04c9e-126">Request body</span></span>
<span data-ttu-id="04c9e-127">在请求正文中，提供 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04c9e-127">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="04c9e-128">下表显示创建 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04c9e-128">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="04c9e-129">属性</span><span class="sxs-lookup"><span data-stu-id="04c9e-129">Property</span></span>|<span data-ttu-id="04c9e-130">类型</span><span class="sxs-lookup"><span data-stu-id="04c9e-130">Type</span></span>|<span data-ttu-id="04c9e-131">说明</span><span class="sxs-lookup"><span data-stu-id="04c9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04c9e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="04c9e-132">displayName</span></span>|<span data-ttu-id="04c9e-133">String</span><span class="sxs-lookup"><span data-stu-id="04c9e-133">String</span></span>|<span data-ttu-id="04c9e-134">操作名称。</span><span class="sxs-lookup"><span data-stu-id="04c9e-134">The operation name.</span></span>|
|<span data-ttu-id="04c9e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04c9e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="04c9e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04c9e-136">DateTimeOffset</span></span>|<span data-ttu-id="04c9e-137">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="04c9e-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="04c9e-138">state</span><span class="sxs-lookup"><span data-stu-id="04c9e-138">state</span></span>|<span data-ttu-id="04c9e-139">String</span><span class="sxs-lookup"><span data-stu-id="04c9e-139">String</span></span>|<span data-ttu-id="04c9e-140">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="04c9e-140">The current state of the operation</span></span>|
|<span data-ttu-id="04c9e-141">id</span><span class="sxs-lookup"><span data-stu-id="04c9e-141">id</span></span>|<span data-ttu-id="04c9e-142">字符串</span><span class="sxs-lookup"><span data-stu-id="04c9e-142">String</span></span>|<span data-ttu-id="04c9e-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="04c9e-143">Key of the entity.</span></span>|
|<span data-ttu-id="04c9e-144">version</span><span class="sxs-lookup"><span data-stu-id="04c9e-144">version</span></span>|<span data-ttu-id="04c9e-145">String</span><span class="sxs-lookup"><span data-stu-id="04c9e-145">String</span></span>|<span data-ttu-id="04c9e-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="04c9e-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="04c9e-147">响应</span><span class="sxs-lookup"><span data-stu-id="04c9e-147">Response</span></span>
<span data-ttu-id="04c9e-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04c9e-148">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04c9e-149">示例</span><span class="sxs-lookup"><span data-stu-id="04c9e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="04c9e-150">请求</span><span class="sxs-lookup"><span data-stu-id="04c9e-150">Request</span></span>
<span data-ttu-id="04c9e-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04c9e-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04c9e-152">响应</span><span class="sxs-lookup"><span data-stu-id="04c9e-152">Response</span></span>
<span data-ttu-id="04c9e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04c9e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




