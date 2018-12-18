---
title: 创建 managedAppOperation
description: 创建新的 managedAppOperation 对象。
author: tfitzmac
ms.openlocfilehash: 21b9fdd862b72b6935e694f3a7937e675dcd5343
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313340"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="fb65b-103">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fb65b-103">Create managedAppOperation</span></span>

> <span data-ttu-id="fb65b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb65b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb65b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb65b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb65b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb65b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb65b-107">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb65b-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb65b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb65b-108">Prerequisites</span></span>
<span data-ttu-id="fb65b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fb65b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb65b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb65b-111">Permission type</span></span>|<span data-ttu-id="fb65b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb65b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb65b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb65b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb65b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb65b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb65b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb65b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb65b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb65b-116">Not supported.</span></span>|
|<span data-ttu-id="fb65b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb65b-117">Application</span></span>|<span data-ttu-id="fb65b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb65b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb65b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb65b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="fb65b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb65b-120">Request headers</span></span>
|<span data-ttu-id="fb65b-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb65b-121">Header</span></span>|<span data-ttu-id="fb65b-122">值</span><span class="sxs-lookup"><span data-stu-id="fb65b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb65b-123">授权</span><span class="sxs-lookup"><span data-stu-id="fb65b-123">Authorization</span></span>|<span data-ttu-id="fb65b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb65b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb65b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb65b-125">Accept</span></span>|<span data-ttu-id="fb65b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb65b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb65b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb65b-127">Request body</span></span>
<span data-ttu-id="fb65b-128">在请求正文中，提供 managedAppOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb65b-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="fb65b-129">下表显示创建 managedAppOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb65b-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="fb65b-130">属性</span><span class="sxs-lookup"><span data-stu-id="fb65b-130">Property</span></span>|<span data-ttu-id="fb65b-131">类型</span><span class="sxs-lookup"><span data-stu-id="fb65b-131">Type</span></span>|<span data-ttu-id="fb65b-132">说明</span><span class="sxs-lookup"><span data-stu-id="fb65b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb65b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fb65b-133">displayName</span></span>|<span data-ttu-id="fb65b-134">String</span><span class="sxs-lookup"><span data-stu-id="fb65b-134">String</span></span>|<span data-ttu-id="fb65b-135">操作名称。</span><span class="sxs-lookup"><span data-stu-id="fb65b-135">The operation name.</span></span>|
|<span data-ttu-id="fb65b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb65b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fb65b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb65b-137">DateTimeOffset</span></span>|<span data-ttu-id="fb65b-138">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="fb65b-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="fb65b-139">state</span><span class="sxs-lookup"><span data-stu-id="fb65b-139">state</span></span>|<span data-ttu-id="fb65b-140">String</span><span class="sxs-lookup"><span data-stu-id="fb65b-140">String</span></span>|<span data-ttu-id="fb65b-141">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="fb65b-141">The current state of the operation</span></span>|
|<span data-ttu-id="fb65b-142">id</span><span class="sxs-lookup"><span data-stu-id="fb65b-142">id</span></span>|<span data-ttu-id="fb65b-143">String</span><span class="sxs-lookup"><span data-stu-id="fb65b-143">String</span></span>|<span data-ttu-id="fb65b-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fb65b-144">Key of the entity.</span></span>|
|<span data-ttu-id="fb65b-145">version</span><span class="sxs-lookup"><span data-stu-id="fb65b-145">version</span></span>|<span data-ttu-id="fb65b-146">String</span><span class="sxs-lookup"><span data-stu-id="fb65b-146">String</span></span>|<span data-ttu-id="fb65b-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="fb65b-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="fb65b-148">响应</span><span class="sxs-lookup"><span data-stu-id="fb65b-148">Response</span></span>
<span data-ttu-id="fb65b-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb65b-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb65b-150">示例</span><span class="sxs-lookup"><span data-stu-id="fb65b-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb65b-151">请求</span><span class="sxs-lookup"><span data-stu-id="fb65b-151">Request</span></span>
<span data-ttu-id="fb65b-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb65b-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="fb65b-153">响应</span><span class="sxs-lookup"><span data-stu-id="fb65b-153">Response</span></span>
<span data-ttu-id="fb65b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb65b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





