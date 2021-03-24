---
title: 更新 deviceManagementIntentSettingCategory
description: 更新 deviceManagementIntentSettingCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d74309de7de867267a9cfc9abaaf31ff360175d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130915"
---
# <a name="update-devicemanagementintentsettingcategory"></a><span data-ttu-id="4f068-103">更新 deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="4f068-103">Update deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="4f068-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f068-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f068-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f068-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f068-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f068-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f068-107">更新 [deviceManagementIntentSettingCategory 对象](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4f068-107">Update the properties of a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f068-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f068-108">Prerequisites</span></span>
<span data-ttu-id="4f068-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f068-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f068-111">Permission type</span></span>|<span data-ttu-id="4f068-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f068-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f068-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f068-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f068-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f068-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f068-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f068-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f068-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f068-116">Not supported.</span></span>|
|<span data-ttu-id="4f068-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f068-117">Application</span></span>|<span data-ttu-id="4f068-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f068-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f068-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f068-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="4f068-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f068-120">Request headers</span></span>
|<span data-ttu-id="4f068-121">标头</span><span class="sxs-lookup"><span data-stu-id="4f068-121">Header</span></span>|<span data-ttu-id="4f068-122">值</span><span class="sxs-lookup"><span data-stu-id="4f068-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f068-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f068-123">Authorization</span></span>|<span data-ttu-id="4f068-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4f068-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f068-125">接受</span><span class="sxs-lookup"><span data-stu-id="4f068-125">Accept</span></span>|<span data-ttu-id="4f068-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f068-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f068-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f068-127">Request body</span></span>
<span data-ttu-id="4f068-128">在请求正文中，提供 [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f068-128">In the request body, supply a JSON representation for the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

<span data-ttu-id="4f068-129">下表显示创建 [deviceManagementIntentSettingCategory 时所需的属性](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="4f068-129">The following table shows the properties that are required when you create the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>

|<span data-ttu-id="4f068-130">属性</span><span class="sxs-lookup"><span data-stu-id="4f068-130">Property</span></span>|<span data-ttu-id="4f068-131">类型</span><span class="sxs-lookup"><span data-stu-id="4f068-131">Type</span></span>|<span data-ttu-id="4f068-132">说明</span><span class="sxs-lookup"><span data-stu-id="4f068-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f068-133">id</span><span class="sxs-lookup"><span data-stu-id="4f068-133">id</span></span>|<span data-ttu-id="4f068-134">String</span><span class="sxs-lookup"><span data-stu-id="4f068-134">String</span></span>|<span data-ttu-id="4f068-135">类别 ID 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4f068-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="4f068-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4f068-136">displayName</span></span>|<span data-ttu-id="4f068-137">String</span><span class="sxs-lookup"><span data-stu-id="4f068-137">String</span></span>|<span data-ttu-id="4f068-138">类别名称 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4f068-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="4f068-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="4f068-139">hasRequiredSetting</span></span>|<span data-ttu-id="4f068-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f068-140">Boolean</span></span>|<span data-ttu-id="4f068-141">类别包含顶级所需设置 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4f068-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4f068-142">响应</span><span class="sxs-lookup"><span data-stu-id="4f068-142">Response</span></span>
<span data-ttu-id="4f068-143">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f068-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f068-144">示例</span><span class="sxs-lookup"><span data-stu-id="4f068-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f068-145">请求</span><span class="sxs-lookup"><span data-stu-id="4f068-145">Request</span></span>
<span data-ttu-id="4f068-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f068-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="4f068-147">响应</span><span class="sxs-lookup"><span data-stu-id="4f068-147">Response</span></span>
<span data-ttu-id="4f068-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f068-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




