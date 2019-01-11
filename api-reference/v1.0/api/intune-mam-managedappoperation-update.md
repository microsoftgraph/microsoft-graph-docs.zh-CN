---
title: 更新 managedAppOperation
description: 更新 managedAppOperation 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d4ddc127c6d35a44f10e6ad9ff6f1fef82462392
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875577"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="9aa23-103">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="9aa23-103">Update managedAppOperation</span></span>

> <span data-ttu-id="9aa23-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9aa23-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9aa23-105">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9aa23-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9aa23-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9aa23-106">Prerequisites</span></span>
<span data-ttu-id="9aa23-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9aa23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aa23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9aa23-109">Permission type</span></span>|<span data-ttu-id="9aa23-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9aa23-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9aa23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9aa23-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9aa23-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aa23-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9aa23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9aa23-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9aa23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9aa23-114">Not supported.</span></span>|
|<span data-ttu-id="9aa23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9aa23-115">Application</span></span>|<span data-ttu-id="9aa23-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9aa23-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9aa23-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9aa23-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="9aa23-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9aa23-118">Request headers</span></span>
|<span data-ttu-id="9aa23-119">标头</span><span class="sxs-lookup"><span data-stu-id="9aa23-119">Header</span></span>|<span data-ttu-id="9aa23-120">值</span><span class="sxs-lookup"><span data-stu-id="9aa23-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9aa23-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9aa23-121">Authorization</span></span>|<span data-ttu-id="9aa23-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9aa23-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9aa23-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9aa23-123">Accept</span></span>|<span data-ttu-id="9aa23-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9aa23-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aa23-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9aa23-125">Request body</span></span>
<span data-ttu-id="9aa23-126">在请求正文中，提供 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aa23-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="9aa23-127">下表显示创建 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9aa23-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="9aa23-128">属性</span><span class="sxs-lookup"><span data-stu-id="9aa23-128">Property</span></span>|<span data-ttu-id="9aa23-129">类型</span><span class="sxs-lookup"><span data-stu-id="9aa23-129">Type</span></span>|<span data-ttu-id="9aa23-130">说明</span><span class="sxs-lookup"><span data-stu-id="9aa23-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa23-131">displayName</span><span class="sxs-lookup"><span data-stu-id="9aa23-131">displayName</span></span>|<span data-ttu-id="9aa23-132">String</span><span class="sxs-lookup"><span data-stu-id="9aa23-132">String</span></span>|<span data-ttu-id="9aa23-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="9aa23-133">The operation name.</span></span>|
|<span data-ttu-id="9aa23-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9aa23-134">lastModifiedDateTime</span></span>|<span data-ttu-id="9aa23-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aa23-135">DateTimeOffset</span></span>|<span data-ttu-id="9aa23-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="9aa23-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="9aa23-137">state</span><span class="sxs-lookup"><span data-stu-id="9aa23-137">state</span></span>|<span data-ttu-id="9aa23-138">String</span><span class="sxs-lookup"><span data-stu-id="9aa23-138">String</span></span>|<span data-ttu-id="9aa23-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="9aa23-139">The current state of the operation</span></span>|
|<span data-ttu-id="9aa23-140">id</span><span class="sxs-lookup"><span data-stu-id="9aa23-140">id</span></span>|<span data-ttu-id="9aa23-141">String</span><span class="sxs-lookup"><span data-stu-id="9aa23-141">String</span></span>|<span data-ttu-id="9aa23-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9aa23-142">Key of the entity.</span></span>|
|<span data-ttu-id="9aa23-143">version</span><span class="sxs-lookup"><span data-stu-id="9aa23-143">version</span></span>|<span data-ttu-id="9aa23-144">String</span><span class="sxs-lookup"><span data-stu-id="9aa23-144">String</span></span>|<span data-ttu-id="9aa23-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9aa23-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9aa23-146">响应</span><span class="sxs-lookup"><span data-stu-id="9aa23-146">Response</span></span>
<span data-ttu-id="9aa23-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9aa23-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9aa23-148">示例</span><span class="sxs-lookup"><span data-stu-id="9aa23-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="9aa23-149">请求</span><span class="sxs-lookup"><span data-stu-id="9aa23-149">Request</span></span>
<span data-ttu-id="9aa23-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9aa23-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9aa23-151">响应</span><span class="sxs-lookup"><span data-stu-id="9aa23-151">Response</span></span>
<span data-ttu-id="9aa23-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9aa23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



