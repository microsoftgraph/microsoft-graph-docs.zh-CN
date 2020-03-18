---
title: 更新 deviceManagementSettingCategory
description: 更新 deviceManagementSettingCategory 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4e5711e8d9adf026e94b85c01c0d7e384ce677c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815105"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="2c04f-103">更新 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="2c04f-103">Update deviceManagementSettingCategory</span></span>

> <span data-ttu-id="2c04f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c04f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c04f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c04f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c04f-106">更新[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c04f-106">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c04f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c04f-107">Prerequisites</span></span>
<span data-ttu-id="2c04f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c04f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c04f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c04f-110">Permission type</span></span>|<span data-ttu-id="2c04f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c04f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c04f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c04f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c04f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c04f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c04f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c04f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c04f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c04f-115">Not supported.</span></span>|
|<span data-ttu-id="2c04f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c04f-116">Application</span></span>|<span data-ttu-id="2c04f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c04f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c04f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c04f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="2c04f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c04f-119">Request headers</span></span>
|<span data-ttu-id="2c04f-120">标头</span><span class="sxs-lookup"><span data-stu-id="2c04f-120">Header</span></span>|<span data-ttu-id="2c04f-121">值</span><span class="sxs-lookup"><span data-stu-id="2c04f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c04f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c04f-122">Authorization</span></span>|<span data-ttu-id="2c04f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c04f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c04f-124">接受</span><span class="sxs-lookup"><span data-stu-id="2c04f-124">Accept</span></span>|<span data-ttu-id="2c04f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c04f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c04f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c04f-126">Request body</span></span>
<span data-ttu-id="2c04f-127">在请求正文中，提供[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c04f-127">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="2c04f-128">下表显示创建[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c04f-128">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="2c04f-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c04f-129">Property</span></span>|<span data-ttu-id="2c04f-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c04f-130">Type</span></span>|<span data-ttu-id="2c04f-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c04f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c04f-132">id</span><span class="sxs-lookup"><span data-stu-id="2c04f-132">id</span></span>|<span data-ttu-id="2c04f-133">String</span><span class="sxs-lookup"><span data-stu-id="2c04f-133">String</span></span>|<span data-ttu-id="2c04f-134">类别 ID</span><span class="sxs-lookup"><span data-stu-id="2c04f-134">The category ID</span></span>|
|<span data-ttu-id="2c04f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2c04f-135">displayName</span></span>|<span data-ttu-id="2c04f-136">String</span><span class="sxs-lookup"><span data-stu-id="2c04f-136">String</span></span>|<span data-ttu-id="2c04f-137">类别名称</span><span class="sxs-lookup"><span data-stu-id="2c04f-137">The category name</span></span>|
|<span data-ttu-id="2c04f-138">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="2c04f-138">hasRequiredSetting</span></span>|<span data-ttu-id="2c04f-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="2c04f-139">Boolean</span></span>|<span data-ttu-id="2c04f-140">类别包含 "必需顶级" 设置</span><span class="sxs-lookup"><span data-stu-id="2c04f-140">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="2c04f-141">响应</span><span class="sxs-lookup"><span data-stu-id="2c04f-141">Response</span></span>
<span data-ttu-id="2c04f-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c04f-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c04f-143">示例</span><span class="sxs-lookup"><span data-stu-id="2c04f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c04f-144">请求</span><span class="sxs-lookup"><span data-stu-id="2c04f-144">Request</span></span>
<span data-ttu-id="2c04f-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c04f-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="2c04f-146">响应</span><span class="sxs-lookup"><span data-stu-id="2c04f-146">Response</span></span>
<span data-ttu-id="2c04f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c04f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




