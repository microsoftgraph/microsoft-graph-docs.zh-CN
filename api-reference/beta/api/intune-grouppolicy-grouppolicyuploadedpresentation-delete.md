---
title: 删除 groupPolicyUploadedPresentation
description: 删除 groupPolicyUploadedPresentation。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b50f7ad4827dcd310229191bed7ccaffd2b1a84a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803720"
---
# <a name="delete-grouppolicyuploadedpresentation"></a><span data-ttu-id="a5927-103">删除 groupPolicyUploadedPresentation</span><span class="sxs-lookup"><span data-stu-id="a5927-103">Delete groupPolicyUploadedPresentation</span></span>

> <span data-ttu-id="a5927-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5927-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5927-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5927-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5927-106">删除[groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)。</span><span class="sxs-lookup"><span data-stu-id="a5927-106">Deletes a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5927-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a5927-107">Prerequisites</span></span>
<span data-ttu-id="a5927-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5927-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5927-110">Permission type</span></span>|<span data-ttu-id="a5927-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a5927-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5927-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5927-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5927-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5927-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a5927-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5927-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5927-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5927-115">Not supported.</span></span>|
|<span data-ttu-id="a5927-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5927-116">Application</span></span>|<span data-ttu-id="a5927-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5927-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5927-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5927-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="a5927-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5927-119">Request headers</span></span>
|<span data-ttu-id="a5927-120">标头</span><span class="sxs-lookup"><span data-stu-id="a5927-120">Header</span></span>|<span data-ttu-id="a5927-121">值</span><span class="sxs-lookup"><span data-stu-id="a5927-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5927-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5927-122">Authorization</span></span>|<span data-ttu-id="a5927-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a5927-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5927-124">接受</span><span class="sxs-lookup"><span data-stu-id="a5927-124">Accept</span></span>|<span data-ttu-id="a5927-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5927-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5927-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5927-126">Request body</span></span>
<span data-ttu-id="a5927-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5927-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5927-128">响应</span><span class="sxs-lookup"><span data-stu-id="a5927-128">Response</span></span>
<span data-ttu-id="a5927-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a5927-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5927-130">示例</span><span class="sxs-lookup"><span data-stu-id="a5927-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5927-131">请求</span><span class="sxs-lookup"><span data-stu-id="a5927-131">Request</span></span>
<span data-ttu-id="a5927-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5927-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="a5927-133">响应</span><span class="sxs-lookup"><span data-stu-id="a5927-133">Response</span></span>
<span data-ttu-id="a5927-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a5927-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




