---
title: assign 操作
description: 替换策略的所有目标组。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9d548e4ac1ec6f72b600c4e91ecd50e5e455159
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322259"
---
# <a name="assign-action"></a><span data-ttu-id="fd1d3-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="fd1d3-103">assign action</span></span>

> <span data-ttu-id="fd1d3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd1d3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd1d3-106">替换策略的所有目标组。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-106">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd1d3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fd1d3-107">Prerequisites</span></span>
<span data-ttu-id="fd1d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd1d3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd1d3-110">Permission type</span></span>|<span data-ttu-id="fd1d3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd1d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd1d3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd1d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd1d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd1d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd1d3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd1d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd1d3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-115">Not supported.</span></span>|
|<span data-ttu-id="fd1d3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd1d3-116">Application</span></span>|<span data-ttu-id="fd1d3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd1d3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd1d3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd1d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="fd1d3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd1d3-119">Request headers</span></span>
|<span data-ttu-id="fd1d3-120">标头</span><span class="sxs-lookup"><span data-stu-id="fd1d3-120">Header</span></span>|<span data-ttu-id="fd1d3-121">值</span><span class="sxs-lookup"><span data-stu-id="fd1d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd1d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd1d3-122">Authorization</span></span>|<span data-ttu-id="fd1d3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd1d3-124">接受</span><span class="sxs-lookup"><span data-stu-id="fd1d3-124">Accept</span></span>|<span data-ttu-id="fd1d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd1d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd1d3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd1d3-126">Request body</span></span>
<span data-ttu-id="fd1d3-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fd1d3-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fd1d3-129">属性</span><span class="sxs-lookup"><span data-stu-id="fd1d3-129">Property</span></span>|<span data-ttu-id="fd1d3-130">类型</span><span class="sxs-lookup"><span data-stu-id="fd1d3-130">Type</span></span>|<span data-ttu-id="fd1d3-131">说明</span><span class="sxs-lookup"><span data-stu-id="fd1d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd1d3-132">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="fd1d3-132">officeConfigurationAssignments</span></span>|<span data-ttu-id="fd1d3-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="fd1d3-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="fd1d3-134">Office 配置分配列表</span><span class="sxs-lookup"><span data-stu-id="fd1d3-134">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="fd1d3-135">响应</span><span class="sxs-lookup"><span data-stu-id="fd1d3-135">Response</span></span>
<span data-ttu-id="fd1d3-136">如果成功, 此操作会在`200 OK`响应正文中返回响应代码和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-136">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd1d3-137">示例</span><span class="sxs-lookup"><span data-stu-id="fd1d3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd1d3-138">请求</span><span class="sxs-lookup"><span data-stu-id="fd1d3-138">Request</span></span>
<span data-ttu-id="fd1d3-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fd1d3-140">响应</span><span class="sxs-lookup"><span data-stu-id="fd1d3-140">Response</span></span>
<span data-ttu-id="fd1d3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd1d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```






