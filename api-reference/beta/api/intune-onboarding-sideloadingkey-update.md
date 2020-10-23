---
title: 更新 sideLoadingKey
description: 更新 sideLoadingKey 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d4d8f3de351164e73584fb6c11248ee7acd2528
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695367"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="7bf38-103">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="7bf38-103">Update sideLoadingKey</span></span>

<span data-ttu-id="7bf38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bf38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bf38-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7bf38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bf38-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7bf38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bf38-107">更新 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7bf38-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bf38-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7bf38-108">Prerequisites</span></span>
<span data-ttu-id="7bf38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bf38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf38-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bf38-111">Permission type</span></span>|<span data-ttu-id="7bf38-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7bf38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bf38-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bf38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bf38-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf38-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7bf38-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bf38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bf38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bf38-116">Not supported.</span></span>|
|<span data-ttu-id="7bf38-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bf38-117">Application</span></span>|<span data-ttu-id="7bf38-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf38-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bf38-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bf38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="7bf38-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bf38-120">Request headers</span></span>
|<span data-ttu-id="7bf38-121">标头</span><span class="sxs-lookup"><span data-stu-id="7bf38-121">Header</span></span>|<span data-ttu-id="7bf38-122">值</span><span class="sxs-lookup"><span data-stu-id="7bf38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bf38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bf38-123">Authorization</span></span>|<span data-ttu-id="7bf38-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7bf38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bf38-125">接受</span><span class="sxs-lookup"><span data-stu-id="7bf38-125">Accept</span></span>|<span data-ttu-id="7bf38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bf38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bf38-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bf38-127">Request body</span></span>
<span data-ttu-id="7bf38-128">在请求正文中，提供 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bf38-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="7bf38-129">下表显示创建 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7bf38-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="7bf38-130">属性</span><span class="sxs-lookup"><span data-stu-id="7bf38-130">Property</span></span>|<span data-ttu-id="7bf38-131">类型</span><span class="sxs-lookup"><span data-stu-id="7bf38-131">Type</span></span>|<span data-ttu-id="7bf38-132">说明</span><span class="sxs-lookup"><span data-stu-id="7bf38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bf38-133">id</span><span class="sxs-lookup"><span data-stu-id="7bf38-133">id</span></span>|<span data-ttu-id="7bf38-134">String</span><span class="sxs-lookup"><span data-stu-id="7bf38-134">String</span></span>|<span data-ttu-id="7bf38-135">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="7bf38-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="7bf38-136">value</span><span class="sxs-lookup"><span data-stu-id="7bf38-136">value</span></span>|<span data-ttu-id="7bf38-137">String</span><span class="sxs-lookup"><span data-stu-id="7bf38-137">String</span></span>|<span data-ttu-id="7bf38-138">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="7bf38-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="7bf38-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7bf38-139">displayName</span></span>|<span data-ttu-id="7bf38-140">String</span><span class="sxs-lookup"><span data-stu-id="7bf38-140">String</span></span>|<span data-ttu-id="7bf38-141">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="7bf38-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="7bf38-142">说明</span><span class="sxs-lookup"><span data-stu-id="7bf38-142">description</span></span>|<span data-ttu-id="7bf38-143">String</span><span class="sxs-lookup"><span data-stu-id="7bf38-143">String</span></span>|<span data-ttu-id="7bf38-144">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="7bf38-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="7bf38-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="7bf38-145">totalActivation</span></span>|<span data-ttu-id="7bf38-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7bf38-146">Int32</span></span>|<span data-ttu-id="7bf38-147">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="7bf38-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="7bf38-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf38-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="7bf38-149">String</span><span class="sxs-lookup"><span data-stu-id="7bf38-149">String</span></span>|<span data-ttu-id="7bf38-150">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="7bf38-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="7bf38-151">响应</span><span class="sxs-lookup"><span data-stu-id="7bf38-151">Response</span></span>
<span data-ttu-id="7bf38-152">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bf38-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bf38-153">示例</span><span class="sxs-lookup"><span data-stu-id="7bf38-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bf38-154">请求</span><span class="sxs-lookup"><span data-stu-id="7bf38-154">Request</span></span>
<span data-ttu-id="7bf38-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bf38-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="7bf38-156">响应</span><span class="sxs-lookup"><span data-stu-id="7bf38-156">Response</span></span>
<span data-ttu-id="7bf38-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bf38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





