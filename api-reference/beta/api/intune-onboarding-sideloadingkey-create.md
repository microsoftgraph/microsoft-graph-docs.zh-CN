---
title: 创建 sideLoadingKey
description: 创建新的 sideLoadingKey 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2b55c672869b95ea85f591a67a710d64c90de61b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352410"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="e7ffc-103">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="e7ffc-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="e7ffc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ffc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ffc-106">创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-106">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7ffc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7ffc-107">Prerequisites</span></span>
<span data-ttu-id="e7ffc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7ffc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7ffc-110">Permission type</span></span>|<span data-ttu-id="e7ffc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7ffc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7ffc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7ffc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7ffc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ffc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7ffc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7ffc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7ffc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-115">Not supported.</span></span>|
|<span data-ttu-id="e7ffc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7ffc-116">Application</span></span>|<span data-ttu-id="e7ffc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ffc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7ffc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7ffc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="e7ffc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7ffc-119">Request headers</span></span>
|<span data-ttu-id="e7ffc-120">标头</span><span class="sxs-lookup"><span data-stu-id="e7ffc-120">Header</span></span>|<span data-ttu-id="e7ffc-121">值</span><span class="sxs-lookup"><span data-stu-id="e7ffc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7ffc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7ffc-122">Authorization</span></span>|<span data-ttu-id="e7ffc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7ffc-124">接受</span><span class="sxs-lookup"><span data-stu-id="e7ffc-124">Accept</span></span>|<span data-ttu-id="e7ffc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7ffc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7ffc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7ffc-126">Request body</span></span>
<span data-ttu-id="e7ffc-127">在请求正文中, 提供 sideLoadingKey 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-127">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="e7ffc-128">下表显示创建 sideLoadingKey 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-128">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="e7ffc-129">属性</span><span class="sxs-lookup"><span data-stu-id="e7ffc-129">Property</span></span>|<span data-ttu-id="e7ffc-130">类型</span><span class="sxs-lookup"><span data-stu-id="e7ffc-130">Type</span></span>|<span data-ttu-id="e7ffc-131">说明</span><span class="sxs-lookup"><span data-stu-id="e7ffc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ffc-132">id</span><span class="sxs-lookup"><span data-stu-id="e7ffc-132">id</span></span>|<span data-ttu-id="e7ffc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e7ffc-133">String</span></span>|<span data-ttu-id="e7ffc-134">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="e7ffc-135">value</span><span class="sxs-lookup"><span data-stu-id="e7ffc-135">value</span></span>|<span data-ttu-id="e7ffc-136">String</span><span class="sxs-lookup"><span data-stu-id="e7ffc-136">String</span></span>|<span data-ttu-id="e7ffc-137">侧加载密钥值, 它是一个5x5 值, 由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="e7ffc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e7ffc-138">displayName</span></span>|<span data-ttu-id="e7ffc-139">字符串</span><span class="sxs-lookup"><span data-stu-id="e7ffc-139">String</span></span>|<span data-ttu-id="e7ffc-140">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="e7ffc-141">说明</span><span class="sxs-lookup"><span data-stu-id="e7ffc-141">description</span></span>|<span data-ttu-id="e7ffc-142">String</span><span class="sxs-lookup"><span data-stu-id="e7ffc-142">String</span></span>|<span data-ttu-id="e7ffc-143">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="e7ffc-144">totalActivation</span><span class="sxs-lookup"><span data-stu-id="e7ffc-144">totalActivation</span></span>|<span data-ttu-id="e7ffc-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ffc-145">Int32</span></span>|<span data-ttu-id="e7ffc-146">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="e7ffc-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ffc-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="e7ffc-148">String</span><span class="sxs-lookup"><span data-stu-id="e7ffc-148">String</span></span>|<span data-ttu-id="e7ffc-149">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="e7ffc-150">响应</span><span class="sxs-lookup"><span data-stu-id="e7ffc-150">Response</span></span>
<span data-ttu-id="e7ffc-151">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-151">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7ffc-152">示例</span><span class="sxs-lookup"><span data-stu-id="e7ffc-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7ffc-153">请求</span><span class="sxs-lookup"><span data-stu-id="e7ffc-153">Request</span></span>
<span data-ttu-id="e7ffc-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
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

### <a name="response"></a><span data-ttu-id="e7ffc-155">响应</span><span class="sxs-lookup"><span data-stu-id="e7ffc-155">Response</span></span>
<span data-ttu-id="e7ffc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7ffc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






