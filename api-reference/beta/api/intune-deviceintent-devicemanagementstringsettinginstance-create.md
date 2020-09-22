---
title: 创建 deviceManagementStringSettingInstance
description: 创建新的 deviceManagementStringSettingInstance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 421fafbd82934b1fa31586970c92abe647c7c9c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054320"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="5e3af-103">创建 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="5e3af-103">Create deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="5e3af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e3af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e3af-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e3af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e3af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e3af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e3af-107">创建新的 [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e3af-107">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e3af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e3af-108">Prerequisites</span></span>
<span data-ttu-id="5e3af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e3af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e3af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e3af-111">Permission type</span></span>|<span data-ttu-id="5e3af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e3af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e3af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e3af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e3af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e3af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e3af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e3af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e3af-116">Not supported.</span></span>|
|<span data-ttu-id="5e3af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e3af-117">Application</span></span>|<span data-ttu-id="5e3af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e3af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e3af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="5e3af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e3af-120">Request headers</span></span>
|<span data-ttu-id="5e3af-121">标头</span><span class="sxs-lookup"><span data-stu-id="5e3af-121">Header</span></span>|<span data-ttu-id="5e3af-122">值</span><span class="sxs-lookup"><span data-stu-id="5e3af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e3af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e3af-123">Authorization</span></span>|<span data-ttu-id="5e3af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e3af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e3af-125">接受</span><span class="sxs-lookup"><span data-stu-id="5e3af-125">Accept</span></span>|<span data-ttu-id="5e3af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e3af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e3af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e3af-127">Request body</span></span>
<span data-ttu-id="5e3af-128">在请求正文中，提供 deviceManagementStringSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e3af-128">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="5e3af-129">下表显示创建 deviceManagementStringSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5e3af-129">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="5e3af-130">属性</span><span class="sxs-lookup"><span data-stu-id="5e3af-130">Property</span></span>|<span data-ttu-id="5e3af-131">类型</span><span class="sxs-lookup"><span data-stu-id="5e3af-131">Type</span></span>|<span data-ttu-id="5e3af-132">说明</span><span class="sxs-lookup"><span data-stu-id="5e3af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e3af-133">id</span><span class="sxs-lookup"><span data-stu-id="5e3af-133">id</span></span>|<span data-ttu-id="5e3af-134">String</span><span class="sxs-lookup"><span data-stu-id="5e3af-134">String</span></span>|<span data-ttu-id="5e3af-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="5e3af-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5e3af-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="5e3af-136">definitionId</span></span>|<span data-ttu-id="5e3af-137">String</span><span class="sxs-lookup"><span data-stu-id="5e3af-137">String</span></span>|<span data-ttu-id="5e3af-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="5e3af-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5e3af-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="5e3af-139">valueJson</span></span>|<span data-ttu-id="5e3af-140">String</span><span class="sxs-lookup"><span data-stu-id="5e3af-140">String</span></span>|<span data-ttu-id="5e3af-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e3af-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="5e3af-142">value</span><span class="sxs-lookup"><span data-stu-id="5e3af-142">value</span></span>|<span data-ttu-id="5e3af-143">String</span><span class="sxs-lookup"><span data-stu-id="5e3af-143">String</span></span>|<span data-ttu-id="5e3af-144">字符串值</span><span class="sxs-lookup"><span data-stu-id="5e3af-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="5e3af-145">响应</span><span class="sxs-lookup"><span data-stu-id="5e3af-145">Response</span></span>
<span data-ttu-id="5e3af-146">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e3af-146">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e3af-147">示例</span><span class="sxs-lookup"><span data-stu-id="5e3af-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e3af-148">请求</span><span class="sxs-lookup"><span data-stu-id="5e3af-148">Request</span></span>
<span data-ttu-id="5e3af-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e3af-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="5e3af-150">响应</span><span class="sxs-lookup"><span data-stu-id="5e3af-150">Response</span></span>
<span data-ttu-id="5e3af-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e3af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```






