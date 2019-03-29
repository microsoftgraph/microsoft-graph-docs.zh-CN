---
title: 删除 groupPolicyPresentationTextBox
description: 删除 groupPolicyPresentationTextBox。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86ea8ae426a74a291b9be50d5f8631553964cf6f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958282"
---
# <a name="delete-grouppolicypresentationtextbox"></a><span data-ttu-id="4711a-103">删除 groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="4711a-103">Delete groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="4711a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4711a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4711a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4711a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4711a-106">删除[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)。</span><span class="sxs-lookup"><span data-stu-id="4711a-106">Deletes a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4711a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4711a-107">Prerequisites</span></span>
<span data-ttu-id="4711a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4711a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4711a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4711a-110">Permission type</span></span>|<span data-ttu-id="4711a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4711a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4711a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4711a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4711a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4711a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4711a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4711a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4711a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4711a-115">Not supported.</span></span>|
|<span data-ttu-id="4711a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4711a-116">Application</span></span>|<span data-ttu-id="4711a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4711a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4711a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4711a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="4711a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4711a-119">Request headers</span></span>
|<span data-ttu-id="4711a-120">标头</span><span class="sxs-lookup"><span data-stu-id="4711a-120">Header</span></span>|<span data-ttu-id="4711a-121">值</span><span class="sxs-lookup"><span data-stu-id="4711a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4711a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4711a-122">Authorization</span></span>|<span data-ttu-id="4711a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4711a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4711a-124">接受</span><span class="sxs-lookup"><span data-stu-id="4711a-124">Accept</span></span>|<span data-ttu-id="4711a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4711a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4711a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4711a-126">Request body</span></span>
<span data-ttu-id="4711a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4711a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4711a-128">响应</span><span class="sxs-lookup"><span data-stu-id="4711a-128">Response</span></span>
<span data-ttu-id="4711a-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4711a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4711a-130">示例</span><span class="sxs-lookup"><span data-stu-id="4711a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4711a-131">请求</span><span class="sxs-lookup"><span data-stu-id="4711a-131">Request</span></span>
<span data-ttu-id="4711a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4711a-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="4711a-133">响应</span><span class="sxs-lookup"><span data-stu-id="4711a-133">Response</span></span>
<span data-ttu-id="4711a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4711a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




