---
title: updatePriorities 操作
description: 更新策略优先级。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1ed9ad9d44502a32387452d789db8581e95f2ca
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665706"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="ece9b-103">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="ece9b-103">updatePriorities action</span></span>

<span data-ttu-id="ece9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ece9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ece9b-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ece9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ece9b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ece9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ece9b-107">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="ece9b-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ece9b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ece9b-108">Prerequisites</span></span>
<span data-ttu-id="ece9b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ece9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece9b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ece9b-111">Permission type</span></span>|<span data-ttu-id="ece9b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ece9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ece9b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ece9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ece9b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece9b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ece9b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ece9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece9b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ece9b-116">Not supported.</span></span>|
|<span data-ttu-id="ece9b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ece9b-117">Application</span></span>|<span data-ttu-id="ece9b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece9b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece9b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ece9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="ece9b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ece9b-120">Request headers</span></span>
|<span data-ttu-id="ece9b-121">标头</span><span class="sxs-lookup"><span data-stu-id="ece9b-121">Header</span></span>|<span data-ttu-id="ece9b-122">值</span><span class="sxs-lookup"><span data-stu-id="ece9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ece9b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ece9b-123">Authorization</span></span>|<span data-ttu-id="ece9b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ece9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ece9b-125">接受</span><span class="sxs-lookup"><span data-stu-id="ece9b-125">Accept</span></span>|<span data-ttu-id="ece9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ece9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece9b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ece9b-127">Request body</span></span>
<span data-ttu-id="ece9b-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ece9b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ece9b-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ece9b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ece9b-130">属性</span><span class="sxs-lookup"><span data-stu-id="ece9b-130">Property</span></span>|<span data-ttu-id="ece9b-131">类型</span><span class="sxs-lookup"><span data-stu-id="ece9b-131">Type</span></span>|<span data-ttu-id="ece9b-132">说明</span><span class="sxs-lookup"><span data-stu-id="ece9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ece9b-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="ece9b-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="ece9b-134">String collection</span><span class="sxs-lookup"><span data-stu-id="ece9b-134">String collection</span></span>|<span data-ttu-id="ece9b-135">Office 配置策略 ID 列表</span><span class="sxs-lookup"><span data-stu-id="ece9b-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="ece9b-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="ece9b-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="ece9b-137">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="ece9b-137">Int32 collection</span></span>|<span data-ttu-id="ece9b-138">Office 配置优先级列表</span><span class="sxs-lookup"><span data-stu-id="ece9b-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="ece9b-139">响应</span><span class="sxs-lookup"><span data-stu-id="ece9b-139">Response</span></span>
<span data-ttu-id="ece9b-140">如果成功，此操作返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ece9b-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ece9b-141">示例</span><span class="sxs-lookup"><span data-stu-id="ece9b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ece9b-142">请求</span><span class="sxs-lookup"><span data-stu-id="ece9b-142">Request</span></span>
<span data-ttu-id="ece9b-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ece9b-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ece9b-144">响应</span><span class="sxs-lookup"><span data-stu-id="ece9b-144">Response</span></span>
<span data-ttu-id="ece9b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ece9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




