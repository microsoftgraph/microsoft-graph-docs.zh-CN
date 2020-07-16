---
title: 列出 policySetAssignments
description: 列出 policySetAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6cdee9ce5f29527ad7ebae846d3a6ef30871caa
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791698"
---
# <a name="list-policysetassignments"></a><span data-ttu-id="6dbfe-103">列出 policySetAssignments</span><span class="sxs-lookup"><span data-stu-id="6dbfe-103">List policySetAssignments</span></span>

<span data-ttu-id="6dbfe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dbfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6dbfe-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dbfe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dbfe-107">列出[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-107">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dbfe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6dbfe-108">Prerequisites</span></span>
<span data-ttu-id="6dbfe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dbfe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dbfe-111">Permission type</span></span>|<span data-ttu-id="6dbfe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6dbfe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dbfe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dbfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dbfe-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dbfe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6dbfe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dbfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dbfe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-116">Not supported.</span></span>|
|<span data-ttu-id="6dbfe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dbfe-117">Application</span></span>|<span data-ttu-id="6dbfe-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dbfe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dbfe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dbfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6dbfe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dbfe-120">Request headers</span></span>
|<span data-ttu-id="6dbfe-121">标头</span><span class="sxs-lookup"><span data-stu-id="6dbfe-121">Header</span></span>|<span data-ttu-id="6dbfe-122">值</span><span class="sxs-lookup"><span data-stu-id="6dbfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dbfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dbfe-123">Authorization</span></span>|<span data-ttu-id="6dbfe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dbfe-125">接受</span><span class="sxs-lookup"><span data-stu-id="6dbfe-125">Accept</span></span>|<span data-ttu-id="6dbfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6dbfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dbfe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dbfe-127">Request body</span></span>
<span data-ttu-id="6dbfe-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dbfe-129">响应</span><span class="sxs-lookup"><span data-stu-id="6dbfe-129">Response</span></span>
<span data-ttu-id="6dbfe-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-130">If successful, this method returns a `200 OK` response code and a collection of [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dbfe-131">示例</span><span class="sxs-lookup"><span data-stu-id="6dbfe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dbfe-132">请求</span><span class="sxs-lookup"><span data-stu-id="6dbfe-132">Request</span></span>
<span data-ttu-id="6dbfe-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
```

### <a name="response"></a><span data-ttu-id="6dbfe-134">响应</span><span class="sxs-lookup"><span data-stu-id="6dbfe-134">Response</span></span>
<span data-ttu-id="6dbfe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dbfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 492

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySetAssignment",
      "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



