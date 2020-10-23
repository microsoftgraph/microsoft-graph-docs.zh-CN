---
title: 创建 deviceManagementCollectionSettingInstance
description: 创建新的 deviceManagementCollectionSettingInstance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 302e34f3e191688f9d6ad88b723f924f170ae07a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708261"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="a0235-103">创建 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="a0235-103">Create deviceManagementCollectionSettingInstance</span></span>

<span data-ttu-id="a0235-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0235-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0235-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0235-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0235-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0235-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0235-107">创建新的 [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0235-107">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0235-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0235-108">Prerequisites</span></span>
<span data-ttu-id="a0235-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0235-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0235-111">Permission type</span></span>|<span data-ttu-id="a0235-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a0235-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0235-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0235-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0235-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0235-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0235-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0235-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0235-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0235-116">Not supported.</span></span>|
|<span data-ttu-id="a0235-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0235-117">Application</span></span>|<span data-ttu-id="a0235-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0235-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0235-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0235-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a0235-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0235-120">Request headers</span></span>
|<span data-ttu-id="a0235-121">标头</span><span class="sxs-lookup"><span data-stu-id="a0235-121">Header</span></span>|<span data-ttu-id="a0235-122">值</span><span class="sxs-lookup"><span data-stu-id="a0235-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0235-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0235-123">Authorization</span></span>|<span data-ttu-id="a0235-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0235-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0235-125">接受</span><span class="sxs-lookup"><span data-stu-id="a0235-125">Accept</span></span>|<span data-ttu-id="a0235-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0235-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0235-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0235-127">Request body</span></span>
<span data-ttu-id="a0235-128">在请求正文中，提供 deviceManagementCollectionSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0235-128">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="a0235-129">下表显示创建 deviceManagementCollectionSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a0235-129">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="a0235-130">属性</span><span class="sxs-lookup"><span data-stu-id="a0235-130">Property</span></span>|<span data-ttu-id="a0235-131">类型</span><span class="sxs-lookup"><span data-stu-id="a0235-131">Type</span></span>|<span data-ttu-id="a0235-132">说明</span><span class="sxs-lookup"><span data-stu-id="a0235-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0235-133">id</span><span class="sxs-lookup"><span data-stu-id="a0235-133">id</span></span>|<span data-ttu-id="a0235-134">String</span><span class="sxs-lookup"><span data-stu-id="a0235-134">String</span></span>|<span data-ttu-id="a0235-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="a0235-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="a0235-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="a0235-136">definitionId</span></span>|<span data-ttu-id="a0235-137">String</span><span class="sxs-lookup"><span data-stu-id="a0235-137">String</span></span>|<span data-ttu-id="a0235-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="a0235-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="a0235-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="a0235-139">valueJson</span></span>|<span data-ttu-id="a0235-140">String</span><span class="sxs-lookup"><span data-stu-id="a0235-140">String</span></span>|<span data-ttu-id="a0235-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0235-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a0235-142">响应</span><span class="sxs-lookup"><span data-stu-id="a0235-142">Response</span></span>
<span data-ttu-id="a0235-143">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0235-143">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0235-144">示例</span><span class="sxs-lookup"><span data-stu-id="a0235-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0235-145">请求</span><span class="sxs-lookup"><span data-stu-id="a0235-145">Request</span></span>
<span data-ttu-id="a0235-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0235-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0235-147">响应</span><span class="sxs-lookup"><span data-stu-id="a0235-147">Response</span></span>
<span data-ttu-id="a0235-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0235-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





