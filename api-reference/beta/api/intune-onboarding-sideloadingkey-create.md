---
title: 创建 sideLoadingKey
description: 创建新的 sideLoadingKey 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9cdde6b87f573414860abab77d82c17216c09170
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276894"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="0bb54-103">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="0bb54-103">Create sideLoadingKey</span></span>

<span data-ttu-id="0bb54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bb54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bb54-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0bb54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bb54-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0bb54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bb54-107">创建新的 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bb54-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bb54-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0bb54-108">Prerequisites</span></span>
<span data-ttu-id="0bb54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bb54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bb54-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bb54-111">Permission type</span></span>|<span data-ttu-id="0bb54-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0bb54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bb54-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bb54-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bb54-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0bb54-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bb54-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bb54-116">Not supported.</span></span>|
|<span data-ttu-id="0bb54-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bb54-117">Application</span></span>|<span data-ttu-id="0bb54-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bb54-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bb54-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bb54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="0bb54-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bb54-120">Request headers</span></span>
|<span data-ttu-id="0bb54-121">标头</span><span class="sxs-lookup"><span data-stu-id="0bb54-121">Header</span></span>|<span data-ttu-id="0bb54-122">值</span><span class="sxs-lookup"><span data-stu-id="0bb54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bb54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bb54-123">Authorization</span></span>|<span data-ttu-id="0bb54-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0bb54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bb54-125">接受</span><span class="sxs-lookup"><span data-stu-id="0bb54-125">Accept</span></span>|<span data-ttu-id="0bb54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bb54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bb54-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bb54-127">Request body</span></span>
<span data-ttu-id="0bb54-128">在请求正文中，提供 sideLoadingKey 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bb54-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="0bb54-129">下表显示创建 sideLoadingKey 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0bb54-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="0bb54-130">属性</span><span class="sxs-lookup"><span data-stu-id="0bb54-130">Property</span></span>|<span data-ttu-id="0bb54-131">类型</span><span class="sxs-lookup"><span data-stu-id="0bb54-131">Type</span></span>|<span data-ttu-id="0bb54-132">说明</span><span class="sxs-lookup"><span data-stu-id="0bb54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb54-133">id</span><span class="sxs-lookup"><span data-stu-id="0bb54-133">id</span></span>|<span data-ttu-id="0bb54-134">字符串</span><span class="sxs-lookup"><span data-stu-id="0bb54-134">String</span></span>|<span data-ttu-id="0bb54-135">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="0bb54-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="0bb54-136">value</span><span class="sxs-lookup"><span data-stu-id="0bb54-136">value</span></span>|<span data-ttu-id="0bb54-137">String</span><span class="sxs-lookup"><span data-stu-id="0bb54-137">String</span></span>|<span data-ttu-id="0bb54-138">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="0bb54-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="0bb54-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0bb54-139">displayName</span></span>|<span data-ttu-id="0bb54-140">字符串</span><span class="sxs-lookup"><span data-stu-id="0bb54-140">String</span></span>|<span data-ttu-id="0bb54-141">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="0bb54-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="0bb54-142">description</span><span class="sxs-lookup"><span data-stu-id="0bb54-142">description</span></span>|<span data-ttu-id="0bb54-143">字符串</span><span class="sxs-lookup"><span data-stu-id="0bb54-143">String</span></span>|<span data-ttu-id="0bb54-144">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="0bb54-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="0bb54-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="0bb54-145">totalActivation</span></span>|<span data-ttu-id="0bb54-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0bb54-146">Int32</span></span>|<span data-ttu-id="0bb54-147">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="0bb54-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="0bb54-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bb54-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="0bb54-149">字符串</span><span class="sxs-lookup"><span data-stu-id="0bb54-149">String</span></span>|<span data-ttu-id="0bb54-150">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="0bb54-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="0bb54-151">响应</span><span class="sxs-lookup"><span data-stu-id="0bb54-151">Response</span></span>
<span data-ttu-id="0bb54-152">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bb54-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bb54-153">示例</span><span class="sxs-lookup"><span data-stu-id="0bb54-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bb54-154">请求</span><span class="sxs-lookup"><span data-stu-id="0bb54-154">Request</span></span>
<span data-ttu-id="0bb54-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bb54-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0bb54-156">响应</span><span class="sxs-lookup"><span data-stu-id="0bb54-156">Response</span></span>
<span data-ttu-id="0bb54-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bb54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




