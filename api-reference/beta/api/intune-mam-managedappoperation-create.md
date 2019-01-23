---
title: 创建 managedAppOperation
description: 创建新的 managedAppOperation 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4ffc03237e034321dab2bf2a03bdcca0cfbe505c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399057"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="887fd-103">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="887fd-103">Create managedAppOperation</span></span>

> <span data-ttu-id="887fd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="887fd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="887fd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="887fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="887fd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="887fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="887fd-107">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="887fd-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="887fd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="887fd-108">Prerequisites</span></span>
<span data-ttu-id="887fd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="887fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="887fd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="887fd-111">Permission type</span></span>|<span data-ttu-id="887fd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="887fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="887fd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="887fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="887fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="887fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="887fd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="887fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="887fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="887fd-116">Not supported.</span></span>|
|<span data-ttu-id="887fd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="887fd-117">Application</span></span>|<span data-ttu-id="887fd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="887fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="887fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="887fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="887fd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="887fd-120">Request headers</span></span>
|<span data-ttu-id="887fd-121">标头</span><span class="sxs-lookup"><span data-stu-id="887fd-121">Header</span></span>|<span data-ttu-id="887fd-122">值</span><span class="sxs-lookup"><span data-stu-id="887fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="887fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="887fd-123">Authorization</span></span>|<span data-ttu-id="887fd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="887fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="887fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="887fd-125">Accept</span></span>|<span data-ttu-id="887fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="887fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="887fd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="887fd-127">Request body</span></span>
<span data-ttu-id="887fd-128">在请求正文中，提供 managedAppOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="887fd-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="887fd-129">下表显示创建 managedAppOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="887fd-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="887fd-130">属性</span><span class="sxs-lookup"><span data-stu-id="887fd-130">Property</span></span>|<span data-ttu-id="887fd-131">类型</span><span class="sxs-lookup"><span data-stu-id="887fd-131">Type</span></span>|<span data-ttu-id="887fd-132">说明</span><span class="sxs-lookup"><span data-stu-id="887fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="887fd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="887fd-133">displayName</span></span>|<span data-ttu-id="887fd-134">String</span><span class="sxs-lookup"><span data-stu-id="887fd-134">String</span></span>|<span data-ttu-id="887fd-135">操作名称。</span><span class="sxs-lookup"><span data-stu-id="887fd-135">The operation name.</span></span>|
|<span data-ttu-id="887fd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="887fd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="887fd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="887fd-137">DateTimeOffset</span></span>|<span data-ttu-id="887fd-138">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="887fd-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="887fd-139">state</span><span class="sxs-lookup"><span data-stu-id="887fd-139">state</span></span>|<span data-ttu-id="887fd-140">String</span><span class="sxs-lookup"><span data-stu-id="887fd-140">String</span></span>|<span data-ttu-id="887fd-141">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="887fd-141">The current state of the operation</span></span>|
|<span data-ttu-id="887fd-142">id</span><span class="sxs-lookup"><span data-stu-id="887fd-142">id</span></span>|<span data-ttu-id="887fd-143">String</span><span class="sxs-lookup"><span data-stu-id="887fd-143">String</span></span>|<span data-ttu-id="887fd-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="887fd-144">Key of the entity.</span></span>|
|<span data-ttu-id="887fd-145">version</span><span class="sxs-lookup"><span data-stu-id="887fd-145">version</span></span>|<span data-ttu-id="887fd-146">String</span><span class="sxs-lookup"><span data-stu-id="887fd-146">String</span></span>|<span data-ttu-id="887fd-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="887fd-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="887fd-148">响应</span><span class="sxs-lookup"><span data-stu-id="887fd-148">Response</span></span>
<span data-ttu-id="887fd-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="887fd-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="887fd-150">示例</span><span class="sxs-lookup"><span data-stu-id="887fd-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="887fd-151">请求</span><span class="sxs-lookup"><span data-stu-id="887fd-151">Request</span></span>
<span data-ttu-id="887fd-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="887fd-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="887fd-153">响应</span><span class="sxs-lookup"><span data-stu-id="887fd-153">Response</span></span>
<span data-ttu-id="887fd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="887fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




