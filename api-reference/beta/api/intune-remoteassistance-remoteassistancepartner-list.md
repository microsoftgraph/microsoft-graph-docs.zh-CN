---
title: 列出 remoteAssistancePartners
description: 列出 remoteAssistancePartner 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5736f675f0efe93cf601fab4f1a8b8fb033d6a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414772"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="9772f-103">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="9772f-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="9772f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9772f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9772f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9772f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9772f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9772f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9772f-107">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9772f-107">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9772f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9772f-108">Prerequisites</span></span>
<span data-ttu-id="9772f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9772f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9772f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9772f-111">Permission type</span></span>|<span data-ttu-id="9772f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9772f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9772f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9772f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9772f-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9772f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9772f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9772f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9772f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9772f-116">Not supported.</span></span>|
|<span data-ttu-id="9772f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9772f-117">Application</span></span>|<span data-ttu-id="9772f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9772f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9772f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9772f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="9772f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9772f-120">Request headers</span></span>
|<span data-ttu-id="9772f-121">标头</span><span class="sxs-lookup"><span data-stu-id="9772f-121">Header</span></span>|<span data-ttu-id="9772f-122">值</span><span class="sxs-lookup"><span data-stu-id="9772f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9772f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9772f-123">Authorization</span></span>|<span data-ttu-id="9772f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9772f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9772f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9772f-125">Accept</span></span>|<span data-ttu-id="9772f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9772f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9772f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9772f-127">Request body</span></span>
<span data-ttu-id="9772f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9772f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9772f-129">响应</span><span class="sxs-lookup"><span data-stu-id="9772f-129">Response</span></span>
<span data-ttu-id="9772f-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9772f-130">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9772f-131">示例</span><span class="sxs-lookup"><span data-stu-id="9772f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9772f-132">请求</span><span class="sxs-lookup"><span data-stu-id="9772f-132">Request</span></span>
<span data-ttu-id="9772f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9772f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="9772f-134">响应</span><span class="sxs-lookup"><span data-stu-id="9772f-134">Response</span></span>
<span data-ttu-id="9772f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9772f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "onboarding",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```




