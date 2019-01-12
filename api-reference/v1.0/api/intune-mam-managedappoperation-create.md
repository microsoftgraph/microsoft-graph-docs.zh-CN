---
title: 创建 managedAppOperation
description: 创建新的 managedAppOperation 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 297296dae82a172f68b04ca13eeb9200a33aaba0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964205"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="1d8f7-103">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1d8f7-103">Create managedAppOperation</span></span>

> <span data-ttu-id="1d8f7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d8f7-105">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-105">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d8f7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d8f7-106">Prerequisites</span></span>
<span data-ttu-id="1d8f7-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1d8f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d8f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d8f7-109">Permission type</span></span>|<span data-ttu-id="1d8f7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1d8f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d8f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d8f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d8f7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d8f7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d8f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d8f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d8f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-114">Not supported.</span></span>|
|<span data-ttu-id="1d8f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d8f7-115">Application</span></span>|<span data-ttu-id="1d8f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d8f7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d8f7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="1d8f7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d8f7-118">Request headers</span></span>
|<span data-ttu-id="1d8f7-119">标头</span><span class="sxs-lookup"><span data-stu-id="1d8f7-119">Header</span></span>|<span data-ttu-id="1d8f7-120">值</span><span class="sxs-lookup"><span data-stu-id="1d8f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d8f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d8f7-121">Authorization</span></span>|<span data-ttu-id="1d8f7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d8f7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1d8f7-123">Accept</span></span>|<span data-ttu-id="1d8f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1d8f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d8f7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d8f7-125">Request body</span></span>
<span data-ttu-id="1d8f7-126">在请求正文中，提供 managedAppOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-126">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="1d8f7-127">下表显示创建 managedAppOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-127">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="1d8f7-128">属性</span><span class="sxs-lookup"><span data-stu-id="1d8f7-128">Property</span></span>|<span data-ttu-id="1d8f7-129">类型</span><span class="sxs-lookup"><span data-stu-id="1d8f7-129">Type</span></span>|<span data-ttu-id="1d8f7-130">说明</span><span class="sxs-lookup"><span data-stu-id="1d8f7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d8f7-131">displayName</span><span class="sxs-lookup"><span data-stu-id="1d8f7-131">displayName</span></span>|<span data-ttu-id="1d8f7-132">String</span><span class="sxs-lookup"><span data-stu-id="1d8f7-132">String</span></span>|<span data-ttu-id="1d8f7-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-133">The operation name.</span></span>|
|<span data-ttu-id="1d8f7-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d8f7-134">lastModifiedDateTime</span></span>|<span data-ttu-id="1d8f7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d8f7-135">DateTimeOffset</span></span>|<span data-ttu-id="1d8f7-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="1d8f7-137">state</span><span class="sxs-lookup"><span data-stu-id="1d8f7-137">state</span></span>|<span data-ttu-id="1d8f7-138">String</span><span class="sxs-lookup"><span data-stu-id="1d8f7-138">String</span></span>|<span data-ttu-id="1d8f7-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="1d8f7-139">The current state of the operation</span></span>|
|<span data-ttu-id="1d8f7-140">id</span><span class="sxs-lookup"><span data-stu-id="1d8f7-140">id</span></span>|<span data-ttu-id="1d8f7-141">String</span><span class="sxs-lookup"><span data-stu-id="1d8f7-141">String</span></span>|<span data-ttu-id="1d8f7-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-142">Key of the entity.</span></span>|
|<span data-ttu-id="1d8f7-143">version</span><span class="sxs-lookup"><span data-stu-id="1d8f7-143">version</span></span>|<span data-ttu-id="1d8f7-144">String</span><span class="sxs-lookup"><span data-stu-id="1d8f7-144">String</span></span>|<span data-ttu-id="1d8f7-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1d8f7-146">响应</span><span class="sxs-lookup"><span data-stu-id="1d8f7-146">Response</span></span>
<span data-ttu-id="1d8f7-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-147">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d8f7-148">示例</span><span class="sxs-lookup"><span data-stu-id="1d8f7-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d8f7-149">请求</span><span class="sxs-lookup"><span data-stu-id="1d8f7-149">Request</span></span>
<span data-ttu-id="1d8f7-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d8f7-151">响应</span><span class="sxs-lookup"><span data-stu-id="1d8f7-151">Response</span></span>
<span data-ttu-id="1d8f7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d8f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



