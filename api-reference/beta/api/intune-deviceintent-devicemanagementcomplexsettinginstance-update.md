---
title: 更新 deviceManagementComplexSettingInstance
description: 更新 deviceManagementComplexSettingInstance 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d88733bbd1dbfb8950e26dc9ca68c204f647221b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945976"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="0cfcc-103">更新 deviceManagementComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="0cfcc-103">Update deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="0cfcc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cfcc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cfcc-106">更新[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-106">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cfcc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0cfcc-107">Prerequisites</span></span>
<span data-ttu-id="0cfcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cfcc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cfcc-110">Permission type</span></span>|<span data-ttu-id="0cfcc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0cfcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cfcc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cfcc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cfcc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cfcc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cfcc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cfcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cfcc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-115">Not supported.</span></span>|
|<span data-ttu-id="0cfcc-116">Application</span><span class="sxs-lookup"><span data-stu-id="0cfcc-116">Application</span></span>|<span data-ttu-id="0cfcc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cfcc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cfcc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cfcc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0cfcc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cfcc-119">Request headers</span></span>
|<span data-ttu-id="0cfcc-120">标头</span><span class="sxs-lookup"><span data-stu-id="0cfcc-120">Header</span></span>|<span data-ttu-id="0cfcc-121">值</span><span class="sxs-lookup"><span data-stu-id="0cfcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cfcc-122">授权</span><span class="sxs-lookup"><span data-stu-id="0cfcc-122">Authorization</span></span>|<span data-ttu-id="0cfcc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cfcc-124">接受</span><span class="sxs-lookup"><span data-stu-id="0cfcc-124">Accept</span></span>|<span data-ttu-id="0cfcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cfcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cfcc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cfcc-126">Request body</span></span>
<span data-ttu-id="0cfcc-127">在请求正文中，提供[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="0cfcc-128">下表显示创建[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="0cfcc-129">属性</span><span class="sxs-lookup"><span data-stu-id="0cfcc-129">Property</span></span>|<span data-ttu-id="0cfcc-130">类型</span><span class="sxs-lookup"><span data-stu-id="0cfcc-130">Type</span></span>|<span data-ttu-id="0cfcc-131">说明</span><span class="sxs-lookup"><span data-stu-id="0cfcc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cfcc-132">id</span><span class="sxs-lookup"><span data-stu-id="0cfcc-132">id</span></span>|<span data-ttu-id="0cfcc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0cfcc-133">String</span></span>|<span data-ttu-id="0cfcc-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="0cfcc-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="0cfcc-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="0cfcc-135">definitionId</span></span>|<span data-ttu-id="0cfcc-136">字符串</span><span class="sxs-lookup"><span data-stu-id="0cfcc-136">String</span></span>|<span data-ttu-id="0cfcc-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="0cfcc-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="0cfcc-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="0cfcc-138">valueJson</span></span>|<span data-ttu-id="0cfcc-139">字符串</span><span class="sxs-lookup"><span data-stu-id="0cfcc-139">String</span></span>|<span data-ttu-id="0cfcc-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0cfcc-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0cfcc-141">响应</span><span class="sxs-lookup"><span data-stu-id="0cfcc-141">Response</span></span>
<span data-ttu-id="0cfcc-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cfcc-143">示例</span><span class="sxs-lookup"><span data-stu-id="0cfcc-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cfcc-144">请求</span><span class="sxs-lookup"><span data-stu-id="0cfcc-144">Request</span></span>
<span data-ttu-id="0cfcc-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="0cfcc-146">响应</span><span class="sxs-lookup"><span data-stu-id="0cfcc-146">Response</span></span>
<span data-ttu-id="0cfcc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0cfcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





