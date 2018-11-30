---
title: updatePriorities 操作
description: 更新策略优先级。
ms.openlocfilehash: 23f41214b0dbbbdbf5949edea8857f8623ef0208
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048712"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="4d770-103">updatePriorities 操作</span><span class="sxs-lookup"><span data-stu-id="4d770-103">updatePriorities action</span></span>

> <span data-ttu-id="4d770-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4d770-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d770-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4d770-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d770-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4d770-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d770-107">更新策略优先级。</span><span class="sxs-lookup"><span data-stu-id="4d770-107">Update policy priorities.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d770-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d770-108">Prerequisites</span></span>
<span data-ttu-id="4d770-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4d770-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d770-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d770-111">Permission type</span></span>|<span data-ttu-id="4d770-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d770-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d770-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d770-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d770-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d770-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d770-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d770-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d770-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d770-116">Not supported.</span></span>|
|<span data-ttu-id="4d770-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d770-117">Application</span></span>|<span data-ttu-id="4d770-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d770-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d770-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d770-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="4d770-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d770-120">Request headers</span></span>
|<span data-ttu-id="4d770-121">标头</span><span class="sxs-lookup"><span data-stu-id="4d770-121">Header</span></span>|<span data-ttu-id="4d770-122">值</span><span class="sxs-lookup"><span data-stu-id="4d770-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d770-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d770-123">Authorization</span></span>|<span data-ttu-id="4d770-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d770-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d770-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4d770-125">Accept</span></span>|<span data-ttu-id="4d770-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d770-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d770-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d770-127">Request body</span></span>
<span data-ttu-id="4d770-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d770-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4d770-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="4d770-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4d770-130">属性</span><span class="sxs-lookup"><span data-stu-id="4d770-130">Property</span></span>|<span data-ttu-id="4d770-131">类型</span><span class="sxs-lookup"><span data-stu-id="4d770-131">Type</span></span>|<span data-ttu-id="4d770-132">说明</span><span class="sxs-lookup"><span data-stu-id="4d770-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d770-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="4d770-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="4d770-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="4d770-134">String collection</span></span>|<span data-ttu-id="4d770-135">Office 配置策略 id 列表</span><span class="sxs-lookup"><span data-stu-id="4d770-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="4d770-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="4d770-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="4d770-137">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="4d770-137">Int32 collection</span></span>|<span data-ttu-id="4d770-138">Office 配置优先级列表</span><span class="sxs-lookup"><span data-stu-id="4d770-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="4d770-139">响应</span><span class="sxs-lookup"><span data-stu-id="4d770-139">Response</span></span>
<span data-ttu-id="4d770-140">如果成功，此操作返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4d770-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d770-141">示例</span><span class="sxs-lookup"><span data-stu-id="4d770-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d770-142">请求</span><span class="sxs-lookup"><span data-stu-id="4d770-142">Request</span></span>
<span data-ttu-id="4d770-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d770-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d770-144">响应</span><span class="sxs-lookup"><span data-stu-id="4d770-144">Response</span></span>
<span data-ttu-id="4d770-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d770-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



