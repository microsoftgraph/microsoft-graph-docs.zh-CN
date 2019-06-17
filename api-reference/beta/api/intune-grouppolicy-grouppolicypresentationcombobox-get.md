---
title: 获取 groupPolicyPresentationComboBox
description: 读取 groupPolicyPresentationComboBox 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4b651b8bfdf57b144df4a296e5c206724f8238c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985127"
---
# <a name="get-grouppolicypresentationcombobox"></a><span data-ttu-id="f0df9-103">获取 groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="f0df9-103">Get groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="f0df9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0df9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0df9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0df9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0df9-106">读取[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0df9-106">Read properties and relationships of the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0df9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0df9-107">Prerequisites</span></span>
<span data-ttu-id="f0df9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0df9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0df9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0df9-110">Permission type</span></span>|<span data-ttu-id="f0df9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0df9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0df9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0df9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0df9-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0df9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f0df9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0df9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0df9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0df9-115">Not supported.</span></span>|
|<span data-ttu-id="f0df9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0df9-116">Application</span></span>|<span data-ttu-id="f0df9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0df9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0df9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0df9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0df9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0df9-119">Optional query parameters</span></span>
<span data-ttu-id="f0df9-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f0df9-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0df9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0df9-121">Request headers</span></span>
|<span data-ttu-id="f0df9-122">标头</span><span class="sxs-lookup"><span data-stu-id="f0df9-122">Header</span></span>|<span data-ttu-id="f0df9-123">值</span><span class="sxs-lookup"><span data-stu-id="f0df9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0df9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0df9-124">Authorization</span></span>|<span data-ttu-id="f0df9-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0df9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0df9-126">接受</span><span class="sxs-lookup"><span data-stu-id="f0df9-126">Accept</span></span>|<span data-ttu-id="f0df9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f0df9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0df9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0df9-128">Request body</span></span>
<span data-ttu-id="f0df9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0df9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0df9-130">响应</span><span class="sxs-lookup"><span data-stu-id="f0df9-130">Response</span></span>
<span data-ttu-id="f0df9-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0df9-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0df9-132">示例</span><span class="sxs-lookup"><span data-stu-id="f0df9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0df9-133">请求</span><span class="sxs-lookup"><span data-stu-id="f0df9-133">Request</span></span>
<span data-ttu-id="f0df9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0df9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="f0df9-135">响应</span><span class="sxs-lookup"><span data-stu-id="f0df9-135">Response</span></span>
<span data-ttu-id="f0df9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0df9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
    "label": "Label value",
    "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": "Default Value value",
    "suggestions": [
      "Suggestions value"
    ],
    "required": true,
    "maxLength": 9
  }
}
```





