---
title: 创建 deviceManagementSettingCategory
description: 创建新的 deviceManagementSettingCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c889962597896fefc5a2be03a44bc4121d5a7fb5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203577"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="ffa3f-103">创建 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ffa3f-103">Create deviceManagementSettingCategory</span></span>

<span data-ttu-id="ffa3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffa3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffa3f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffa3f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffa3f-107">创建新的 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-107">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffa3f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffa3f-108">Prerequisites</span></span>
<span data-ttu-id="ffa3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffa3f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffa3f-111">Permission type</span></span>|<span data-ttu-id="ffa3f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffa3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffa3f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffa3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffa3f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffa3f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffa3f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffa3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffa3f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-116">Not supported.</span></span>|
|<span data-ttu-id="ffa3f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffa3f-117">Application</span></span>|<span data-ttu-id="ffa3f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffa3f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffa3f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffa3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="ffa3f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffa3f-120">Request headers</span></span>
|<span data-ttu-id="ffa3f-121">标头</span><span class="sxs-lookup"><span data-stu-id="ffa3f-121">Header</span></span>|<span data-ttu-id="ffa3f-122">值</span><span class="sxs-lookup"><span data-stu-id="ffa3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffa3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffa3f-123">Authorization</span></span>|<span data-ttu-id="ffa3f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffa3f-125">接受</span><span class="sxs-lookup"><span data-stu-id="ffa3f-125">Accept</span></span>|<span data-ttu-id="ffa3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffa3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffa3f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffa3f-127">Request body</span></span>
<span data-ttu-id="ffa3f-128">在请求正文中，提供 deviceManagementSettingCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-128">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="ffa3f-129">下表显示创建 deviceManagementSettingCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-129">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="ffa3f-130">属性</span><span class="sxs-lookup"><span data-stu-id="ffa3f-130">Property</span></span>|<span data-ttu-id="ffa3f-131">类型</span><span class="sxs-lookup"><span data-stu-id="ffa3f-131">Type</span></span>|<span data-ttu-id="ffa3f-132">说明</span><span class="sxs-lookup"><span data-stu-id="ffa3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffa3f-133">id</span><span class="sxs-lookup"><span data-stu-id="ffa3f-133">id</span></span>|<span data-ttu-id="ffa3f-134">String</span><span class="sxs-lookup"><span data-stu-id="ffa3f-134">String</span></span>|<span data-ttu-id="ffa3f-135">类别 ID</span><span class="sxs-lookup"><span data-stu-id="ffa3f-135">The category ID</span></span>|
|<span data-ttu-id="ffa3f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ffa3f-136">displayName</span></span>|<span data-ttu-id="ffa3f-137">String</span><span class="sxs-lookup"><span data-stu-id="ffa3f-137">String</span></span>|<span data-ttu-id="ffa3f-138">类别名称</span><span class="sxs-lookup"><span data-stu-id="ffa3f-138">The category name</span></span>|
|<span data-ttu-id="ffa3f-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="ffa3f-139">hasRequiredSetting</span></span>|<span data-ttu-id="ffa3f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffa3f-140">Boolean</span></span>|<span data-ttu-id="ffa3f-141">类别包含 "必需顶级" 设置</span><span class="sxs-lookup"><span data-stu-id="ffa3f-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="ffa3f-142">响应</span><span class="sxs-lookup"><span data-stu-id="ffa3f-142">Response</span></span>
<span data-ttu-id="ffa3f-143">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-143">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffa3f-144">示例</span><span class="sxs-lookup"><span data-stu-id="ffa3f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffa3f-145">请求</span><span class="sxs-lookup"><span data-stu-id="ffa3f-145">Request</span></span>
<span data-ttu-id="ffa3f-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/categories
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="ffa3f-147">响应</span><span class="sxs-lookup"><span data-stu-id="ffa3f-147">Response</span></span>
<span data-ttu-id="ffa3f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffa3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




