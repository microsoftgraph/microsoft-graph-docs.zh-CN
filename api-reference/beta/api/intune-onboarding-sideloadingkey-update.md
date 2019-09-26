---
title: 更新 sideLoadingKey
description: 更新 sideLoadingKey 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f075e72f11f70050fd6d460cfee4c43144ffbfdd
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37190318"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="ca818-103">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="ca818-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="ca818-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca818-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca818-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca818-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca818-106">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ca818-106">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca818-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca818-107">Prerequisites</span></span>
<span data-ttu-id="ca818-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca818-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca818-110">Permission type</span></span>|<span data-ttu-id="ca818-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca818-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca818-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca818-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca818-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca818-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ca818-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca818-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca818-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca818-115">Not supported.</span></span>|
|<span data-ttu-id="ca818-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca818-116">Application</span></span>|<span data-ttu-id="ca818-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca818-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca818-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca818-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="ca818-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca818-119">Request headers</span></span>
|<span data-ttu-id="ca818-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca818-120">Header</span></span>|<span data-ttu-id="ca818-121">值</span><span class="sxs-lookup"><span data-stu-id="ca818-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca818-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca818-122">Authorization</span></span>|<span data-ttu-id="ca818-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca818-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca818-124">接受</span><span class="sxs-lookup"><span data-stu-id="ca818-124">Accept</span></span>|<span data-ttu-id="ca818-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca818-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca818-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca818-126">Request body</span></span>
<span data-ttu-id="ca818-127">在请求正文中，提供[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca818-127">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="ca818-128">下表显示创建[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca818-128">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="ca818-129">属性</span><span class="sxs-lookup"><span data-stu-id="ca818-129">Property</span></span>|<span data-ttu-id="ca818-130">类型</span><span class="sxs-lookup"><span data-stu-id="ca818-130">Type</span></span>|<span data-ttu-id="ca818-131">说明</span><span class="sxs-lookup"><span data-stu-id="ca818-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca818-132">id</span><span class="sxs-lookup"><span data-stu-id="ca818-132">id</span></span>|<span data-ttu-id="ca818-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ca818-133">String</span></span>|<span data-ttu-id="ca818-134">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="ca818-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="ca818-135">value</span><span class="sxs-lookup"><span data-stu-id="ca818-135">value</span></span>|<span data-ttu-id="ca818-136">String</span><span class="sxs-lookup"><span data-stu-id="ca818-136">String</span></span>|<span data-ttu-id="ca818-137">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="ca818-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="ca818-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ca818-138">displayName</span></span>|<span data-ttu-id="ca818-139">字符串</span><span class="sxs-lookup"><span data-stu-id="ca818-139">String</span></span>|<span data-ttu-id="ca818-140">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="ca818-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ca818-141">说明</span><span class="sxs-lookup"><span data-stu-id="ca818-141">description</span></span>|<span data-ttu-id="ca818-142">String</span><span class="sxs-lookup"><span data-stu-id="ca818-142">String</span></span>|<span data-ttu-id="ca818-143">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="ca818-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="ca818-144">totalActivation</span><span class="sxs-lookup"><span data-stu-id="ca818-144">totalActivation</span></span>|<span data-ttu-id="ca818-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ca818-145">Int32</span></span>|<span data-ttu-id="ca818-146">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="ca818-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ca818-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca818-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="ca818-148">String</span><span class="sxs-lookup"><span data-stu-id="ca818-148">String</span></span>|<span data-ttu-id="ca818-149">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="ca818-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="ca818-150">响应</span><span class="sxs-lookup"><span data-stu-id="ca818-150">Response</span></span>
<span data-ttu-id="ca818-151">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca818-151">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca818-152">示例</span><span class="sxs-lookup"><span data-stu-id="ca818-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca818-153">请求</span><span class="sxs-lookup"><span data-stu-id="ca818-153">Request</span></span>
<span data-ttu-id="ca818-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca818-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca818-155">响应</span><span class="sxs-lookup"><span data-stu-id="ca818-155">Response</span></span>
<span data-ttu-id="ca818-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca818-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




