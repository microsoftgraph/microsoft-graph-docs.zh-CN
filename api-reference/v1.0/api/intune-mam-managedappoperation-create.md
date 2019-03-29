---
title: 创建 managedAppOperation
description: 创建新的 managedAppOperation 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 354795b68992307d27189d0edaa9088509d710c8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965282"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="edbe5-103">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="edbe5-103">Create managedAppOperation</span></span>

> <span data-ttu-id="edbe5-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edbe5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edbe5-105">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edbe5-105">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edbe5-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="edbe5-106">Prerequisites</span></span>
<span data-ttu-id="edbe5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edbe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edbe5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="edbe5-109">Permission type</span></span>|<span data-ttu-id="edbe5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="edbe5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edbe5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edbe5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="edbe5-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbe5-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="edbe5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edbe5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edbe5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="edbe5-114">Not supported.</span></span>|
|<span data-ttu-id="edbe5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="edbe5-115">Application</span></span>|<span data-ttu-id="edbe5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="edbe5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edbe5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edbe5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="edbe5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="edbe5-118">Request headers</span></span>
|<span data-ttu-id="edbe5-119">标头</span><span class="sxs-lookup"><span data-stu-id="edbe5-119">Header</span></span>|<span data-ttu-id="edbe5-120">值</span><span class="sxs-lookup"><span data-stu-id="edbe5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edbe5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="edbe5-121">Authorization</span></span>|<span data-ttu-id="edbe5-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="edbe5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edbe5-123">接受</span><span class="sxs-lookup"><span data-stu-id="edbe5-123">Accept</span></span>|<span data-ttu-id="edbe5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="edbe5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edbe5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="edbe5-125">Request body</span></span>
<span data-ttu-id="edbe5-126">在请求正文中，提供 managedAppOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edbe5-126">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="edbe5-127">下表显示创建 managedAppOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="edbe5-127">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="edbe5-128">属性</span><span class="sxs-lookup"><span data-stu-id="edbe5-128">Property</span></span>|<span data-ttu-id="edbe5-129">类型</span><span class="sxs-lookup"><span data-stu-id="edbe5-129">Type</span></span>|<span data-ttu-id="edbe5-130">说明</span><span class="sxs-lookup"><span data-stu-id="edbe5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edbe5-131">displayName</span><span class="sxs-lookup"><span data-stu-id="edbe5-131">displayName</span></span>|<span data-ttu-id="edbe5-132">String</span><span class="sxs-lookup"><span data-stu-id="edbe5-132">String</span></span>|<span data-ttu-id="edbe5-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="edbe5-133">The operation name.</span></span>|
|<span data-ttu-id="edbe5-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edbe5-134">lastModifiedDateTime</span></span>|<span data-ttu-id="edbe5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edbe5-135">DateTimeOffset</span></span>|<span data-ttu-id="edbe5-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="edbe5-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="edbe5-137">state</span><span class="sxs-lookup"><span data-stu-id="edbe5-137">state</span></span>|<span data-ttu-id="edbe5-138">String</span><span class="sxs-lookup"><span data-stu-id="edbe5-138">String</span></span>|<span data-ttu-id="edbe5-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="edbe5-139">The current state of the operation</span></span>|
|<span data-ttu-id="edbe5-140">id</span><span class="sxs-lookup"><span data-stu-id="edbe5-140">id</span></span>|<span data-ttu-id="edbe5-141">String</span><span class="sxs-lookup"><span data-stu-id="edbe5-141">String</span></span>|<span data-ttu-id="edbe5-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="edbe5-142">Key of the entity.</span></span>|
|<span data-ttu-id="edbe5-143">version</span><span class="sxs-lookup"><span data-stu-id="edbe5-143">version</span></span>|<span data-ttu-id="edbe5-144">String</span><span class="sxs-lookup"><span data-stu-id="edbe5-144">String</span></span>|<span data-ttu-id="edbe5-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="edbe5-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="edbe5-146">响应</span><span class="sxs-lookup"><span data-stu-id="edbe5-146">Response</span></span>
<span data-ttu-id="edbe5-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edbe5-147">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edbe5-148">示例</span><span class="sxs-lookup"><span data-stu-id="edbe5-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="edbe5-149">请求</span><span class="sxs-lookup"><span data-stu-id="edbe5-149">Request</span></span>
<span data-ttu-id="edbe5-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="edbe5-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="edbe5-151">响应</span><span class="sxs-lookup"><span data-stu-id="edbe5-151">Response</span></span>
<span data-ttu-id="edbe5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="edbe5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



