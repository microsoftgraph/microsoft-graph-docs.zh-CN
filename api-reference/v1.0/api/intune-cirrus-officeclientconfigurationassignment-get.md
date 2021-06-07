---
title: 获取 officeClientConfigurationAssignment
description: 读取 officeClientConfigurationAssignment 对象的属性和关系。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82380a555c0dade29463b78297ddde0cc96348f0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753058"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="10f8c-103">获取 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="10f8c-103">Get officeClientConfigurationAssignment</span></span>

<span data-ttu-id="10f8c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10f8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10f8c-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10f8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10f8c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10f8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10f8c-107">读取 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10f8c-107">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10f8c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="10f8c-108">Prerequisites</span></span>
<span data-ttu-id="10f8c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10f8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f8c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="10f8c-111">Permission type</span></span>|<span data-ttu-id="10f8c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10f8c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10f8c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10f8c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10f8c-114">\*\*TODO： Determine scopes \*\*</span><span class="sxs-lookup"><span data-stu-id="10f8c-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="10f8c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10f8c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10f8c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10f8c-116">Not supported.</span></span>|
|<span data-ttu-id="10f8c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="10f8c-117">Application</span></span>|<span data-ttu-id="10f8c-118">\*\*TODO： Determine scopes \*\*</span><span class="sxs-lookup"><span data-stu-id="10f8c-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="10f8c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10f8c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10f8c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10f8c-120">Optional query parameters</span></span>
<span data-ttu-id="10f8c-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10f8c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10f8c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="10f8c-122">Request headers</span></span>
|<span data-ttu-id="10f8c-123">标头</span><span class="sxs-lookup"><span data-stu-id="10f8c-123">Header</span></span>|<span data-ttu-id="10f8c-124">值</span><span class="sxs-lookup"><span data-stu-id="10f8c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10f8c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="10f8c-125">Authorization</span></span>|<span data-ttu-id="10f8c-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10f8c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10f8c-127">接受</span><span class="sxs-lookup"><span data-stu-id="10f8c-127">Accept</span></span>|<span data-ttu-id="10f8c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="10f8c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10f8c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="10f8c-129">Request body</span></span>
<span data-ttu-id="10f8c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10f8c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10f8c-131">响应</span><span class="sxs-lookup"><span data-stu-id="10f8c-131">Response</span></span>
<span data-ttu-id="10f8c-132">如果成功，此方法在响应正文 `200 OK` 中返回 响应代码和 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10f8c-132">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f8c-133">示例</span><span class="sxs-lookup"><span data-stu-id="10f8c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="10f8c-134">请求</span><span class="sxs-lookup"><span data-stu-id="10f8c-134">Request</span></span>
<span data-ttu-id="10f8c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10f8c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="10f8c-136">响应</span><span class="sxs-lookup"><span data-stu-id="10f8c-136">Response</span></span>
<span data-ttu-id="10f8c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10f8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




