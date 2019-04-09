---
title: 创建 deviceManagementCollectionSettingInstance
description: 创建新的 deviceManagementCollectionSettingInstance 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df6d4c9e0aff1a3b66d651d076f89c6fc7eae27b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524216"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="c224a-103">创建 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="c224a-103">Create deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="c224a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c224a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c224a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c224a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c224a-106">创建新的[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c224a-106">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c224a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c224a-107">Prerequisites</span></span>
<span data-ttu-id="c224a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c224a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c224a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c224a-110">Permission type</span></span>|<span data-ttu-id="c224a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c224a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c224a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c224a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c224a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c224a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c224a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c224a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c224a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c224a-115">Not supported.</span></span>|
|<span data-ttu-id="c224a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c224a-116">Application</span></span>|<span data-ttu-id="c224a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c224a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c224a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c224a-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c224a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c224a-119">Request headers</span></span>
|<span data-ttu-id="c224a-120">标头</span><span class="sxs-lookup"><span data-stu-id="c224a-120">Header</span></span>|<span data-ttu-id="c224a-121">值</span><span class="sxs-lookup"><span data-stu-id="c224a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c224a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c224a-122">Authorization</span></span>|<span data-ttu-id="c224a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c224a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c224a-124">接受</span><span class="sxs-lookup"><span data-stu-id="c224a-124">Accept</span></span>|<span data-ttu-id="c224a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c224a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c224a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c224a-126">Request body</span></span>
<span data-ttu-id="c224a-127">在请求正文中, 提供 deviceManagementCollectionSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c224a-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="c224a-128">下表显示创建 deviceManagementCollectionSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c224a-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="c224a-129">属性</span><span class="sxs-lookup"><span data-stu-id="c224a-129">Property</span></span>|<span data-ttu-id="c224a-130">类型</span><span class="sxs-lookup"><span data-stu-id="c224a-130">Type</span></span>|<span data-ttu-id="c224a-131">说明</span><span class="sxs-lookup"><span data-stu-id="c224a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c224a-132">id</span><span class="sxs-lookup"><span data-stu-id="c224a-132">id</span></span>|<span data-ttu-id="c224a-133">String</span><span class="sxs-lookup"><span data-stu-id="c224a-133">String</span></span>|<span data-ttu-id="c224a-134">从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="c224a-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c224a-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="c224a-135">definitionId</span></span>|<span data-ttu-id="c224a-136">String</span><span class="sxs-lookup"><span data-stu-id="c224a-136">String</span></span>|<span data-ttu-id="c224a-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="c224a-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c224a-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="c224a-138">valueJson</span></span>|<span data-ttu-id="c224a-139">String</span><span class="sxs-lookup"><span data-stu-id="c224a-139">String</span></span>|<span data-ttu-id="c224a-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c224a-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c224a-141">响应</span><span class="sxs-lookup"><span data-stu-id="c224a-141">Response</span></span>
<span data-ttu-id="c224a-142">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c224a-142">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c224a-143">示例</span><span class="sxs-lookup"><span data-stu-id="c224a-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c224a-144">请求</span><span class="sxs-lookup"><span data-stu-id="c224a-144">Request</span></span>
<span data-ttu-id="c224a-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c224a-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c224a-146">响应</span><span class="sxs-lookup"><span data-stu-id="c224a-146">Response</span></span>
<span data-ttu-id="c224a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c224a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







