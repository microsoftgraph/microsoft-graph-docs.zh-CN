---
title: updatePriorities 操作
description: 更新策略优先级。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a78ec2801522354709643dfdd88da0e6dd9756c8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412973"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="f2aad-103">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="f2aad-103">updatePriorities action</span></span>

> <span data-ttu-id="f2aad-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f2aad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2aad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2aad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2aad-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2aad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2aad-107">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="f2aad-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2aad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2aad-108">Prerequisites</span></span>
<span data-ttu-id="f2aad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2aad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2aad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2aad-111">Permission type</span></span>|<span data-ttu-id="f2aad-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2aad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2aad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2aad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2aad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2aad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2aad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2aad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2aad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2aad-116">Not supported.</span></span>|
|<span data-ttu-id="f2aad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2aad-117">Application</span></span>|<span data-ttu-id="f2aad-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2aad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2aad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2aad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="f2aad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2aad-120">Request headers</span></span>
|<span data-ttu-id="f2aad-121">标头</span><span class="sxs-lookup"><span data-stu-id="f2aad-121">Header</span></span>|<span data-ttu-id="f2aad-122">值</span><span class="sxs-lookup"><span data-stu-id="f2aad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2aad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2aad-123">Authorization</span></span>|<span data-ttu-id="f2aad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2aad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2aad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2aad-125">Accept</span></span>|<span data-ttu-id="f2aad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2aad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2aad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2aad-127">Request body</span></span>
<span data-ttu-id="f2aad-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2aad-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f2aad-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f2aad-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f2aad-130">属性</span><span class="sxs-lookup"><span data-stu-id="f2aad-130">Property</span></span>|<span data-ttu-id="f2aad-131">类型</span><span class="sxs-lookup"><span data-stu-id="f2aad-131">Type</span></span>|<span data-ttu-id="f2aad-132">说明</span><span class="sxs-lookup"><span data-stu-id="f2aad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2aad-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="f2aad-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="f2aad-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="f2aad-134">String collection</span></span>|<span data-ttu-id="f2aad-135">Office 配置策略 id 列表</span><span class="sxs-lookup"><span data-stu-id="f2aad-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="f2aad-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="f2aad-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="f2aad-137">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="f2aad-137">Int32 collection</span></span>|<span data-ttu-id="f2aad-138">Office 配置优先级列表</span><span class="sxs-lookup"><span data-stu-id="f2aad-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="f2aad-139">响应</span><span class="sxs-lookup"><span data-stu-id="f2aad-139">Response</span></span>
<span data-ttu-id="f2aad-140">如果成功，此操作返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2aad-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f2aad-141">示例</span><span class="sxs-lookup"><span data-stu-id="f2aad-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2aad-142">请求</span><span class="sxs-lookup"><span data-stu-id="f2aad-142">Request</span></span>
<span data-ttu-id="f2aad-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2aad-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2aad-144">响应</span><span class="sxs-lookup"><span data-stu-id="f2aad-144">Response</span></span>
<span data-ttu-id="f2aad-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2aad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



