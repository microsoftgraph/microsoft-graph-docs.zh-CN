---
title: 更新 sideLoadingKey
description: 更新 sideLoadingKey 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92c20c807b3763bbd0b6a4d9d9e9d3859ba1afe8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980210"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="d716b-103">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d716b-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="d716b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d716b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d716b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d716b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d716b-106">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d716b-106">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d716b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d716b-107">Prerequisites</span></span>
<span data-ttu-id="d716b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d716b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d716b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d716b-110">Permission type</span></span>|<span data-ttu-id="d716b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d716b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d716b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d716b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d716b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d716b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d716b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d716b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d716b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d716b-115">Not supported.</span></span>|
|<span data-ttu-id="d716b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d716b-116">Application</span></span>|<span data-ttu-id="d716b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d716b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d716b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d716b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="d716b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d716b-119">Request headers</span></span>
|<span data-ttu-id="d716b-120">标头</span><span class="sxs-lookup"><span data-stu-id="d716b-120">Header</span></span>|<span data-ttu-id="d716b-121">值</span><span class="sxs-lookup"><span data-stu-id="d716b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d716b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d716b-122">Authorization</span></span>|<span data-ttu-id="d716b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d716b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d716b-124">接受</span><span class="sxs-lookup"><span data-stu-id="d716b-124">Accept</span></span>|<span data-ttu-id="d716b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d716b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d716b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d716b-126">Request body</span></span>
<span data-ttu-id="d716b-127">在请求正文中, 提供[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d716b-127">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="d716b-128">下表显示创建[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d716b-128">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="d716b-129">属性</span><span class="sxs-lookup"><span data-stu-id="d716b-129">Property</span></span>|<span data-ttu-id="d716b-130">类型</span><span class="sxs-lookup"><span data-stu-id="d716b-130">Type</span></span>|<span data-ttu-id="d716b-131">说明</span><span class="sxs-lookup"><span data-stu-id="d716b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d716b-132">id</span><span class="sxs-lookup"><span data-stu-id="d716b-132">id</span></span>|<span data-ttu-id="d716b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d716b-133">String</span></span>|<span data-ttu-id="d716b-134">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="d716b-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="d716b-135">value</span><span class="sxs-lookup"><span data-stu-id="d716b-135">value</span></span>|<span data-ttu-id="d716b-136">String</span><span class="sxs-lookup"><span data-stu-id="d716b-136">String</span></span>|<span data-ttu-id="d716b-137">侧加载密钥值, 它是一个5x5 值, 由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="d716b-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="d716b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d716b-138">displayName</span></span>|<span data-ttu-id="d716b-139">字符串</span><span class="sxs-lookup"><span data-stu-id="d716b-139">String</span></span>|<span data-ttu-id="d716b-140">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="d716b-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="d716b-141">说明</span><span class="sxs-lookup"><span data-stu-id="d716b-141">description</span></span>|<span data-ttu-id="d716b-142">String</span><span class="sxs-lookup"><span data-stu-id="d716b-142">String</span></span>|<span data-ttu-id="d716b-143">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="d716b-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="d716b-144">totalActivation</span><span class="sxs-lookup"><span data-stu-id="d716b-144">totalActivation</span></span>|<span data-ttu-id="d716b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d716b-145">Int32</span></span>|<span data-ttu-id="d716b-146">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="d716b-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="d716b-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d716b-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="d716b-148">String</span><span class="sxs-lookup"><span data-stu-id="d716b-148">String</span></span>|<span data-ttu-id="d716b-149">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="d716b-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="d716b-150">响应</span><span class="sxs-lookup"><span data-stu-id="d716b-150">Response</span></span>
<span data-ttu-id="d716b-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d716b-151">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d716b-152">示例</span><span class="sxs-lookup"><span data-stu-id="d716b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d716b-153">请求</span><span class="sxs-lookup"><span data-stu-id="d716b-153">Request</span></span>
<span data-ttu-id="d716b-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d716b-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d716b-155">响应</span><span class="sxs-lookup"><span data-stu-id="d716b-155">Response</span></span>
<span data-ttu-id="d716b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d716b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





