---
title: Office客户端配置分配操作
description: 替换策略的所有目标组。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4fb8f6d2bb05e5809337ed4be0010f8f6cb470f4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665714"
---
# <a name="office-client-configuration-assign--assign-action"></a><span data-ttu-id="c9633-103">Office客户端配置分配操作</span><span class="sxs-lookup"><span data-stu-id="c9633-103">Office client configuration assign  assign action</span></span>

<span data-ttu-id="c9633-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9633-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9633-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9633-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9633-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9633-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9633-107">替换策略的所有目标组。</span><span class="sxs-lookup"><span data-stu-id="c9633-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9633-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9633-108">Prerequisites</span></span>
<span data-ttu-id="c9633-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9633-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9633-111">Permission type</span></span>|<span data-ttu-id="c9633-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9633-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9633-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9633-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9633-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9633-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9633-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9633-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9633-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9633-116">Not supported.</span></span>|
|<span data-ttu-id="c9633-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9633-117">Application</span></span>|<span data-ttu-id="c9633-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9633-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9633-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9633-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c9633-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9633-120">Request headers</span></span>
|<span data-ttu-id="c9633-121">标头</span><span class="sxs-lookup"><span data-stu-id="c9633-121">Header</span></span>|<span data-ttu-id="c9633-122">值</span><span class="sxs-lookup"><span data-stu-id="c9633-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9633-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9633-123">Authorization</span></span>|<span data-ttu-id="c9633-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9633-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9633-125">接受</span><span class="sxs-lookup"><span data-stu-id="c9633-125">Accept</span></span>|<span data-ttu-id="c9633-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9633-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9633-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9633-127">Request body</span></span>
<span data-ttu-id="c9633-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9633-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c9633-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c9633-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c9633-130">属性</span><span class="sxs-lookup"><span data-stu-id="c9633-130">Property</span></span>|<span data-ttu-id="c9633-131">类型</span><span class="sxs-lookup"><span data-stu-id="c9633-131">Type</span></span>|<span data-ttu-id="c9633-132">说明</span><span class="sxs-lookup"><span data-stu-id="c9633-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9633-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c9633-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="c9633-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9633-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c9633-135">Office 配置分配列表</span><span class="sxs-lookup"><span data-stu-id="c9633-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="c9633-136">响应</span><span class="sxs-lookup"><span data-stu-id="c9633-136">Response</span></span>
<span data-ttu-id="c9633-137">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="c9633-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9633-138">示例</span><span class="sxs-lookup"><span data-stu-id="c9633-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9633-139">请求</span><span class="sxs-lookup"><span data-stu-id="c9633-139">Request</span></span>
<span data-ttu-id="c9633-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9633-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9633-141">响应</span><span class="sxs-lookup"><span data-stu-id="c9633-141">Response</span></span>
<span data-ttu-id="c9633-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9633-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




