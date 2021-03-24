---
title: compare 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe4a73d3f1ea449027a193c8de4e3fc8a3c2ee20
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128948"
---
# <a name="compare-function"></a><span data-ttu-id="b0c33-103">compare 函数</span><span class="sxs-lookup"><span data-stu-id="b0c33-103">compare function</span></span>

<span data-ttu-id="b0c33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0c33-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0c33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0c33-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0c33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0c33-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b0c33-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0c33-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0c33-108">Prerequisites</span></span>
<span data-ttu-id="b0c33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0c33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0c33-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0c33-111">Permission type</span></span>|<span data-ttu-id="b0c33-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0c33-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0c33-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0c33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0c33-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c33-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0c33-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0c33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0c33-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0c33-116">Not supported.</span></span>|
|<span data-ttu-id="b0c33-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0c33-117">Application</span></span>|<span data-ttu-id="b0c33-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c33-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0c33-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0c33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="b0c33-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0c33-120">Request headers</span></span>
|<span data-ttu-id="b0c33-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0c33-121">Header</span></span>|<span data-ttu-id="b0c33-122">值</span><span class="sxs-lookup"><span data-stu-id="b0c33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0c33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0c33-123">Authorization</span></span>|<span data-ttu-id="b0c33-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0c33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0c33-125">接受</span><span class="sxs-lookup"><span data-stu-id="b0c33-125">Accept</span></span>|<span data-ttu-id="b0c33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0c33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0c33-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0c33-127">Request body</span></span>
<span data-ttu-id="b0c33-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b0c33-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b0c33-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b0c33-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b0c33-130">属性</span><span class="sxs-lookup"><span data-stu-id="b0c33-130">Property</span></span>|<span data-ttu-id="b0c33-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0c33-131">Type</span></span>|<span data-ttu-id="b0c33-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0c33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c33-133">templateId</span><span class="sxs-lookup"><span data-stu-id="b0c33-133">templateId</span></span>|<span data-ttu-id="b0c33-134">String</span><span class="sxs-lookup"><span data-stu-id="b0c33-134">String</span></span>|<span data-ttu-id="b0c33-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b0c33-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b0c33-136">响应</span><span class="sxs-lookup"><span data-stu-id="b0c33-136">Response</span></span>
<span data-ttu-id="b0c33-137">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="b0c33-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0c33-138">示例</span><span class="sxs-lookup"><span data-stu-id="b0c33-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0c33-139">请求</span><span class="sxs-lookup"><span data-stu-id="b0c33-139">Request</span></span>
<span data-ttu-id="b0c33-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0c33-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b0c33-141">响应</span><span class="sxs-lookup"><span data-stu-id="b0c33-141">Response</span></span>
<span data-ttu-id="b0c33-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0c33-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




