---
title: 更新 deviceManagementTemplateSettingCategory
description: 更新 deviceManagementTemplateSettingCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c221216f0471823a8db315cfef0340fd994e6521
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150673"
---
# <a name="update-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="b9743-103">更新 deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="b9743-103">Update deviceManagementTemplateSettingCategory</span></span>

<span data-ttu-id="b9743-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9743-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9743-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9743-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9743-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9743-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9743-107">更新 [deviceManagementTemplateSettingCategory 对象](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b9743-107">Update the properties of a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9743-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9743-108">Prerequisites</span></span>
<span data-ttu-id="b9743-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9743-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9743-111">Permission type</span></span>|<span data-ttu-id="b9743-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9743-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9743-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9743-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9743-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9743-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9743-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9743-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9743-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9743-116">Not supported.</span></span>|
|<span data-ttu-id="b9743-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9743-117">Application</span></span>|<span data-ttu-id="b9743-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9743-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9743-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9743-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="b9743-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9743-120">Request headers</span></span>
|<span data-ttu-id="b9743-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9743-121">Header</span></span>|<span data-ttu-id="b9743-122">值</span><span class="sxs-lookup"><span data-stu-id="b9743-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9743-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9743-123">Authorization</span></span>|<span data-ttu-id="b9743-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9743-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9743-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9743-125">Accept</span></span>|<span data-ttu-id="b9743-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9743-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9743-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9743-127">Request body</span></span>
<span data-ttu-id="b9743-128">在请求正文中，提供 [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9743-128">In the request body, supply a JSON representation for the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

<span data-ttu-id="b9743-129">下表显示创建 [deviceManagementTemplateSettingCategory 时所需的属性](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="b9743-129">The following table shows the properties that are required when you create the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span></span>

|<span data-ttu-id="b9743-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9743-130">Property</span></span>|<span data-ttu-id="b9743-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9743-131">Type</span></span>|<span data-ttu-id="b9743-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9743-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9743-133">id</span><span class="sxs-lookup"><span data-stu-id="b9743-133">id</span></span>|<span data-ttu-id="b9743-134">String</span><span class="sxs-lookup"><span data-stu-id="b9743-134">String</span></span>|<span data-ttu-id="b9743-135">类别 ID 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b9743-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="b9743-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b9743-136">displayName</span></span>|<span data-ttu-id="b9743-137">String</span><span class="sxs-lookup"><span data-stu-id="b9743-137">String</span></span>|<span data-ttu-id="b9743-138">类别名称 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b9743-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="b9743-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="b9743-139">hasRequiredSetting</span></span>|<span data-ttu-id="b9743-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9743-140">Boolean</span></span>|<span data-ttu-id="b9743-141">类别包含顶级所需设置 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b9743-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b9743-142">响应</span><span class="sxs-lookup"><span data-stu-id="b9743-142">Response</span></span>
<span data-ttu-id="b9743-143">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9743-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9743-144">示例</span><span class="sxs-lookup"><span data-stu-id="b9743-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9743-145">请求</span><span class="sxs-lookup"><span data-stu-id="b9743-145">Request</span></span>
<span data-ttu-id="b9743-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9743-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9743-147">响应</span><span class="sxs-lookup"><span data-stu-id="b9743-147">Response</span></span>
<span data-ttu-id="b9743-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9743-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




