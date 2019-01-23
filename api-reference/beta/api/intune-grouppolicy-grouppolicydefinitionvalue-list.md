---
title: 列表 groupPolicyDefinitionValues
description: 列出属性和 groupPolicyDefinitionValue 对象之间的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6ba2a625745b3754c2948f626384f6647ca1ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429510"
---
# <a name="list-grouppolicydefinitionvalues"></a><span data-ttu-id="ea87a-103">列表 groupPolicyDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="ea87a-103">List groupPolicyDefinitionValues</span></span>

> <span data-ttu-id="ea87a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ea87a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ea87a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea87a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea87a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea87a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea87a-107">列出属性和[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="ea87a-107">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea87a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea87a-108">Prerequisites</span></span>
<span data-ttu-id="ea87a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ea87a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ea87a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea87a-111">Permission type</span></span>|<span data-ttu-id="ea87a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea87a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea87a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea87a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea87a-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea87a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ea87a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea87a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea87a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea87a-116">Not supported.</span></span>|
|<span data-ttu-id="ea87a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea87a-117">Application</span></span>|<span data-ttu-id="ea87a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea87a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea87a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea87a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="ea87a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea87a-120">Request headers</span></span>
|<span data-ttu-id="ea87a-121">标头</span><span class="sxs-lookup"><span data-stu-id="ea87a-121">Header</span></span>|<span data-ttu-id="ea87a-122">值</span><span class="sxs-lookup"><span data-stu-id="ea87a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea87a-123">授权</span><span class="sxs-lookup"><span data-stu-id="ea87a-123">Authorization</span></span>|<span data-ttu-id="ea87a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea87a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea87a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea87a-125">Accept</span></span>|<span data-ttu-id="ea87a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea87a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea87a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea87a-127">Request body</span></span>
<span data-ttu-id="ea87a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea87a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea87a-129">响应</span><span class="sxs-lookup"><span data-stu-id="ea87a-129">Response</span></span>
<span data-ttu-id="ea87a-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="ea87a-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea87a-131">示例</span><span class="sxs-lookup"><span data-stu-id="ea87a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea87a-132">请求</span><span class="sxs-lookup"><span data-stu-id="ea87a-132">Request</span></span>
<span data-ttu-id="ea87a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea87a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

### <a name="response"></a><span data-ttu-id="ea87a-134">响应</span><span class="sxs-lookup"><span data-stu-id="ea87a-134">Response</span></span>
<span data-ttu-id="ea87a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea87a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




