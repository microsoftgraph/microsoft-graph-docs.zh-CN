---
title: 获取 onPremisesConditionalAccessSettings
description: 读取 onPremisesConditionalAccessSettings 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1aa3e48edfcc36f4b0cf72da77d693f63d324ff0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377681"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="96ba3-103">获取 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="96ba3-103">Get onPremisesConditionalAccessSettings</span></span>

<span data-ttu-id="96ba3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96ba3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96ba3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96ba3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96ba3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96ba3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96ba3-107">读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96ba3-107">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96ba3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="96ba3-108">Prerequisites</span></span>
<span data-ttu-id="96ba3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96ba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96ba3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96ba3-111">Permission type</span></span>|<span data-ttu-id="96ba3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96ba3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96ba3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96ba3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96ba3-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="96ba3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="96ba3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96ba3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96ba3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96ba3-116">Not supported.</span></span>|
|<span data-ttu-id="96ba3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="96ba3-117">Application</span></span>|<span data-ttu-id="96ba3-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="96ba3-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96ba3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96ba3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96ba3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96ba3-120">Optional query parameters</span></span>
<span data-ttu-id="96ba3-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96ba3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96ba3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="96ba3-122">Request headers</span></span>
|<span data-ttu-id="96ba3-123">标头</span><span class="sxs-lookup"><span data-stu-id="96ba3-123">Header</span></span>|<span data-ttu-id="96ba3-124">值</span><span class="sxs-lookup"><span data-stu-id="96ba3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96ba3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96ba3-125">Authorization</span></span>|<span data-ttu-id="96ba3-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96ba3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96ba3-127">接受</span><span class="sxs-lookup"><span data-stu-id="96ba3-127">Accept</span></span>|<span data-ttu-id="96ba3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="96ba3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96ba3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="96ba3-129">Request body</span></span>
<span data-ttu-id="96ba3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96ba3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96ba3-131">响应</span><span class="sxs-lookup"><span data-stu-id="96ba3-131">Response</span></span>
<span data-ttu-id="96ba3-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96ba3-132">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96ba3-133">示例</span><span class="sxs-lookup"><span data-stu-id="96ba3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="96ba3-134">请求</span><span class="sxs-lookup"><span data-stu-id="96ba3-134">Request</span></span>
<span data-ttu-id="96ba3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96ba3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="96ba3-136">响应</span><span class="sxs-lookup"><span data-stu-id="96ba3-136">Response</span></span>
<span data-ttu-id="96ba3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96ba3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "77c9d466-d466-77c9-66d4-c97766d4c977"
    ],
    "excludedGroups": [
      "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
    ],
    "overrideDefaultRule": true
  }
}
```



