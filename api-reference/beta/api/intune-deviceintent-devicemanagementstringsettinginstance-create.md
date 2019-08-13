---
title: 创建 deviceManagementStringSettingInstance
description: 创建新的 deviceManagementStringSettingInstance 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0b9c28944be5c816940fa4f9154bb8411bd0644
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343193"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="2d143-103">创建 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2d143-103">Create deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="2d143-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d143-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d143-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d143-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d143-106">创建新的[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d143-106">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d143-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d143-107">Prerequisites</span></span>
<span data-ttu-id="2d143-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d143-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d143-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d143-110">Permission type</span></span>|<span data-ttu-id="2d143-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d143-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d143-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d143-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d143-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d143-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d143-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d143-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d143-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d143-115">Not supported.</span></span>|
|<span data-ttu-id="2d143-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d143-116">Application</span></span>|<span data-ttu-id="2d143-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d143-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d143-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d143-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2d143-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d143-119">Request headers</span></span>
|<span data-ttu-id="2d143-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d143-120">Header</span></span>|<span data-ttu-id="2d143-121">值</span><span class="sxs-lookup"><span data-stu-id="2d143-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d143-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d143-122">Authorization</span></span>|<span data-ttu-id="2d143-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d143-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d143-124">接受</span><span class="sxs-lookup"><span data-stu-id="2d143-124">Accept</span></span>|<span data-ttu-id="2d143-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d143-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d143-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d143-126">Request body</span></span>
<span data-ttu-id="2d143-127">在请求正文中, 提供 deviceManagementStringSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d143-127">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="2d143-128">下表显示创建 deviceManagementStringSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d143-128">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="2d143-129">属性</span><span class="sxs-lookup"><span data-stu-id="2d143-129">Property</span></span>|<span data-ttu-id="2d143-130">类型</span><span class="sxs-lookup"><span data-stu-id="2d143-130">Type</span></span>|<span data-ttu-id="2d143-131">说明</span><span class="sxs-lookup"><span data-stu-id="2d143-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d143-132">id</span><span class="sxs-lookup"><span data-stu-id="2d143-132">id</span></span>|<span data-ttu-id="2d143-133">String</span><span class="sxs-lookup"><span data-stu-id="2d143-133">String</span></span>|<span data-ttu-id="2d143-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="2d143-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2d143-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="2d143-135">definitionId</span></span>|<span data-ttu-id="2d143-136">String</span><span class="sxs-lookup"><span data-stu-id="2d143-136">String</span></span>|<span data-ttu-id="2d143-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="2d143-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2d143-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="2d143-138">valueJson</span></span>|<span data-ttu-id="2d143-139">String</span><span class="sxs-lookup"><span data-stu-id="2d143-139">String</span></span>|<span data-ttu-id="2d143-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d143-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2d143-141">value</span><span class="sxs-lookup"><span data-stu-id="2d143-141">value</span></span>|<span data-ttu-id="2d143-142">String</span><span class="sxs-lookup"><span data-stu-id="2d143-142">String</span></span>|<span data-ttu-id="2d143-143">字符串值</span><span class="sxs-lookup"><span data-stu-id="2d143-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="2d143-144">响应</span><span class="sxs-lookup"><span data-stu-id="2d143-144">Response</span></span>
<span data-ttu-id="2d143-145">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d143-145">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d143-146">示例</span><span class="sxs-lookup"><span data-stu-id="2d143-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d143-147">请求</span><span class="sxs-lookup"><span data-stu-id="2d143-147">Request</span></span>
<span data-ttu-id="2d143-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d143-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d143-149">响应</span><span class="sxs-lookup"><span data-stu-id="2d143-149">Response</span></span>
<span data-ttu-id="2d143-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d143-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






