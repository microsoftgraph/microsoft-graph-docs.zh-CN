---
title: 创建 deviceManagementAbstractComplexSettingInstance
description: 创建新的 deviceManagementAbstractComplexSettingInstance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d537ce7eb8d222c05e5c1c30031ab09e7711150f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146718"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="1c5ed-103">创建 deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1c5ed-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="1c5ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c5ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c5ed-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c5ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c5ed-107">创建新的 [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-107">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c5ed-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1c5ed-108">Prerequisites</span></span>
<span data-ttu-id="1c5ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c5ed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c5ed-111">Permission type</span></span>|<span data-ttu-id="1c5ed-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c5ed-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c5ed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c5ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c5ed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c5ed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c5ed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c5ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c5ed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-116">Not supported.</span></span>|
|<span data-ttu-id="1c5ed-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c5ed-117">Application</span></span>|<span data-ttu-id="1c5ed-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c5ed-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c5ed-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c5ed-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1c5ed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c5ed-120">Request headers</span></span>
|<span data-ttu-id="1c5ed-121">标头</span><span class="sxs-lookup"><span data-stu-id="1c5ed-121">Header</span></span>|<span data-ttu-id="1c5ed-122">值</span><span class="sxs-lookup"><span data-stu-id="1c5ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c5ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c5ed-123">Authorization</span></span>|<span data-ttu-id="1c5ed-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c5ed-125">接受</span><span class="sxs-lookup"><span data-stu-id="1c5ed-125">Accept</span></span>|<span data-ttu-id="1c5ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c5ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c5ed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c5ed-127">Request body</span></span>
<span data-ttu-id="1c5ed-128">在请求正文中，提供 deviceManagementAbstractComplexSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-128">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="1c5ed-129">下表显示创建 deviceManagementAbstractComplexSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-129">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="1c5ed-130">属性</span><span class="sxs-lookup"><span data-stu-id="1c5ed-130">Property</span></span>|<span data-ttu-id="1c5ed-131">类型</span><span class="sxs-lookup"><span data-stu-id="1c5ed-131">Type</span></span>|<span data-ttu-id="1c5ed-132">说明</span><span class="sxs-lookup"><span data-stu-id="1c5ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c5ed-133">id</span><span class="sxs-lookup"><span data-stu-id="1c5ed-133">id</span></span>|<span data-ttu-id="1c5ed-134">String</span><span class="sxs-lookup"><span data-stu-id="1c5ed-134">String</span></span>|<span data-ttu-id="1c5ed-135">设置实例 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1c5ed-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1c5ed-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="1c5ed-136">definitionId</span></span>|<span data-ttu-id="1c5ed-137">String</span><span class="sxs-lookup"><span data-stu-id="1c5ed-137">String</span></span>|<span data-ttu-id="1c5ed-138">此实例的设置定义的 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1c5ed-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1c5ed-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="1c5ed-139">valueJson</span></span>|<span data-ttu-id="1c5ed-140">String</span><span class="sxs-lookup"><span data-stu-id="1c5ed-140">String</span></span>|<span data-ttu-id="1c5ed-141">值的 JSON 表示形式 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1c5ed-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1c5ed-142">implementationId</span><span class="sxs-lookup"><span data-stu-id="1c5ed-142">implementationId</span></span>|<span data-ttu-id="1c5ed-143">String</span><span class="sxs-lookup"><span data-stu-id="1c5ed-143">String</span></span>|<span data-ttu-id="1c5ed-144">此复杂设置所选实现的定义 ID</span><span class="sxs-lookup"><span data-stu-id="1c5ed-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="1c5ed-145">响应</span><span class="sxs-lookup"><span data-stu-id="1c5ed-145">Response</span></span>
<span data-ttu-id="1c5ed-146">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-146">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c5ed-147">示例</span><span class="sxs-lookup"><span data-stu-id="1c5ed-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c5ed-148">请求</span><span class="sxs-lookup"><span data-stu-id="1c5ed-148">Request</span></span>
<span data-ttu-id="1c5ed-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="1c5ed-150">响应</span><span class="sxs-lookup"><span data-stu-id="1c5ed-150">Response</span></span>
<span data-ttu-id="1c5ed-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c5ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "433e9565-9565-433e-6595-3e4365953e43",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```




