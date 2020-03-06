---
title: 更新 deviceManagementTemplateSettingCategory
description: 更新 deviceManagementTemplateSettingCategory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2431f0c265ab2acbfdd5efe0cfc9d3bfe4474dac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470306"
---
# <a name="update-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="35926-103">更新 deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="35926-103">Update deviceManagementTemplateSettingCategory</span></span>

<span data-ttu-id="35926-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35926-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35926-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35926-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35926-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35926-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35926-107">更新[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35926-107">Update the properties of a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35926-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="35926-108">Prerequisites</span></span>
<span data-ttu-id="35926-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35926-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="35926-111">Permission type</span></span>|<span data-ttu-id="35926-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35926-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35926-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35926-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35926-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35926-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35926-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35926-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35926-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="35926-116">Not supported.</span></span>|
|<span data-ttu-id="35926-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="35926-117">Application</span></span>|<span data-ttu-id="35926-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35926-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35926-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35926-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="35926-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="35926-120">Request headers</span></span>
|<span data-ttu-id="35926-121">标头</span><span class="sxs-lookup"><span data-stu-id="35926-121">Header</span></span>|<span data-ttu-id="35926-122">值</span><span class="sxs-lookup"><span data-stu-id="35926-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35926-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35926-123">Authorization</span></span>|<span data-ttu-id="35926-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35926-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35926-125">接受</span><span class="sxs-lookup"><span data-stu-id="35926-125">Accept</span></span>|<span data-ttu-id="35926-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35926-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35926-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="35926-127">Request body</span></span>
<span data-ttu-id="35926-128">在请求正文中，提供[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35926-128">In the request body, supply a JSON representation for the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

<span data-ttu-id="35926-129">下表显示创建[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35926-129">The following table shows the properties that are required when you create the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span></span>

|<span data-ttu-id="35926-130">属性</span><span class="sxs-lookup"><span data-stu-id="35926-130">Property</span></span>|<span data-ttu-id="35926-131">类型</span><span class="sxs-lookup"><span data-stu-id="35926-131">Type</span></span>|<span data-ttu-id="35926-132">说明</span><span class="sxs-lookup"><span data-stu-id="35926-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35926-133">id</span><span class="sxs-lookup"><span data-stu-id="35926-133">id</span></span>|<span data-ttu-id="35926-134">字符串</span><span class="sxs-lookup"><span data-stu-id="35926-134">String</span></span>|<span data-ttu-id="35926-135">从[DeviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)继承的类别 ID</span><span class="sxs-lookup"><span data-stu-id="35926-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="35926-136">displayName</span><span class="sxs-lookup"><span data-stu-id="35926-136">displayName</span></span>|<span data-ttu-id="35926-137">String</span><span class="sxs-lookup"><span data-stu-id="35926-137">String</span></span>|<span data-ttu-id="35926-138">继承自[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)的类别名称</span><span class="sxs-lookup"><span data-stu-id="35926-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="35926-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="35926-139">hasRequiredSetting</span></span>|<span data-ttu-id="35926-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="35926-140">Boolean</span></span>|<span data-ttu-id="35926-141">类别包含继承自[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)的顶级 "必需" 设置</span><span class="sxs-lookup"><span data-stu-id="35926-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="35926-142">响应</span><span class="sxs-lookup"><span data-stu-id="35926-142">Response</span></span>
<span data-ttu-id="35926-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35926-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35926-144">示例</span><span class="sxs-lookup"><span data-stu-id="35926-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="35926-145">请求</span><span class="sxs-lookup"><span data-stu-id="35926-145">Request</span></span>
<span data-ttu-id="35926-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35926-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="35926-147">响应</span><span class="sxs-lookup"><span data-stu-id="35926-147">Response</span></span>
<span data-ttu-id="35926-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35926-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 201

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```





