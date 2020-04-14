---
title: 更新 deviceManagementSettingCategory
description: 更新 deviceManagementSettingCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd4e412d8793e8fd2999a72643ab28aec1fc32b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427829"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="c953d-103">更新 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c953d-103">Update deviceManagementSettingCategory</span></span>

<span data-ttu-id="c953d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c953d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c953d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c953d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c953d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c953d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c953d-107">更新[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c953d-107">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c953d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c953d-108">Prerequisites</span></span>
<span data-ttu-id="c953d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c953d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c953d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c953d-111">Permission type</span></span>|<span data-ttu-id="c953d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c953d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c953d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c953d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c953d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c953d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c953d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c953d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c953d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c953d-116">Not supported.</span></span>|
|<span data-ttu-id="c953d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c953d-117">Application</span></span>|<span data-ttu-id="c953d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c953d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c953d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c953d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="c953d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c953d-120">Request headers</span></span>
|<span data-ttu-id="c953d-121">标头</span><span class="sxs-lookup"><span data-stu-id="c953d-121">Header</span></span>|<span data-ttu-id="c953d-122">值</span><span class="sxs-lookup"><span data-stu-id="c953d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c953d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c953d-123">Authorization</span></span>|<span data-ttu-id="c953d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c953d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c953d-125">接受</span><span class="sxs-lookup"><span data-stu-id="c953d-125">Accept</span></span>|<span data-ttu-id="c953d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c953d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c953d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c953d-127">Request body</span></span>
<span data-ttu-id="c953d-128">在请求正文中，提供[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c953d-128">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="c953d-129">下表显示创建[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c953d-129">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="c953d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c953d-130">Property</span></span>|<span data-ttu-id="c953d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c953d-131">Type</span></span>|<span data-ttu-id="c953d-132">说明</span><span class="sxs-lookup"><span data-stu-id="c953d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c953d-133">id</span><span class="sxs-lookup"><span data-stu-id="c953d-133">id</span></span>|<span data-ttu-id="c953d-134">String</span><span class="sxs-lookup"><span data-stu-id="c953d-134">String</span></span>|<span data-ttu-id="c953d-135">类别 ID</span><span class="sxs-lookup"><span data-stu-id="c953d-135">The category ID</span></span>|
|<span data-ttu-id="c953d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c953d-136">displayName</span></span>|<span data-ttu-id="c953d-137">String</span><span class="sxs-lookup"><span data-stu-id="c953d-137">String</span></span>|<span data-ttu-id="c953d-138">类别名称</span><span class="sxs-lookup"><span data-stu-id="c953d-138">The category name</span></span>|
|<span data-ttu-id="c953d-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="c953d-139">hasRequiredSetting</span></span>|<span data-ttu-id="c953d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c953d-140">Boolean</span></span>|<span data-ttu-id="c953d-141">类别包含 "必需顶级" 设置</span><span class="sxs-lookup"><span data-stu-id="c953d-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="c953d-142">响应</span><span class="sxs-lookup"><span data-stu-id="c953d-142">Response</span></span>
<span data-ttu-id="c953d-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c953d-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c953d-144">示例</span><span class="sxs-lookup"><span data-stu-id="c953d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c953d-145">请求</span><span class="sxs-lookup"><span data-stu-id="c953d-145">Request</span></span>
<span data-ttu-id="c953d-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c953d-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c953d-147">响应</span><span class="sxs-lookup"><span data-stu-id="c953d-147">Response</span></span>
<span data-ttu-id="c953d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c953d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



