---
title: 更新 deviceManagementAbstractComplexSettingInstance
description: 更新 deviceManagementAbstractComplexSettingInstance 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fbda6661c56593147373ee0b25e41c3d151ad622
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472770"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="9a935-103">更新 deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="9a935-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="9a935-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9a935-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a935-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a935-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a935-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a935-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a935-107">更新[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a935-107">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a935-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a935-108">Prerequisites</span></span>
<span data-ttu-id="9a935-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a935-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a935-111">Permission type</span></span>|<span data-ttu-id="9a935-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a935-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a935-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a935-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a935-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a935-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a935-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a935-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a935-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a935-116">Not supported.</span></span>|
|<span data-ttu-id="9a935-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a935-117">Application</span></span>|<span data-ttu-id="9a935-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a935-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a935-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a935-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="9a935-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a935-120">Request headers</span></span>
|<span data-ttu-id="9a935-121">标头</span><span class="sxs-lookup"><span data-stu-id="9a935-121">Header</span></span>|<span data-ttu-id="9a935-122">值</span><span class="sxs-lookup"><span data-stu-id="9a935-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a935-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a935-123">Authorization</span></span>|<span data-ttu-id="9a935-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a935-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a935-125">接受</span><span class="sxs-lookup"><span data-stu-id="9a935-125">Accept</span></span>|<span data-ttu-id="9a935-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a935-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a935-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a935-127">Request body</span></span>
<span data-ttu-id="9a935-128">在请求正文中，提供[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a935-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="9a935-129">下表显示创建[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a935-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="9a935-130">属性</span><span class="sxs-lookup"><span data-stu-id="9a935-130">Property</span></span>|<span data-ttu-id="9a935-131">类型</span><span class="sxs-lookup"><span data-stu-id="9a935-131">Type</span></span>|<span data-ttu-id="9a935-132">说明</span><span class="sxs-lookup"><span data-stu-id="9a935-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a935-133">id</span><span class="sxs-lookup"><span data-stu-id="9a935-133">id</span></span>|<span data-ttu-id="9a935-134">String</span><span class="sxs-lookup"><span data-stu-id="9a935-134">String</span></span>|<span data-ttu-id="9a935-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="9a935-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9a935-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="9a935-136">definitionId</span></span>|<span data-ttu-id="9a935-137">String</span><span class="sxs-lookup"><span data-stu-id="9a935-137">String</span></span>|<span data-ttu-id="9a935-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="9a935-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9a935-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="9a935-139">valueJson</span></span>|<span data-ttu-id="9a935-140">String</span><span class="sxs-lookup"><span data-stu-id="9a935-140">String</span></span>|<span data-ttu-id="9a935-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a935-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9a935-142">implementationId</span><span class="sxs-lookup"><span data-stu-id="9a935-142">implementationId</span></span>|<span data-ttu-id="9a935-143">String</span><span class="sxs-lookup"><span data-stu-id="9a935-143">String</span></span>|<span data-ttu-id="9a935-144">此复杂设置的所选实现的定义 ID</span><span class="sxs-lookup"><span data-stu-id="9a935-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="9a935-145">响应</span><span class="sxs-lookup"><span data-stu-id="9a935-145">Response</span></span>
<span data-ttu-id="9a935-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a935-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a935-147">示例</span><span class="sxs-lookup"><span data-stu-id="9a935-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a935-148">请求</span><span class="sxs-lookup"><span data-stu-id="9a935-148">Request</span></span>
<span data-ttu-id="9a935-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a935-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="9a935-150">响应</span><span class="sxs-lookup"><span data-stu-id="9a935-150">Response</span></span>
<span data-ttu-id="9a935-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a935-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





