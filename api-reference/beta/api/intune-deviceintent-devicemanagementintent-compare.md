---
title: compare 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00f9dac88c6fa5d283857e188f0ce07367c184d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471566"
---
# <a name="compare-function"></a><span data-ttu-id="42998-103">compare 函数</span><span class="sxs-lookup"><span data-stu-id="42998-103">compare function</span></span>

<span data-ttu-id="42998-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="42998-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42998-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42998-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42998-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42998-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42998-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42998-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42998-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="42998-108">Prerequisites</span></span>
<span data-ttu-id="42998-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42998-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="42998-111">Permission type</span></span>|<span data-ttu-id="42998-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42998-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42998-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42998-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42998-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="42998-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="42998-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42998-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42998-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42998-116">Not supported.</span></span>|
|<span data-ttu-id="42998-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="42998-117">Application</span></span>|<span data-ttu-id="42998-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="42998-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42998-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42998-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="42998-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42998-120">Request headers</span></span>
|<span data-ttu-id="42998-121">标头</span><span class="sxs-lookup"><span data-stu-id="42998-121">Header</span></span>|<span data-ttu-id="42998-122">值</span><span class="sxs-lookup"><span data-stu-id="42998-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42998-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42998-123">Authorization</span></span>|<span data-ttu-id="42998-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42998-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42998-125">接受</span><span class="sxs-lookup"><span data-stu-id="42998-125">Accept</span></span>|<span data-ttu-id="42998-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42998-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42998-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="42998-127">Request body</span></span>
<span data-ttu-id="42998-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="42998-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="42998-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="42998-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="42998-130">属性</span><span class="sxs-lookup"><span data-stu-id="42998-130">Property</span></span>|<span data-ttu-id="42998-131">类型</span><span class="sxs-lookup"><span data-stu-id="42998-131">Type</span></span>|<span data-ttu-id="42998-132">说明</span><span class="sxs-lookup"><span data-stu-id="42998-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42998-133">templateId</span><span class="sxs-lookup"><span data-stu-id="42998-133">templateId</span></span>|<span data-ttu-id="42998-134">String</span><span class="sxs-lookup"><span data-stu-id="42998-134">String</span></span>|<span data-ttu-id="42998-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42998-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42998-136">响应</span><span class="sxs-lookup"><span data-stu-id="42998-136">Response</span></span>
<span data-ttu-id="42998-137">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)集合。</span><span class="sxs-lookup"><span data-stu-id="42998-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42998-138">示例</span><span class="sxs-lookup"><span data-stu-id="42998-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="42998-139">请求</span><span class="sxs-lookup"><span data-stu-id="42998-139">Request</span></span>
<span data-ttu-id="42998-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42998-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="42998-141">响应</span><span class="sxs-lookup"><span data-stu-id="42998-141">Response</span></span>
<span data-ttu-id="42998-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42998-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingComparison",
      "id": "Id value",
      "displayName": "Display Name value",
      "definitionId": "Definition Id value",
      "currentValueJson": "Current Value Json value",
      "newValueJson": "New Value Json value",
      "comparisonResult": "equal"
    }
  ]
}
```





