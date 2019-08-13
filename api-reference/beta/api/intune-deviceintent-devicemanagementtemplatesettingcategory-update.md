---
title: 更新 deviceManagementTemplateSettingCategory
description: 更新 deviceManagementTemplateSettingCategory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7df91d50f04ab5fc0053f0809ea381d0541366da
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313067"
---
# <a name="update-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="a2e00-103">更新 deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="a2e00-103">Update deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="a2e00-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2e00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2e00-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2e00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2e00-106">更新[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2e00-106">Update the properties of a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2e00-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2e00-107">Prerequisites</span></span>
<span data-ttu-id="a2e00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e00-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2e00-110">Permission type</span></span>|<span data-ttu-id="a2e00-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2e00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e00-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2e00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2e00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2e00-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2e00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2e00-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2e00-115">Not supported.</span></span>|
|<span data-ttu-id="a2e00-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2e00-116">Application</span></span>|<span data-ttu-id="a2e00-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e00-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2e00-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2e00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a2e00-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2e00-119">Request headers</span></span>
|<span data-ttu-id="a2e00-120">标头</span><span class="sxs-lookup"><span data-stu-id="a2e00-120">Header</span></span>|<span data-ttu-id="a2e00-121">值</span><span class="sxs-lookup"><span data-stu-id="a2e00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2e00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2e00-122">Authorization</span></span>|<span data-ttu-id="a2e00-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2e00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2e00-124">接受</span><span class="sxs-lookup"><span data-stu-id="a2e00-124">Accept</span></span>|<span data-ttu-id="a2e00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2e00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e00-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2e00-126">Request body</span></span>
<span data-ttu-id="a2e00-127">在请求正文中, 提供[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2e00-127">In the request body, supply a JSON representation for the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

<span data-ttu-id="a2e00-128">下表显示创建[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2e00-128">The following table shows the properties that are required when you create the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span></span>

|<span data-ttu-id="a2e00-129">属性</span><span class="sxs-lookup"><span data-stu-id="a2e00-129">Property</span></span>|<span data-ttu-id="a2e00-130">类型</span><span class="sxs-lookup"><span data-stu-id="a2e00-130">Type</span></span>|<span data-ttu-id="a2e00-131">说明</span><span class="sxs-lookup"><span data-stu-id="a2e00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e00-132">id</span><span class="sxs-lookup"><span data-stu-id="a2e00-132">id</span></span>|<span data-ttu-id="a2e00-133">String</span><span class="sxs-lookup"><span data-stu-id="a2e00-133">String</span></span>|<span data-ttu-id="a2e00-134">从[DeviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)继承的类别 ID</span><span class="sxs-lookup"><span data-stu-id="a2e00-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="a2e00-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a2e00-135">displayName</span></span>|<span data-ttu-id="a2e00-136">String</span><span class="sxs-lookup"><span data-stu-id="a2e00-136">String</span></span>|<span data-ttu-id="a2e00-137">继承自[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)的类别名称</span><span class="sxs-lookup"><span data-stu-id="a2e00-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a2e00-138">响应</span><span class="sxs-lookup"><span data-stu-id="a2e00-138">Response</span></span>
<span data-ttu-id="a2e00-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2e00-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2e00-140">示例</span><span class="sxs-lookup"><span data-stu-id="a2e00-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2e00-141">请求</span><span class="sxs-lookup"><span data-stu-id="a2e00-141">Request</span></span>
<span data-ttu-id="a2e00-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2e00-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a2e00-143">响应</span><span class="sxs-lookup"><span data-stu-id="a2e00-143">Response</span></span>
<span data-ttu-id="a2e00-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2e00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 170

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value"
}
```






