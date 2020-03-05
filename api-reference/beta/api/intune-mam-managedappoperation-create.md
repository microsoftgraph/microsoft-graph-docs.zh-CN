---
title: 创建 managedAppOperation
description: 创建新的 managedAppOperation 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2ba1f5a28cadee8e55b352d99ef0b02fd9a531f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463571"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="f6c70-103">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f6c70-103">Create managedAppOperation</span></span>

<span data-ttu-id="f6c70-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f6c70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6c70-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6c70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6c70-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6c70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6c70-107">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6c70-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6c70-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f6c70-108">Prerequisites</span></span>
<span data-ttu-id="f6c70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6c70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6c70-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6c70-111">Permission type</span></span>|<span data-ttu-id="f6c70-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f6c70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6c70-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6c70-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c70-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6c70-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6c70-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6c70-116">Not supported.</span></span>|
|<span data-ttu-id="f6c70-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6c70-117">Application</span></span>|<span data-ttu-id="f6c70-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c70-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6c70-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6c70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="f6c70-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6c70-120">Request headers</span></span>
|<span data-ttu-id="f6c70-121">标头</span><span class="sxs-lookup"><span data-stu-id="f6c70-121">Header</span></span>|<span data-ttu-id="f6c70-122">值</span><span class="sxs-lookup"><span data-stu-id="f6c70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6c70-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c70-123">Authorization</span></span>|<span data-ttu-id="f6c70-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f6c70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6c70-125">接受</span><span class="sxs-lookup"><span data-stu-id="f6c70-125">Accept</span></span>|<span data-ttu-id="f6c70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6c70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6c70-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6c70-127">Request body</span></span>
<span data-ttu-id="f6c70-128">在请求正文中，提供 managedAppOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6c70-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="f6c70-129">下表显示创建 managedAppOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f6c70-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="f6c70-130">属性</span><span class="sxs-lookup"><span data-stu-id="f6c70-130">Property</span></span>|<span data-ttu-id="f6c70-131">类型</span><span class="sxs-lookup"><span data-stu-id="f6c70-131">Type</span></span>|<span data-ttu-id="f6c70-132">说明</span><span class="sxs-lookup"><span data-stu-id="f6c70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c70-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f6c70-133">displayName</span></span>|<span data-ttu-id="f6c70-134">String</span><span class="sxs-lookup"><span data-stu-id="f6c70-134">String</span></span>|<span data-ttu-id="f6c70-135">操作名称。</span><span class="sxs-lookup"><span data-stu-id="f6c70-135">The operation name.</span></span>|
|<span data-ttu-id="f6c70-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6c70-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f6c70-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6c70-137">DateTimeOffset</span></span>|<span data-ttu-id="f6c70-138">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="f6c70-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="f6c70-139">state</span><span class="sxs-lookup"><span data-stu-id="f6c70-139">state</span></span>|<span data-ttu-id="f6c70-140">String</span><span class="sxs-lookup"><span data-stu-id="f6c70-140">String</span></span>|<span data-ttu-id="f6c70-141">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="f6c70-141">The current state of the operation</span></span>|
|<span data-ttu-id="f6c70-142">id</span><span class="sxs-lookup"><span data-stu-id="f6c70-142">id</span></span>|<span data-ttu-id="f6c70-143">字符串</span><span class="sxs-lookup"><span data-stu-id="f6c70-143">String</span></span>|<span data-ttu-id="f6c70-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f6c70-144">Key of the entity.</span></span>|
|<span data-ttu-id="f6c70-145">version</span><span class="sxs-lookup"><span data-stu-id="f6c70-145">version</span></span>|<span data-ttu-id="f6c70-146">String</span><span class="sxs-lookup"><span data-stu-id="f6c70-146">String</span></span>|<span data-ttu-id="f6c70-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="f6c70-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="f6c70-148">响应</span><span class="sxs-lookup"><span data-stu-id="f6c70-148">Response</span></span>
<span data-ttu-id="f6c70-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6c70-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c70-150">示例</span><span class="sxs-lookup"><span data-stu-id="f6c70-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6c70-151">请求</span><span class="sxs-lookup"><span data-stu-id="f6c70-151">Request</span></span>
<span data-ttu-id="f6c70-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6c70-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6c70-153">响应</span><span class="sxs-lookup"><span data-stu-id="f6c70-153">Response</span></span>
<span data-ttu-id="f6c70-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6c70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





