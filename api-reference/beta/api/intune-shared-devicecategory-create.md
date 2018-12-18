---
title: 创建 deviceCategory
description: 创建新的 deviceCategory 对象。
author: tfitzmac
ms.openlocfilehash: a6481784721396bc6d7011fb91ea18e8119390bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307299"
---
# <a name="create-devicecategory"></a><span data-ttu-id="02ad4-103">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="02ad4-103">Create deviceCategory</span></span>

> <span data-ttu-id="02ad4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="02ad4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02ad4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="02ad4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02ad4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="02ad4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02ad4-107">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02ad4-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02ad4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="02ad4-108">Prerequisites</span></span>

<span data-ttu-id="02ad4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="02ad4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02ad4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02ad4-111">Permission type</span></span>|<span data-ttu-id="02ad4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02ad4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02ad4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02ad4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="02ad4-114">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="02ad4-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="02ad4-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ad4-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="02ad4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02ad4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02ad4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="02ad4-117">Not supported.</span></span>|
|<span data-ttu-id="02ad4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="02ad4-118">Application</span></span>|<span data-ttu-id="02ad4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="02ad4-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02ad4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02ad4-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="02ad4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="02ad4-121">Request headers</span></span>

|<span data-ttu-id="02ad4-122">标头</span><span class="sxs-lookup"><span data-stu-id="02ad4-122">Header</span></span>|<span data-ttu-id="02ad4-123">值</span><span class="sxs-lookup"><span data-stu-id="02ad4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02ad4-124">授权</span><span class="sxs-lookup"><span data-stu-id="02ad4-124">Authorization</span></span>|<span data-ttu-id="02ad4-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="02ad4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02ad4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="02ad4-126">Accept</span></span>|<span data-ttu-id="02ad4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="02ad4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02ad4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="02ad4-128">Request body</span></span>

<span data-ttu-id="02ad4-129">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02ad4-129">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="02ad4-130">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="02ad4-130">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="02ad4-131">属性</span><span class="sxs-lookup"><span data-stu-id="02ad4-131">Property</span></span>|<span data-ttu-id="02ad4-132">类型</span><span class="sxs-lookup"><span data-stu-id="02ad4-132">Type</span></span>|<span data-ttu-id="02ad4-133">说明</span><span class="sxs-lookup"><span data-stu-id="02ad4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02ad4-134">id</span><span class="sxs-lookup"><span data-stu-id="02ad4-134">id</span></span>|<span data-ttu-id="02ad4-135">String</span><span class="sxs-lookup"><span data-stu-id="02ad4-135">String</span></span>|<span data-ttu-id="02ad4-136">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="02ad4-136">Unique identifier for the device category.</span></span> <span data-ttu-id="02ad4-137">只读。</span><span class="sxs-lookup"><span data-stu-id="02ad4-137">Read-only.</span></span>|
|<span data-ttu-id="02ad4-138">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="02ad4-138">**Obboarding**</span></span>|
|<span data-ttu-id="02ad4-139">说明</span><span class="sxs-lookup"><span data-stu-id="02ad4-139">description</span></span>|<span data-ttu-id="02ad4-140">String</span><span class="sxs-lookup"><span data-stu-id="02ad4-140">String</span></span>|<span data-ttu-id="02ad4-141">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="02ad4-141">Optional description for the device category.</span></span>|
|<span data-ttu-id="02ad4-142">displayName</span><span class="sxs-lookup"><span data-stu-id="02ad4-142">displayName</span></span>|<span data-ttu-id="02ad4-143">String</span><span class="sxs-lookup"><span data-stu-id="02ad4-143">String</span></span>|<span data-ttu-id="02ad4-144">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="02ad4-144">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="02ad4-145">响应</span><span class="sxs-lookup"><span data-stu-id="02ad4-145">Response</span></span>

<span data-ttu-id="02ad4-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02ad4-146">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02ad4-147">示例</span><span class="sxs-lookup"><span data-stu-id="02ad4-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="02ad4-148">请求</span><span class="sxs-lookup"><span data-stu-id="02ad4-148">Request</span></span>

<span data-ttu-id="02ad4-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02ad4-149">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="02ad4-150">响应</span><span class="sxs-lookup"><span data-stu-id="02ad4-150">Response</span></span>

<span data-ttu-id="02ad4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02ad4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



