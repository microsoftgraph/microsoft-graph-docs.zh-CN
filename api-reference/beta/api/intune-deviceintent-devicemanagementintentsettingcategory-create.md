---
title: 创建 deviceManagementIntentSettingCategory
description: 创建新的 deviceManagementIntentSettingCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1146c0f2fbfba38f7917f97589ce9015c8ef0741
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428125"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="50e74-103">创建 deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="50e74-103">Create deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="50e74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50e74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50e74-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50e74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50e74-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50e74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e74-107">创建新的[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50e74-107">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50e74-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="50e74-108">Prerequisites</span></span>
<span data-ttu-id="50e74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50e74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50e74-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="50e74-111">Permission type</span></span>|<span data-ttu-id="50e74-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50e74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50e74-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50e74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50e74-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50e74-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50e74-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50e74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50e74-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="50e74-116">Not supported.</span></span>|
|<span data-ttu-id="50e74-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="50e74-117">Application</span></span>|<span data-ttu-id="50e74-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50e74-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50e74-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50e74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="50e74-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="50e74-120">Request headers</span></span>
|<span data-ttu-id="50e74-121">标头</span><span class="sxs-lookup"><span data-stu-id="50e74-121">Header</span></span>|<span data-ttu-id="50e74-122">值</span><span class="sxs-lookup"><span data-stu-id="50e74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50e74-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50e74-123">Authorization</span></span>|<span data-ttu-id="50e74-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50e74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50e74-125">接受</span><span class="sxs-lookup"><span data-stu-id="50e74-125">Accept</span></span>|<span data-ttu-id="50e74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50e74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50e74-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50e74-127">Request body</span></span>
<span data-ttu-id="50e74-128">在请求正文中，提供 deviceManagementIntentSettingCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50e74-128">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="50e74-129">下表显示创建 deviceManagementIntentSettingCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50e74-129">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="50e74-130">属性</span><span class="sxs-lookup"><span data-stu-id="50e74-130">Property</span></span>|<span data-ttu-id="50e74-131">类型</span><span class="sxs-lookup"><span data-stu-id="50e74-131">Type</span></span>|<span data-ttu-id="50e74-132">说明</span><span class="sxs-lookup"><span data-stu-id="50e74-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50e74-133">id</span><span class="sxs-lookup"><span data-stu-id="50e74-133">id</span></span>|<span data-ttu-id="50e74-134">String</span><span class="sxs-lookup"><span data-stu-id="50e74-134">String</span></span>|<span data-ttu-id="50e74-135">从[DeviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)继承的类别 ID</span><span class="sxs-lookup"><span data-stu-id="50e74-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="50e74-136">displayName</span><span class="sxs-lookup"><span data-stu-id="50e74-136">displayName</span></span>|<span data-ttu-id="50e74-137">String</span><span class="sxs-lookup"><span data-stu-id="50e74-137">String</span></span>|<span data-ttu-id="50e74-138">继承自[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)的类别名称</span><span class="sxs-lookup"><span data-stu-id="50e74-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="50e74-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="50e74-139">hasRequiredSetting</span></span>|<span data-ttu-id="50e74-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e74-140">Boolean</span></span>|<span data-ttu-id="50e74-141">类别包含继承自[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)的顶级 "必需" 设置</span><span class="sxs-lookup"><span data-stu-id="50e74-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="50e74-142">响应</span><span class="sxs-lookup"><span data-stu-id="50e74-142">Response</span></span>
<span data-ttu-id="50e74-143">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50e74-143">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50e74-144">示例</span><span class="sxs-lookup"><span data-stu-id="50e74-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="50e74-145">请求</span><span class="sxs-lookup"><span data-stu-id="50e74-145">Request</span></span>
<span data-ttu-id="50e74-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50e74-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="50e74-147">响应</span><span class="sxs-lookup"><span data-stu-id="50e74-147">Response</span></span>
<span data-ttu-id="50e74-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50e74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```



