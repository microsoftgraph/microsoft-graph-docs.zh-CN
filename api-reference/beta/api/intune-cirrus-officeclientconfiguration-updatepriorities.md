---
title: updatePriorities 操作
description: 更新策略优先级。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 695ef53c26d2eabf119c88084f9698a8db3bd3b2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39930770"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="0a389-103">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="0a389-103">updatePriorities action</span></span>

> <span data-ttu-id="0a389-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a389-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a389-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a389-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a389-106">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="0a389-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a389-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0a389-107">Prerequisites</span></span>
<span data-ttu-id="0a389-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a389-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a389-110">Permission type</span></span>|<span data-ttu-id="0a389-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0a389-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a389-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a389-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a389-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a389-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a389-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a389-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a389-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a389-115">Not supported.</span></span>|
|<span data-ttu-id="0a389-116">Application</span><span class="sxs-lookup"><span data-stu-id="0a389-116">Application</span></span>|<span data-ttu-id="0a389-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a389-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a389-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a389-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="0a389-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a389-119">Request headers</span></span>
|<span data-ttu-id="0a389-120">标头</span><span class="sxs-lookup"><span data-stu-id="0a389-120">Header</span></span>|<span data-ttu-id="0a389-121">值</span><span class="sxs-lookup"><span data-stu-id="0a389-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a389-122">授权</span><span class="sxs-lookup"><span data-stu-id="0a389-122">Authorization</span></span>|<span data-ttu-id="0a389-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0a389-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a389-124">接受</span><span class="sxs-lookup"><span data-stu-id="0a389-124">Accept</span></span>|<span data-ttu-id="0a389-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a389-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a389-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a389-126">Request body</span></span>
<span data-ttu-id="0a389-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a389-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0a389-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="0a389-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0a389-129">属性</span><span class="sxs-lookup"><span data-stu-id="0a389-129">Property</span></span>|<span data-ttu-id="0a389-130">类型</span><span class="sxs-lookup"><span data-stu-id="0a389-130">Type</span></span>|<span data-ttu-id="0a389-131">说明</span><span class="sxs-lookup"><span data-stu-id="0a389-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a389-132">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="0a389-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="0a389-133">String collection</span><span class="sxs-lookup"><span data-stu-id="0a389-133">String collection</span></span>|<span data-ttu-id="0a389-134">Office 配置策略 id 列表</span><span class="sxs-lookup"><span data-stu-id="0a389-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="0a389-135">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="0a389-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="0a389-136">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="0a389-136">Int32 collection</span></span>|<span data-ttu-id="0a389-137">Office 配置优先级列表</span><span class="sxs-lookup"><span data-stu-id="0a389-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="0a389-138">响应</span><span class="sxs-lookup"><span data-stu-id="0a389-138">Response</span></span>
<span data-ttu-id="0a389-139">如果成功，此操作返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0a389-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a389-140">示例</span><span class="sxs-lookup"><span data-stu-id="0a389-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a389-141">请求</span><span class="sxs-lookup"><span data-stu-id="0a389-141">Request</span></span>
<span data-ttu-id="0a389-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a389-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities

Content-type: application/json
Content-length: 143

{
  "officeConfigurationPolicyIds": [
    "Office Configuration Policy Ids value"
  ],
  "officeConfigurationPriorities": [
    13
  ]
}
```

### <a name="response"></a><span data-ttu-id="0a389-143">响应</span><span class="sxs-lookup"><span data-stu-id="0a389-143">Response</span></span>
<span data-ttu-id="0a389-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a389-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```





