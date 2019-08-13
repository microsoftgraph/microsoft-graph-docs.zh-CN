---
title: 列出 deviceManagementIntentSettingCategories
description: 列出 deviceManagementIntentSettingCategory 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90c00671b621a5e5a6ffe3de2d8a3f8cd621f358
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343473"
---
# <a name="list-devicemanagementintentsettingcategories"></a><span data-ttu-id="775c6-103">列出 deviceManagementIntentSettingCategories</span><span class="sxs-lookup"><span data-stu-id="775c6-103">List deviceManagementIntentSettingCategories</span></span>

> <span data-ttu-id="775c6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="775c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="775c6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="775c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="775c6-106">列出[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="775c6-106">List properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="775c6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="775c6-107">Prerequisites</span></span>
<span data-ttu-id="775c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="775c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="775c6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="775c6-110">Permission type</span></span>|<span data-ttu-id="775c6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="775c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="775c6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="775c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="775c6-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="775c6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="775c6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="775c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="775c6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="775c6-115">Not supported.</span></span>|
|<span data-ttu-id="775c6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="775c6-116">Application</span></span>|<span data-ttu-id="775c6-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="775c6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="775c6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="775c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="775c6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="775c6-119">Request headers</span></span>
|<span data-ttu-id="775c6-120">标头</span><span class="sxs-lookup"><span data-stu-id="775c6-120">Header</span></span>|<span data-ttu-id="775c6-121">值</span><span class="sxs-lookup"><span data-stu-id="775c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="775c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="775c6-122">Authorization</span></span>|<span data-ttu-id="775c6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="775c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="775c6-124">接受</span><span class="sxs-lookup"><span data-stu-id="775c6-124">Accept</span></span>|<span data-ttu-id="775c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="775c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="775c6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="775c6-126">Request body</span></span>
<span data-ttu-id="775c6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="775c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="775c6-128">响应</span><span class="sxs-lookup"><span data-stu-id="775c6-128">Response</span></span>
<span data-ttu-id="775c6-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="775c6-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="775c6-130">示例</span><span class="sxs-lookup"><span data-stu-id="775c6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="775c6-131">请求</span><span class="sxs-lookup"><span data-stu-id="775c6-131">Request</span></span>
<span data-ttu-id="775c6-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="775c6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
```

### <a name="response"></a><span data-ttu-id="775c6-133">响应</span><span class="sxs-lookup"><span data-stu-id="775c6-133">Response</span></span>
<span data-ttu-id="775c6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="775c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
      "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
      "displayName": "Display Name value"
    }
  ]
}
```






