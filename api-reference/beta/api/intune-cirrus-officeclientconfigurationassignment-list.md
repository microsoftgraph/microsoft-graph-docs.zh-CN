---
title: 列出 officeClientConfigurationAssignments
description: 列出 officeClientConfigurationAssignment 对象的属性和关系。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 570281f3961f1f4449ae9050cd77b12863452fc3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665703"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="4e343-103">列出 officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="4e343-103">List officeClientConfigurationAssignments</span></span>

<span data-ttu-id="4e343-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e343-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e343-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e343-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e343-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e343-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e343-107">列出 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4e343-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e343-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4e343-108">Prerequisites</span></span>
<span data-ttu-id="4e343-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e343-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e343-111">Permission type</span></span>|<span data-ttu-id="4e343-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4e343-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e343-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e343-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e343-114">\*\*TODO： Determine scopes \*\*</span><span class="sxs-lookup"><span data-stu-id="4e343-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="4e343-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e343-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e343-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e343-116">Not supported.</span></span>|
|<span data-ttu-id="4e343-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e343-117">Application</span></span>|<span data-ttu-id="4e343-118">\*\*TODO： Determine scopes \*\*</span><span class="sxs-lookup"><span data-stu-id="4e343-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e343-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e343-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4e343-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e343-120">Request headers</span></span>
|<span data-ttu-id="4e343-121">标头</span><span class="sxs-lookup"><span data-stu-id="4e343-121">Header</span></span>|<span data-ttu-id="4e343-122">值</span><span class="sxs-lookup"><span data-stu-id="4e343-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e343-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e343-123">Authorization</span></span>|<span data-ttu-id="4e343-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4e343-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e343-125">接受</span><span class="sxs-lookup"><span data-stu-id="4e343-125">Accept</span></span>|<span data-ttu-id="4e343-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e343-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e343-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e343-127">Request body</span></span>
<span data-ttu-id="4e343-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e343-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e343-129">响应</span><span class="sxs-lookup"><span data-stu-id="4e343-129">Response</span></span>
<span data-ttu-id="4e343-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4e343-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e343-131">示例</span><span class="sxs-lookup"><span data-stu-id="4e343-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e343-132">请求</span><span class="sxs-lookup"><span data-stu-id="4e343-132">Request</span></span>
<span data-ttu-id="4e343-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e343-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="4e343-134">响应</span><span class="sxs-lookup"><span data-stu-id="4e343-134">Response</span></span>
<span data-ttu-id="4e343-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e343-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




