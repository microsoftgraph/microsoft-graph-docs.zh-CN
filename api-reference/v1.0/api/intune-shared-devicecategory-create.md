---
title: 创建 deviceCategory
description: 创建新的 deviceCategory 对象。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 603a42e7b662295e73461732f4a8e0462092847f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512109"
---
# <a name="create-devicecategory"></a><span data-ttu-id="f7e96-103">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f7e96-103">Create deviceCategory</span></span>

<span data-ttu-id="f7e96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7e96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7e96-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7e96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7e96-106">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7e96-106">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7e96-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7e96-107">Prerequisites</span></span>
<span data-ttu-id="f7e96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e96-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7e96-110">Permission type</span></span>|<span data-ttu-id="f7e96-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7e96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7e96-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e96-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f7e96-113">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="f7e96-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f7e96-114">DeviceManagementManaged 设备。 ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="f7e96-114">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="f7e96-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7e96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7e96-116">Not supported.</span></span>|
|<span data-ttu-id="f7e96-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7e96-117">Application</span></span>|<span data-ttu-id="f7e96-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7e96-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7e96-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7e96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="f7e96-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7e96-120">Request headers</span></span>
|<span data-ttu-id="f7e96-121">标头</span><span class="sxs-lookup"><span data-stu-id="f7e96-121">Header</span></span>|<span data-ttu-id="f7e96-122">值</span><span class="sxs-lookup"><span data-stu-id="f7e96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7e96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e96-123">Authorization</span></span>|<span data-ttu-id="f7e96-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7e96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7e96-125">接受</span><span class="sxs-lookup"><span data-stu-id="f7e96-125">Accept</span></span>|<span data-ttu-id="f7e96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7e96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e96-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7e96-127">Request body</span></span>
<span data-ttu-id="f7e96-128">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7e96-128">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="f7e96-129">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f7e96-129">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="f7e96-130">属性</span><span class="sxs-lookup"><span data-stu-id="f7e96-130">Property</span></span>|<span data-ttu-id="f7e96-131">类型</span><span class="sxs-lookup"><span data-stu-id="f7e96-131">Type</span></span>|<span data-ttu-id="f7e96-132">说明</span><span class="sxs-lookup"><span data-stu-id="f7e96-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7e96-133">id</span><span class="sxs-lookup"><span data-stu-id="f7e96-133">id</span></span>|<span data-ttu-id="f7e96-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f7e96-134">String</span></span>|<span data-ttu-id="f7e96-135">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f7e96-135">Unique identifier for the device category.</span></span> <span data-ttu-id="f7e96-136">只读。</span><span class="sxs-lookup"><span data-stu-id="f7e96-136">Read-only.</span></span>|
|<span data-ttu-id="f7e96-137">**载入**</span><span class="sxs-lookup"><span data-stu-id="f7e96-137">**Onboarding**</span></span>|
|<span data-ttu-id="f7e96-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f7e96-138">displayName</span></span>|<span data-ttu-id="f7e96-139">String</span><span class="sxs-lookup"><span data-stu-id="f7e96-139">String</span></span>|<span data-ttu-id="f7e96-140">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f7e96-140">Display name for the device category.</span></span>|
|<span data-ttu-id="f7e96-141">说明</span><span class="sxs-lookup"><span data-stu-id="f7e96-141">description</span></span>|<span data-ttu-id="f7e96-142">String</span><span class="sxs-lookup"><span data-stu-id="f7e96-142">String</span></span>|<span data-ttu-id="f7e96-143">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="f7e96-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="f7e96-144">响应</span><span class="sxs-lookup"><span data-stu-id="f7e96-144">Response</span></span>
<span data-ttu-id="f7e96-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7e96-145">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e96-146">示例</span><span class="sxs-lookup"><span data-stu-id="f7e96-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7e96-147">请求</span><span class="sxs-lookup"><span data-stu-id="f7e96-147">Request</span></span>
<span data-ttu-id="f7e96-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7e96-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7e96-149">响应</span><span class="sxs-lookup"><span data-stu-id="f7e96-149">Response</span></span>
<span data-ttu-id="f7e96-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7e96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




