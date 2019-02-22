---
title: 列出 termsAndConditionses
description: 列出 termsAndConditions 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da16479006a92becfcba1cdf8ebdd93c4f12028f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148445"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="6e2a3-103">列出 termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="6e2a3-103">List termsAndConditionses</span></span>

> <span data-ttu-id="6e2a3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e2a3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e2a3-106">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-106">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e2a3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e2a3-107">Prerequisites</span></span>
<span data-ttu-id="6e2a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e2a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e2a3-110">Permission type</span></span>|<span data-ttu-id="6e2a3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e2a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e2a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e2a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e2a3-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e2a3-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6e2a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e2a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e2a3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-115">Not supported.</span></span>|
|<span data-ttu-id="6e2a3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e2a3-116">Application</span></span>|<span data-ttu-id="6e2a3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e2a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e2a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="6e2a3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e2a3-119">Request headers</span></span>
|<span data-ttu-id="6e2a3-120">标头</span><span class="sxs-lookup"><span data-stu-id="6e2a3-120">Header</span></span>|<span data-ttu-id="6e2a3-121">值</span><span class="sxs-lookup"><span data-stu-id="6e2a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e2a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e2a3-122">Authorization</span></span>|<span data-ttu-id="6e2a3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e2a3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6e2a3-124">Accept</span></span>|<span data-ttu-id="6e2a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e2a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e2a3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e2a3-126">Request body</span></span>
<span data-ttu-id="6e2a3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e2a3-128">响应</span><span class="sxs-lookup"><span data-stu-id="6e2a3-128">Response</span></span>
<span data-ttu-id="6e2a3-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e2a3-130">示例</span><span class="sxs-lookup"><span data-stu-id="6e2a3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e2a3-131">请求</span><span class="sxs-lookup"><span data-stu-id="6e2a3-131">Request</span></span>
<span data-ttu-id="6e2a3-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="6e2a3-133">响应</span><span class="sxs-lookup"><span data-stu-id="6e2a3-133">Response</span></span>
<span data-ttu-id="6e2a3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e2a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```




