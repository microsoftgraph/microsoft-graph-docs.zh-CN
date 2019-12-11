---
title: 创建 deviceManagementCollectionSettingInstance
description: 创建新的 deviceManagementCollectionSettingInstance 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f576701930790461fd8865a35e61aacccb3e1cc2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946103"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="8099d-103">创建 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="8099d-103">Create deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="8099d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8099d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8099d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8099d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8099d-106">创建新的[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8099d-106">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8099d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8099d-107">Prerequisites</span></span>
<span data-ttu-id="8099d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8099d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8099d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8099d-110">Permission type</span></span>|<span data-ttu-id="8099d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8099d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8099d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8099d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8099d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8099d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8099d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8099d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8099d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8099d-115">Not supported.</span></span>|
|<span data-ttu-id="8099d-116">Application</span><span class="sxs-lookup"><span data-stu-id="8099d-116">Application</span></span>|<span data-ttu-id="8099d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8099d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8099d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8099d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8099d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8099d-119">Request headers</span></span>
|<span data-ttu-id="8099d-120">标头</span><span class="sxs-lookup"><span data-stu-id="8099d-120">Header</span></span>|<span data-ttu-id="8099d-121">值</span><span class="sxs-lookup"><span data-stu-id="8099d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8099d-122">授权</span><span class="sxs-lookup"><span data-stu-id="8099d-122">Authorization</span></span>|<span data-ttu-id="8099d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8099d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8099d-124">接受</span><span class="sxs-lookup"><span data-stu-id="8099d-124">Accept</span></span>|<span data-ttu-id="8099d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8099d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8099d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8099d-126">Request body</span></span>
<span data-ttu-id="8099d-127">在请求正文中，提供 deviceManagementCollectionSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8099d-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="8099d-128">下表显示创建 deviceManagementCollectionSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8099d-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="8099d-129">属性</span><span class="sxs-lookup"><span data-stu-id="8099d-129">Property</span></span>|<span data-ttu-id="8099d-130">类型</span><span class="sxs-lookup"><span data-stu-id="8099d-130">Type</span></span>|<span data-ttu-id="8099d-131">说明</span><span class="sxs-lookup"><span data-stu-id="8099d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8099d-132">id</span><span class="sxs-lookup"><span data-stu-id="8099d-132">id</span></span>|<span data-ttu-id="8099d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8099d-133">String</span></span>|<span data-ttu-id="8099d-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="8099d-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="8099d-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="8099d-135">definitionId</span></span>|<span data-ttu-id="8099d-136">字符串</span><span class="sxs-lookup"><span data-stu-id="8099d-136">String</span></span>|<span data-ttu-id="8099d-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="8099d-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="8099d-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="8099d-138">valueJson</span></span>|<span data-ttu-id="8099d-139">字符串</span><span class="sxs-lookup"><span data-stu-id="8099d-139">String</span></span>|<span data-ttu-id="8099d-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8099d-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8099d-141">响应</span><span class="sxs-lookup"><span data-stu-id="8099d-141">Response</span></span>
<span data-ttu-id="8099d-142">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8099d-142">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8099d-143">示例</span><span class="sxs-lookup"><span data-stu-id="8099d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8099d-144">请求</span><span class="sxs-lookup"><span data-stu-id="8099d-144">Request</span></span>
<span data-ttu-id="8099d-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8099d-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="8099d-146">响应</span><span class="sxs-lookup"><span data-stu-id="8099d-146">Response</span></span>
<span data-ttu-id="8099d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8099d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





