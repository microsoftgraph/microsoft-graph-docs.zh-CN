---
title: assign 操作
description: 替换策略的所有目标组。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa0ce371f61b13b5b987fc82fe5329305ec30e65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754345"
---
# <a name="assign-action"></a><span data-ttu-id="34171-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="34171-103">assign action</span></span>

<span data-ttu-id="34171-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34171-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34171-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34171-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34171-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34171-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34171-107">替换策略的所有目标组。</span><span class="sxs-lookup"><span data-stu-id="34171-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34171-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="34171-108">Prerequisites</span></span>
<span data-ttu-id="34171-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34171-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="34171-111">Permission type</span></span>|<span data-ttu-id="34171-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34171-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34171-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34171-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34171-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34171-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34171-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34171-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34171-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34171-116">Not supported.</span></span>|
|<span data-ttu-id="34171-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="34171-117">Application</span></span>|<span data-ttu-id="34171-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34171-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34171-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34171-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="34171-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="34171-120">Request headers</span></span>
|<span data-ttu-id="34171-121">标头</span><span class="sxs-lookup"><span data-stu-id="34171-121">Header</span></span>|<span data-ttu-id="34171-122">值</span><span class="sxs-lookup"><span data-stu-id="34171-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34171-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34171-123">Authorization</span></span>|<span data-ttu-id="34171-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34171-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34171-125">接受</span><span class="sxs-lookup"><span data-stu-id="34171-125">Accept</span></span>|<span data-ttu-id="34171-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34171-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34171-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="34171-127">Request body</span></span>
<span data-ttu-id="34171-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34171-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="34171-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="34171-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="34171-130">属性</span><span class="sxs-lookup"><span data-stu-id="34171-130">Property</span></span>|<span data-ttu-id="34171-131">类型</span><span class="sxs-lookup"><span data-stu-id="34171-131">Type</span></span>|<span data-ttu-id="34171-132">说明</span><span class="sxs-lookup"><span data-stu-id="34171-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34171-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="34171-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="34171-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34171-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="34171-135">Office 配置分配列表</span><span class="sxs-lookup"><span data-stu-id="34171-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="34171-136">响应</span><span class="sxs-lookup"><span data-stu-id="34171-136">Response</span></span>
<span data-ttu-id="34171-137">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="34171-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34171-138">示例</span><span class="sxs-lookup"><span data-stu-id="34171-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="34171-139">请求</span><span class="sxs-lookup"><span data-stu-id="34171-139">Request</span></span>
<span data-ttu-id="34171-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34171-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34171-141">响应</span><span class="sxs-lookup"><span data-stu-id="34171-141">Response</span></span>
<span data-ttu-id="34171-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34171-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




