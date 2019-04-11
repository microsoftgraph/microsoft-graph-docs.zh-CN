---
title: 创建 deviceManagementIntentSettingCategory
description: 创建新的 deviceManagementIntentSettingCategory 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: add0d92a29f2bf2d29176e0d22dc68f7deb19a18
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776617"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="7caa0-103">创建 deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="7caa0-103">Create deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="7caa0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7caa0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7caa0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7caa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7caa0-106">创建新的[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7caa0-106">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7caa0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7caa0-107">Prerequisites</span></span>
<span data-ttu-id="7caa0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7caa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7caa0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7caa0-110">Permission type</span></span>|<span data-ttu-id="7caa0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7caa0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7caa0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7caa0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7caa0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7caa0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7caa0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7caa0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7caa0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7caa0-115">Not supported.</span></span>|
|<span data-ttu-id="7caa0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7caa0-116">Application</span></span>|<span data-ttu-id="7caa0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7caa0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7caa0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7caa0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="7caa0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7caa0-119">Request headers</span></span>
|<span data-ttu-id="7caa0-120">标头</span><span class="sxs-lookup"><span data-stu-id="7caa0-120">Header</span></span>|<span data-ttu-id="7caa0-121">值</span><span class="sxs-lookup"><span data-stu-id="7caa0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7caa0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7caa0-122">Authorization</span></span>|<span data-ttu-id="7caa0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7caa0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7caa0-124">接受</span><span class="sxs-lookup"><span data-stu-id="7caa0-124">Accept</span></span>|<span data-ttu-id="7caa0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7caa0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7caa0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7caa0-126">Request body</span></span>
<span data-ttu-id="7caa0-127">在请求正文中, 提供 deviceManagementIntentSettingCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7caa0-127">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="7caa0-128">下表显示创建 deviceManagementIntentSettingCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7caa0-128">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="7caa0-129">属性</span><span class="sxs-lookup"><span data-stu-id="7caa0-129">Property</span></span>|<span data-ttu-id="7caa0-130">类型</span><span class="sxs-lookup"><span data-stu-id="7caa0-130">Type</span></span>|<span data-ttu-id="7caa0-131">说明</span><span class="sxs-lookup"><span data-stu-id="7caa0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7caa0-132">id</span><span class="sxs-lookup"><span data-stu-id="7caa0-132">id</span></span>|<span data-ttu-id="7caa0-133">String</span><span class="sxs-lookup"><span data-stu-id="7caa0-133">String</span></span>|<span data-ttu-id="7caa0-134">从[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)继承的类别 ID</span><span class="sxs-lookup"><span data-stu-id="7caa0-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="7caa0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7caa0-135">displayName</span></span>|<span data-ttu-id="7caa0-136">String</span><span class="sxs-lookup"><span data-stu-id="7caa0-136">String</span></span>|<span data-ttu-id="7caa0-137">继承自[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)的类别名称</span><span class="sxs-lookup"><span data-stu-id="7caa0-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7caa0-138">响应</span><span class="sxs-lookup"><span data-stu-id="7caa0-138">Response</span></span>
<span data-ttu-id="7caa0-139">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7caa0-139">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7caa0-140">示例</span><span class="sxs-lookup"><span data-stu-id="7caa0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7caa0-141">请求</span><span class="sxs-lookup"><span data-stu-id="7caa0-141">Request</span></span>
<span data-ttu-id="7caa0-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7caa0-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="7caa0-143">响应</span><span class="sxs-lookup"><span data-stu-id="7caa0-143">Response</span></span>
<span data-ttu-id="7caa0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7caa0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 168

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value"
}
```





