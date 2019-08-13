---
title: updateSettings 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f42a8164d944edb1c23f0f7b2a2d67bc025e0e0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343683"
---
# <a name="updatesettings-action"></a><span data-ttu-id="d2c2c-103">updateSettings 操作</span><span class="sxs-lookup"><span data-stu-id="d2c2c-103">updateSettings action</span></span>

> <span data-ttu-id="d2c2c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2c2c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2c2c-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2c2c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2c2c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2c2c-107">Prerequisites</span></span>
<span data-ttu-id="d2c2c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2c2c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2c2c-110">Permission type</span></span>|<span data-ttu-id="d2c2c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2c2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2c2c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2c2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2c2c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c2c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2c2c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2c2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2c2c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-115">Not supported.</span></span>|
|<span data-ttu-id="d2c2c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2c2c-116">Application</span></span>|<span data-ttu-id="d2c2c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c2c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2c2c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2c2c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="d2c2c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2c2c-119">Request headers</span></span>
|<span data-ttu-id="d2c2c-120">标头</span><span class="sxs-lookup"><span data-stu-id="d2c2c-120">Header</span></span>|<span data-ttu-id="d2c2c-121">值</span><span class="sxs-lookup"><span data-stu-id="d2c2c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2c2c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2c2c-122">Authorization</span></span>|<span data-ttu-id="d2c2c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2c2c-124">接受</span><span class="sxs-lookup"><span data-stu-id="d2c2c-124">Accept</span></span>|<span data-ttu-id="d2c2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2c2c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2c2c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2c2c-126">Request body</span></span>
<span data-ttu-id="d2c2c-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d2c2c-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d2c2c-129">属性</span><span class="sxs-lookup"><span data-stu-id="d2c2c-129">Property</span></span>|<span data-ttu-id="d2c2c-130">类型</span><span class="sxs-lookup"><span data-stu-id="d2c2c-130">Type</span></span>|<span data-ttu-id="d2c2c-131">说明</span><span class="sxs-lookup"><span data-stu-id="d2c2c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2c2c-132">settings</span><span class="sxs-lookup"><span data-stu-id="d2c2c-132">settings</span></span>|<span data-ttu-id="d2c2c-133">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="d2c2c-133">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="d2c2c-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2c2c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d2c2c-135">响应</span><span class="sxs-lookup"><span data-stu-id="d2c2c-135">Response</span></span>
<span data-ttu-id="d2c2c-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2c2c-137">示例</span><span class="sxs-lookup"><span data-stu-id="d2c2c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2c2c-138">请求</span><span class="sxs-lookup"><span data-stu-id="d2c2c-138">Request</span></span>
<span data-ttu-id="d2c2c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/updateSettings

Content-type: application/json
Content-length: 252

{
  "settings": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d2c2c-140">响应</span><span class="sxs-lookup"><span data-stu-id="d2c2c-140">Response</span></span>
<span data-ttu-id="d2c2c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2c2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






