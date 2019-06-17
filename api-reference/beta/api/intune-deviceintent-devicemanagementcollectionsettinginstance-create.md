---
title: 创建 deviceManagementCollectionSettingInstance
description: 创建新的 deviceManagementCollectionSettingInstance 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25e120ebc5050be5a84c94879ac6586977a4d2dd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960837"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="4f056-103">创建 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="4f056-103">Create deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="4f056-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f056-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f056-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f056-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f056-106">创建新的[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4f056-106">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f056-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f056-107">Prerequisites</span></span>
<span data-ttu-id="4f056-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f056-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f056-110">Permission type</span></span>|<span data-ttu-id="4f056-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4f056-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f056-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f056-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f056-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f056-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f056-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f056-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f056-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f056-115">Not supported.</span></span>|
|<span data-ttu-id="4f056-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f056-116">Application</span></span>|<span data-ttu-id="4f056-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f056-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f056-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f056-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4f056-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f056-119">Request headers</span></span>
|<span data-ttu-id="4f056-120">标头</span><span class="sxs-lookup"><span data-stu-id="4f056-120">Header</span></span>|<span data-ttu-id="4f056-121">值</span><span class="sxs-lookup"><span data-stu-id="4f056-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f056-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f056-122">Authorization</span></span>|<span data-ttu-id="4f056-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4f056-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f056-124">接受</span><span class="sxs-lookup"><span data-stu-id="4f056-124">Accept</span></span>|<span data-ttu-id="4f056-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f056-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f056-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f056-126">Request body</span></span>
<span data-ttu-id="4f056-127">在请求正文中, 提供 deviceManagementCollectionSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f056-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="4f056-128">下表显示创建 deviceManagementCollectionSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4f056-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="4f056-129">属性</span><span class="sxs-lookup"><span data-stu-id="4f056-129">Property</span></span>|<span data-ttu-id="4f056-130">类型</span><span class="sxs-lookup"><span data-stu-id="4f056-130">Type</span></span>|<span data-ttu-id="4f056-131">说明</span><span class="sxs-lookup"><span data-stu-id="4f056-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f056-132">id</span><span class="sxs-lookup"><span data-stu-id="4f056-132">id</span></span>|<span data-ttu-id="4f056-133">String</span><span class="sxs-lookup"><span data-stu-id="4f056-133">String</span></span>|<span data-ttu-id="4f056-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="4f056-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4f056-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="4f056-135">definitionId</span></span>|<span data-ttu-id="4f056-136">String</span><span class="sxs-lookup"><span data-stu-id="4f056-136">String</span></span>|<span data-ttu-id="4f056-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="4f056-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4f056-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="4f056-138">valueJson</span></span>|<span data-ttu-id="4f056-139">String</span><span class="sxs-lookup"><span data-stu-id="4f056-139">String</span></span>|<span data-ttu-id="4f056-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f056-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4f056-141">响应</span><span class="sxs-lookup"><span data-stu-id="4f056-141">Response</span></span>
<span data-ttu-id="4f056-142">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4f056-142">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f056-143">示例</span><span class="sxs-lookup"><span data-stu-id="4f056-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f056-144">请求</span><span class="sxs-lookup"><span data-stu-id="4f056-144">Request</span></span>
<span data-ttu-id="4f056-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f056-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f056-146">响应</span><span class="sxs-lookup"><span data-stu-id="4f056-146">Response</span></span>
<span data-ttu-id="4f056-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f056-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





