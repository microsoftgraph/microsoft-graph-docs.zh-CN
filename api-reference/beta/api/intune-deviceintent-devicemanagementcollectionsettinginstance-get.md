---
title: 获取 deviceManagementCollectionSettingInstance
description: 读取 deviceManagementCollectionSettingInstance 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b314ee41522288b6297a8ad66a1573bf38899f6a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916733"
---
# <a name="get-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="2a6b0-103">获取 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2a6b0-103">Get deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="2a6b0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a6b0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a6b0-106">读取[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-106">Read properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a6b0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a6b0-107">Prerequisites</span></span>
<span data-ttu-id="2a6b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a6b0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a6b0-110">Permission type</span></span>|<span data-ttu-id="2a6b0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a6b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a6b0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a6b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a6b0-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a6b0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2a6b0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a6b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a6b0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-115">Not supported.</span></span>|
|<span data-ttu-id="2a6b0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a6b0-116">Application</span></span>|<span data-ttu-id="2a6b0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a6b0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a6b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a6b0-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2a6b0-119">Optional query parameters</span></span>
<span data-ttu-id="2a6b0-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a6b0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a6b0-121">Request headers</span></span>
|<span data-ttu-id="2a6b0-122">标头</span><span class="sxs-lookup"><span data-stu-id="2a6b0-122">Header</span></span>|<span data-ttu-id="2a6b0-123">值</span><span class="sxs-lookup"><span data-stu-id="2a6b0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a6b0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a6b0-124">Authorization</span></span>|<span data-ttu-id="2a6b0-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a6b0-126">接受</span><span class="sxs-lookup"><span data-stu-id="2a6b0-126">Accept</span></span>|<span data-ttu-id="2a6b0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2a6b0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a6b0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a6b0-128">Request body</span></span>
<span data-ttu-id="2a6b0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a6b0-130">响应</span><span class="sxs-lookup"><span data-stu-id="2a6b0-130">Response</span></span>
<span data-ttu-id="2a6b0-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-131">If successful, this method returns a `200 OK` response code and [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a6b0-132">示例</span><span class="sxs-lookup"><span data-stu-id="2a6b0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a6b0-133">请求</span><span class="sxs-lookup"><span data-stu-id="2a6b0-133">Request</span></span>
<span data-ttu-id="2a6b0-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="2a6b0-135">响应</span><span class="sxs-lookup"><span data-stu-id="2a6b0-135">Response</span></span>
<span data-ttu-id="2a6b0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a6b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
    "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value"
  }
}
```




