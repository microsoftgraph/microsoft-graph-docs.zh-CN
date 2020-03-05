---
title: 列出 deviceManagementComplexSettingInstances
description: 列出 deviceManagementComplexSettingInstance 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ec9224af76366d5d11685a9fb22221ed99e96d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471944"
---
# <a name="list-devicemanagementcomplexsettinginstances"></a><span data-ttu-id="647f7-103">列出 deviceManagementComplexSettingInstances</span><span class="sxs-lookup"><span data-stu-id="647f7-103">List deviceManagementComplexSettingInstances</span></span>

<span data-ttu-id="647f7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="647f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="647f7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="647f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="647f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="647f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="647f7-107">列出[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="647f7-107">List properties and relationships of the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="647f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="647f7-108">Prerequisites</span></span>
<span data-ttu-id="647f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="647f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="647f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="647f7-111">Permission type</span></span>|<span data-ttu-id="647f7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="647f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="647f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="647f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="647f7-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="647f7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="647f7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="647f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="647f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="647f7-116">Not supported.</span></span>|
|<span data-ttu-id="647f7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="647f7-117">Application</span></span>|<span data-ttu-id="647f7-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="647f7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="647f7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="647f7-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="647f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="647f7-120">Request headers</span></span>
|<span data-ttu-id="647f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="647f7-121">Header</span></span>|<span data-ttu-id="647f7-122">值</span><span class="sxs-lookup"><span data-stu-id="647f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="647f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="647f7-123">Authorization</span></span>|<span data-ttu-id="647f7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="647f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="647f7-125">接受</span><span class="sxs-lookup"><span data-stu-id="647f7-125">Accept</span></span>|<span data-ttu-id="647f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="647f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="647f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="647f7-127">Request body</span></span>
<span data-ttu-id="647f7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="647f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="647f7-129">响应</span><span class="sxs-lookup"><span data-stu-id="647f7-129">Response</span></span>
<span data-ttu-id="647f7-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="647f7-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="647f7-131">示例</span><span class="sxs-lookup"><span data-stu-id="647f7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="647f7-132">请求</span><span class="sxs-lookup"><span data-stu-id="647f7-132">Request</span></span>
<span data-ttu-id="647f7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="647f7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="647f7-134">响应</span><span class="sxs-lookup"><span data-stu-id="647f7-134">Response</span></span>
<span data-ttu-id="647f7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="647f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
      "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```





