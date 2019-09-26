---
title: 列出 groupPolicyPresentationLongDecimalTextBoxes
description: 列出 groupPolicyPresentationLongDecimalTextBox 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a729fdfb552e2f88e29c37ae78e6eed5afbea68
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194157"
---
# <a name="list-grouppolicypresentationlongdecimaltextboxes"></a><span data-ttu-id="24cef-103">列出 groupPolicyPresentationLongDecimalTextBoxes</span><span class="sxs-lookup"><span data-stu-id="24cef-103">List groupPolicyPresentationLongDecimalTextBoxes</span></span>

> <span data-ttu-id="24cef-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24cef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24cef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24cef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24cef-106">列出[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24cef-106">List properties and relationships of the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24cef-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="24cef-107">Prerequisites</span></span>
<span data-ttu-id="24cef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24cef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24cef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="24cef-110">Permission type</span></span>|<span data-ttu-id="24cef-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24cef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24cef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24cef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24cef-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="24cef-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="24cef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24cef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24cef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="24cef-115">Not supported.</span></span>|
|<span data-ttu-id="24cef-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="24cef-116">Application</span></span>|<span data-ttu-id="24cef-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="24cef-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24cef-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24cef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="24cef-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="24cef-119">Request headers</span></span>
|<span data-ttu-id="24cef-120">标头</span><span class="sxs-lookup"><span data-stu-id="24cef-120">Header</span></span>|<span data-ttu-id="24cef-121">值</span><span class="sxs-lookup"><span data-stu-id="24cef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24cef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24cef-122">Authorization</span></span>|<span data-ttu-id="24cef-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24cef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24cef-124">接受</span><span class="sxs-lookup"><span data-stu-id="24cef-124">Accept</span></span>|<span data-ttu-id="24cef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24cef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24cef-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="24cef-126">Request body</span></span>
<span data-ttu-id="24cef-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24cef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24cef-128">响应</span><span class="sxs-lookup"><span data-stu-id="24cef-128">Response</span></span>
<span data-ttu-id="24cef-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="24cef-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24cef-130">示例</span><span class="sxs-lookup"><span data-stu-id="24cef-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="24cef-131">请求</span><span class="sxs-lookup"><span data-stu-id="24cef-131">Request</span></span>
<span data-ttu-id="24cef-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24cef-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="24cef-133">响应</span><span class="sxs-lookup"><span data-stu-id="24cef-133">Response</span></span>
<span data-ttu-id="24cef-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24cef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
      "label": "Label value",
      "id": "754d8495-8495-754d-9584-4d7595844d75",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultValue": 12,
      "spin": true,
      "spinStep": 8,
      "required": true,
      "minValue": 8,
      "maxValue": 8
    }
  ]
}
```




