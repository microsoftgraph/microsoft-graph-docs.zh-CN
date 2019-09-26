---
title: 更新 deviceManagementSettingCategory
description: 更新 deviceManagementSettingCategory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a202fc1eaaf31bd84f907f1bec392e90f79bbf6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180739"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="d7962-103">更新 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="d7962-103">Update deviceManagementSettingCategory</span></span>

> <span data-ttu-id="d7962-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7962-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7962-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7962-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7962-106">更新[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d7962-106">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7962-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d7962-107">Prerequisites</span></span>
<span data-ttu-id="d7962-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7962-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7962-110">Permission type</span></span>|<span data-ttu-id="d7962-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d7962-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7962-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7962-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7962-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7962-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7962-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7962-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7962-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7962-115">Not supported.</span></span>|
|<span data-ttu-id="d7962-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7962-116">Application</span></span>|<span data-ttu-id="d7962-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7962-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7962-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7962-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="d7962-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7962-119">Request headers</span></span>
|<span data-ttu-id="d7962-120">标头</span><span class="sxs-lookup"><span data-stu-id="d7962-120">Header</span></span>|<span data-ttu-id="d7962-121">值</span><span class="sxs-lookup"><span data-stu-id="d7962-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7962-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7962-122">Authorization</span></span>|<span data-ttu-id="d7962-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d7962-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7962-124">接受</span><span class="sxs-lookup"><span data-stu-id="d7962-124">Accept</span></span>|<span data-ttu-id="d7962-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7962-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7962-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7962-126">Request body</span></span>
<span data-ttu-id="d7962-127">在请求正文中，提供[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7962-127">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="d7962-128">下表显示创建[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d7962-128">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="d7962-129">属性</span><span class="sxs-lookup"><span data-stu-id="d7962-129">Property</span></span>|<span data-ttu-id="d7962-130">类型</span><span class="sxs-lookup"><span data-stu-id="d7962-130">Type</span></span>|<span data-ttu-id="d7962-131">说明</span><span class="sxs-lookup"><span data-stu-id="d7962-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7962-132">id</span><span class="sxs-lookup"><span data-stu-id="d7962-132">id</span></span>|<span data-ttu-id="d7962-133">String</span><span class="sxs-lookup"><span data-stu-id="d7962-133">String</span></span>|<span data-ttu-id="d7962-134">类别 ID</span><span class="sxs-lookup"><span data-stu-id="d7962-134">The category ID</span></span>|
|<span data-ttu-id="d7962-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d7962-135">displayName</span></span>|<span data-ttu-id="d7962-136">String</span><span class="sxs-lookup"><span data-stu-id="d7962-136">String</span></span>|<span data-ttu-id="d7962-137">类别名称</span><span class="sxs-lookup"><span data-stu-id="d7962-137">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="d7962-138">响应</span><span class="sxs-lookup"><span data-stu-id="d7962-138">Response</span></span>
<span data-ttu-id="d7962-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7962-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7962-140">示例</span><span class="sxs-lookup"><span data-stu-id="d7962-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7962-141">请求</span><span class="sxs-lookup"><span data-stu-id="d7962-141">Request</span></span>
<span data-ttu-id="d7962-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7962-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d7962-143">响应</span><span class="sxs-lookup"><span data-stu-id="d7962-143">Response</span></span>
<span data-ttu-id="d7962-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7962-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value"
}
```




