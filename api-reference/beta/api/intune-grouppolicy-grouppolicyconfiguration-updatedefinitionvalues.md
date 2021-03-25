---
title: updateDefinitionValues 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3fd94bb71e44fb225e307874c4d6771067e94a14
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153382"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="8d3ac-103">updateDefinitionValues 操作</span><span class="sxs-lookup"><span data-stu-id="8d3ac-103">updateDefinitionValues action</span></span>

<span data-ttu-id="8d3ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d3ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d3ac-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d3ac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d3ac-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d3ac-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d3ac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d3ac-108">Prerequisites</span></span>
<span data-ttu-id="8d3ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d3ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d3ac-111">Permission type</span></span>|<span data-ttu-id="8d3ac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d3ac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d3ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d3ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d3ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d3ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d3ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d3ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d3ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-116">Not supported.</span></span>|
|<span data-ttu-id="8d3ac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d3ac-117">Application</span></span>|<span data-ttu-id="8d3ac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d3ac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d3ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d3ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="8d3ac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d3ac-120">Request headers</span></span>
|<span data-ttu-id="8d3ac-121">标头</span><span class="sxs-lookup"><span data-stu-id="8d3ac-121">Header</span></span>|<span data-ttu-id="8d3ac-122">值</span><span class="sxs-lookup"><span data-stu-id="8d3ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d3ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d3ac-123">Authorization</span></span>|<span data-ttu-id="8d3ac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d3ac-125">接受</span><span class="sxs-lookup"><span data-stu-id="8d3ac-125">Accept</span></span>|<span data-ttu-id="8d3ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d3ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d3ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d3ac-127">Request body</span></span>
<span data-ttu-id="8d3ac-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8d3ac-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8d3ac-130">属性</span><span class="sxs-lookup"><span data-stu-id="8d3ac-130">Property</span></span>|<span data-ttu-id="8d3ac-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d3ac-131">Type</span></span>|<span data-ttu-id="8d3ac-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d3ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d3ac-133">添加内容</span><span class="sxs-lookup"><span data-stu-id="8d3ac-133">added</span></span>|<span data-ttu-id="8d3ac-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d3ac-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="8d3ac-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d3ac-135">Not yet documented</span></span>|
|<span data-ttu-id="8d3ac-136">updated</span><span class="sxs-lookup"><span data-stu-id="8d3ac-136">updated</span></span>|<span data-ttu-id="8d3ac-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d3ac-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="8d3ac-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d3ac-138">Not yet documented</span></span>|
|<span data-ttu-id="8d3ac-139">deletedIds</span><span class="sxs-lookup"><span data-stu-id="8d3ac-139">deletedIds</span></span>|<span data-ttu-id="8d3ac-140">String collection</span><span class="sxs-lookup"><span data-stu-id="8d3ac-140">String collection</span></span>|<span data-ttu-id="8d3ac-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d3ac-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8d3ac-142">响应</span><span class="sxs-lookup"><span data-stu-id="8d3ac-142">Response</span></span>
<span data-ttu-id="8d3ac-143">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d3ac-144">示例</span><span class="sxs-lookup"><span data-stu-id="8d3ac-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d3ac-145">请求</span><span class="sxs-lookup"><span data-stu-id="8d3ac-145">Request</span></span>
<span data-ttu-id="8d3ac-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues

Content-type: application/json
Content-length: 759

{
  "added": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "updated": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "deletedIds": [
    "Deleted Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8d3ac-147">响应</span><span class="sxs-lookup"><span data-stu-id="8d3ac-147">Response</span></span>
<span data-ttu-id="8d3ac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




