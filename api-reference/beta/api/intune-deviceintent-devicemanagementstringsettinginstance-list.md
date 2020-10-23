---
title: 列出 deviceManagementStringSettingInstances
description: 列出 deviceManagementStringSettingInstance 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cccd573bca29ee65e8cff6d5e094925b5bb5e1bf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690369"
---
# <a name="list-devicemanagementstringsettinginstances"></a><span data-ttu-id="8bdcc-103">列出 deviceManagementStringSettingInstances</span><span class="sxs-lookup"><span data-stu-id="8bdcc-103">List deviceManagementStringSettingInstances</span></span>

<span data-ttu-id="8bdcc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bdcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bdcc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bdcc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bdcc-107">列出 [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-107">List properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bdcc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8bdcc-108">Prerequisites</span></span>
<span data-ttu-id="8bdcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bdcc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bdcc-111">Permission type</span></span>|<span data-ttu-id="8bdcc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8bdcc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bdcc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bdcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bdcc-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bdcc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8bdcc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bdcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bdcc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-116">Not supported.</span></span>|
|<span data-ttu-id="8bdcc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bdcc-117">Application</span></span>|<span data-ttu-id="8bdcc-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bdcc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bdcc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bdcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="8bdcc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bdcc-120">Request headers</span></span>
|<span data-ttu-id="8bdcc-121">标头</span><span class="sxs-lookup"><span data-stu-id="8bdcc-121">Header</span></span>|<span data-ttu-id="8bdcc-122">值</span><span class="sxs-lookup"><span data-stu-id="8bdcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bdcc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bdcc-123">Authorization</span></span>|<span data-ttu-id="8bdcc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bdcc-125">接受</span><span class="sxs-lookup"><span data-stu-id="8bdcc-125">Accept</span></span>|<span data-ttu-id="8bdcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bdcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bdcc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bdcc-127">Request body</span></span>
<span data-ttu-id="8bdcc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bdcc-129">响应</span><span class="sxs-lookup"><span data-stu-id="8bdcc-129">Response</span></span>
<span data-ttu-id="8bdcc-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bdcc-131">示例</span><span class="sxs-lookup"><span data-stu-id="8bdcc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bdcc-132">请求</span><span class="sxs-lookup"><span data-stu-id="8bdcc-132">Request</span></span>
<span data-ttu-id="8bdcc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="8bdcc-134">响应</span><span class="sxs-lookup"><span data-stu-id="8bdcc-134">Response</span></span>
<span data-ttu-id="8bdcc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8bdcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
      "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": "Value value"
    }
  ]
}
```





