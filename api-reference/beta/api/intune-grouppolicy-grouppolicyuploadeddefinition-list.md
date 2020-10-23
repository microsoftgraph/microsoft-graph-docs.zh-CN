---
title: 列出 groupPolicyUploadedDefinitions
description: 列出 groupPolicyUploadedDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37b9aa1a7b02ef4349d496b0e0d1a613f0dcd077
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695514"
---
# <a name="list-grouppolicyuploadeddefinitions"></a><span data-ttu-id="76f76-103">列出 groupPolicyUploadedDefinitions</span><span class="sxs-lookup"><span data-stu-id="76f76-103">List groupPolicyUploadedDefinitions</span></span>

<span data-ttu-id="76f76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76f76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76f76-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76f76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76f76-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76f76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76f76-107">列出 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76f76-107">List properties and relationships of the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76f76-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="76f76-108">Prerequisites</span></span>
<span data-ttu-id="76f76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76f76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76f76-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="76f76-111">Permission type</span></span>|<span data-ttu-id="76f76-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76f76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76f76-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76f76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76f76-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76f76-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="76f76-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76f76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76f76-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76f76-116">Not supported.</span></span>|
|<span data-ttu-id="76f76-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="76f76-117">Application</span></span>|<span data-ttu-id="76f76-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76f76-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76f76-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76f76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="76f76-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="76f76-120">Request headers</span></span>
|<span data-ttu-id="76f76-121">标头</span><span class="sxs-lookup"><span data-stu-id="76f76-121">Header</span></span>|<span data-ttu-id="76f76-122">值</span><span class="sxs-lookup"><span data-stu-id="76f76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76f76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76f76-123">Authorization</span></span>|<span data-ttu-id="76f76-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76f76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76f76-125">接受</span><span class="sxs-lookup"><span data-stu-id="76f76-125">Accept</span></span>|<span data-ttu-id="76f76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76f76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76f76-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="76f76-127">Request body</span></span>
<span data-ttu-id="76f76-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76f76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76f76-129">响应</span><span class="sxs-lookup"><span data-stu-id="76f76-129">Response</span></span>
<span data-ttu-id="76f76-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="76f76-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76f76-131">示例</span><span class="sxs-lookup"><span data-stu-id="76f76-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="76f76-132">请求</span><span class="sxs-lookup"><span data-stu-id="76f76-132">Request</span></span>
<span data-ttu-id="76f76-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76f76-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
```

### <a name="response"></a><span data-ttu-id="76f76-134">响应</span><span class="sxs-lookup"><span data-stu-id="76f76-134">Response</span></span>
<span data-ttu-id="76f76-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76f76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
      "classType": "machine",
      "displayName": "Display Name value",
      "explainText": "Explain Text value",
      "categoryPath": "Category Path value",
      "supportedOn": "Supported On value",
      "policyType": "admxIngested",
      "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
      "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





