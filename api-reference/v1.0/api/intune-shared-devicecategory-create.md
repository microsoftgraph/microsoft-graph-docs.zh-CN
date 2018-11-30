---
title: 创建 deviceCategory
description: 创建新的 deviceCategory 对象。
ms.openlocfilehash: 43a731716150a7cc9515a6497840cc47271e88c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010113"
---
# <a name="create-devicecategory"></a><span data-ttu-id="4ae33-103">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4ae33-103">Create deviceCategory</span></span>

> <span data-ttu-id="4ae33-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4ae33-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ae33-105">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ae33-105">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ae33-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ae33-106">Prerequisites</span></span>
<span data-ttu-id="4ae33-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4ae33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae33-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ae33-109">Permission type</span></span>|<span data-ttu-id="4ae33-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ae33-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ae33-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae33-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4ae33-112">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="4ae33-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4ae33-113">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae33-113">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="4ae33-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ae33-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae33-115">Not supported.</span></span>|
|<span data-ttu-id="4ae33-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ae33-116">Application</span></span>|<span data-ttu-id="4ae33-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae33-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ae33-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ae33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="4ae33-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ae33-119">Request headers</span></span>
|<span data-ttu-id="4ae33-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ae33-120">Header</span></span>|<span data-ttu-id="4ae33-121">值</span><span class="sxs-lookup"><span data-stu-id="4ae33-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ae33-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ae33-122">Authorization</span></span>|<span data-ttu-id="4ae33-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ae33-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ae33-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4ae33-124">Accept</span></span>|<span data-ttu-id="4ae33-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ae33-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae33-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ae33-126">Request body</span></span>
<span data-ttu-id="4ae33-127">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ae33-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="4ae33-128">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ae33-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="4ae33-129">属性</span><span class="sxs-lookup"><span data-stu-id="4ae33-129">Property</span></span>|<span data-ttu-id="4ae33-130">类型</span><span class="sxs-lookup"><span data-stu-id="4ae33-130">Type</span></span>|<span data-ttu-id="4ae33-131">说明</span><span class="sxs-lookup"><span data-stu-id="4ae33-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ae33-132">id</span><span class="sxs-lookup"><span data-stu-id="4ae33-132">id</span></span>|<span data-ttu-id="4ae33-133">String</span><span class="sxs-lookup"><span data-stu-id="4ae33-133">String</span></span>|<span data-ttu-id="4ae33-134">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4ae33-134">Unique identifier for the device category.</span></span> <span data-ttu-id="4ae33-135">只读。</span><span class="sxs-lookup"><span data-stu-id="4ae33-135">Read-only.</span></span>|
|<span data-ttu-id="4ae33-136">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="4ae33-136">**Onboarding**</span></span>|
|<span data-ttu-id="4ae33-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4ae33-137">displayName</span></span>|<span data-ttu-id="4ae33-138">String</span><span class="sxs-lookup"><span data-stu-id="4ae33-138">String</span></span>|<span data-ttu-id="4ae33-139">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4ae33-139">Display name for the device category.</span></span>|
|<span data-ttu-id="4ae33-140">description</span><span class="sxs-lookup"><span data-stu-id="4ae33-140">description</span></span>|<span data-ttu-id="4ae33-141">String</span><span class="sxs-lookup"><span data-stu-id="4ae33-141">String</span></span>|<span data-ttu-id="4ae33-142">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="4ae33-142">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="4ae33-143">响应</span><span class="sxs-lookup"><span data-stu-id="4ae33-143">Response</span></span>
<span data-ttu-id="4ae33-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ae33-144">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae33-145">示例</span><span class="sxs-lookup"><span data-stu-id="4ae33-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ae33-146">请求</span><span class="sxs-lookup"><span data-stu-id="4ae33-146">Request</span></span>
<span data-ttu-id="4ae33-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ae33-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="4ae33-148">响应</span><span class="sxs-lookup"><span data-stu-id="4ae33-148">Response</span></span>
<span data-ttu-id="4ae33-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ae33-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



