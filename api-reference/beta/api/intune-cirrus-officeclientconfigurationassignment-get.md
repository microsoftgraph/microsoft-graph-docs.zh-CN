---
title: 获取 officeClientConfigurationAssignment
description: 读取 officeClientConfigurationAssignment 对象的属性和关系。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 047b2d87fd5e0d77837d3a0e40152ea6ba2e0b8e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958891"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="6c812-103">获取 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6c812-103">Get officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="6c812-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c812-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c812-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c812-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c812-106">读取[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c812-106">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c812-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c812-107">Prerequisites</span></span>
<span data-ttu-id="6c812-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c812-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c812-110">Permission type</span></span>|<span data-ttu-id="6c812-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c812-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c812-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c812-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c812-113">\* \* TODO: 确定作用域 \* \*</span><span class="sxs-lookup"><span data-stu-id="6c812-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="6c812-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c812-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c812-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c812-115">Not supported.</span></span>|
|<span data-ttu-id="6c812-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c812-116">Application</span></span>|<span data-ttu-id="6c812-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c812-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c812-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c812-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c812-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6c812-119">Optional query parameters</span></span>
<span data-ttu-id="6c812-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6c812-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c812-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c812-121">Request headers</span></span>
|<span data-ttu-id="6c812-122">标头</span><span class="sxs-lookup"><span data-stu-id="6c812-122">Header</span></span>|<span data-ttu-id="6c812-123">值</span><span class="sxs-lookup"><span data-stu-id="6c812-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c812-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c812-124">Authorization</span></span>|<span data-ttu-id="6c812-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c812-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c812-126">接受</span><span class="sxs-lookup"><span data-stu-id="6c812-126">Accept</span></span>|<span data-ttu-id="6c812-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c812-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c812-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c812-128">Request body</span></span>
<span data-ttu-id="6c812-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c812-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c812-130">响应</span><span class="sxs-lookup"><span data-stu-id="6c812-130">Response</span></span>
<span data-ttu-id="6c812-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6c812-131">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c812-132">示例</span><span class="sxs-lookup"><span data-stu-id="6c812-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c812-133">请求</span><span class="sxs-lookup"><span data-stu-id="6c812-133">Request</span></span>
<span data-ttu-id="6c812-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c812-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6c812-135">响应</span><span class="sxs-lookup"><span data-stu-id="6c812-135">Response</span></span>
<span data-ttu-id="6c812-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c812-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
    "id": "804730f3-30f3-8047-f330-4780f3304780",
    "target": {
      "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
    }
  }
}
```



