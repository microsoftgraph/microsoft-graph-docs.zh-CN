---
title: updateDefinitionValues 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee5b84d880006323ae50c4d78e6c3b762bf8b764
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724190"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="0ac8e-103">updateDefinitionValues 操作</span><span class="sxs-lookup"><span data-stu-id="0ac8e-103">updateDefinitionValues action</span></span>

<span data-ttu-id="0ac8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ac8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ac8e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ac8e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ac8e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0ac8e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ac8e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ac8e-108">Prerequisites</span></span>
<span data-ttu-id="0ac8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac8e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ac8e-111">Permission type</span></span>|<span data-ttu-id="0ac8e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ac8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ac8e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ac8e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac8e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ac8e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ac8e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-116">Not supported.</span></span>|
|<span data-ttu-id="0ac8e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ac8e-117">Application</span></span>|<span data-ttu-id="0ac8e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac8e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ac8e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ac8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="0ac8e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ac8e-120">Request headers</span></span>
|<span data-ttu-id="0ac8e-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ac8e-121">Header</span></span>|<span data-ttu-id="0ac8e-122">值</span><span class="sxs-lookup"><span data-stu-id="0ac8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ac8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac8e-123">Authorization</span></span>|<span data-ttu-id="0ac8e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ac8e-125">接受</span><span class="sxs-lookup"><span data-stu-id="0ac8e-125">Accept</span></span>|<span data-ttu-id="0ac8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ac8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac8e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ac8e-127">Request body</span></span>
<span data-ttu-id="0ac8e-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0ac8e-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0ac8e-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ac8e-130">Property</span></span>|<span data-ttu-id="0ac8e-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ac8e-131">Type</span></span>|<span data-ttu-id="0ac8e-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ac8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ac8e-133">添加内容</span><span class="sxs-lookup"><span data-stu-id="0ac8e-133">added</span></span>|<span data-ttu-id="0ac8e-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ac8e-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="0ac8e-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0ac8e-135">Not yet documented</span></span>|
|<span data-ttu-id="0ac8e-136">updated</span><span class="sxs-lookup"><span data-stu-id="0ac8e-136">updated</span></span>|<span data-ttu-id="0ac8e-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ac8e-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="0ac8e-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0ac8e-138">Not yet documented</span></span>|
|<span data-ttu-id="0ac8e-139">deletedIds</span><span class="sxs-lookup"><span data-stu-id="0ac8e-139">deletedIds</span></span>|<span data-ttu-id="0ac8e-140">String collection</span><span class="sxs-lookup"><span data-stu-id="0ac8e-140">String collection</span></span>|<span data-ttu-id="0ac8e-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0ac8e-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0ac8e-142">响应</span><span class="sxs-lookup"><span data-stu-id="0ac8e-142">Response</span></span>
<span data-ttu-id="0ac8e-143">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0ac8e-144">示例</span><span class="sxs-lookup"><span data-stu-id="0ac8e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ac8e-145">请求</span><span class="sxs-lookup"><span data-stu-id="0ac8e-145">Request</span></span>
<span data-ttu-id="0ac8e-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ac8e-147">响应</span><span class="sxs-lookup"><span data-stu-id="0ac8e-147">Response</span></span>
<span data-ttu-id="0ac8e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ac8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





