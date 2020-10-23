---
title: 删除 groupPolicyUploadedCategory
description: 删除 groupPolicyUploadedCategory。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb1374ed674f7ccd20b8fcd45023e754f6875bd2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695528"
---
# <a name="delete-grouppolicyuploadedcategory"></a><span data-ttu-id="c553a-103">删除 groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="c553a-103">Delete groupPolicyUploadedCategory</span></span>

<span data-ttu-id="c553a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c553a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c553a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c553a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c553a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c553a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c553a-107">删除 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="c553a-107">Deletes a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c553a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c553a-108">Prerequisites</span></span>
<span data-ttu-id="c553a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c553a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c553a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c553a-111">Permission type</span></span>|<span data-ttu-id="c553a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c553a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c553a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c553a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c553a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c553a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c553a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c553a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c553a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c553a-116">Not supported.</span></span>|
|<span data-ttu-id="c553a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c553a-117">Application</span></span>|<span data-ttu-id="c553a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c553a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c553a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c553a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/parent
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children/{groupPolicyCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="c553a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c553a-120">Request headers</span></span>
|<span data-ttu-id="c553a-121">标头</span><span class="sxs-lookup"><span data-stu-id="c553a-121">Header</span></span>|<span data-ttu-id="c553a-122">值</span><span class="sxs-lookup"><span data-stu-id="c553a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c553a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c553a-123">Authorization</span></span>|<span data-ttu-id="c553a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c553a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c553a-125">接受</span><span class="sxs-lookup"><span data-stu-id="c553a-125">Accept</span></span>|<span data-ttu-id="c553a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c553a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c553a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c553a-127">Request body</span></span>
<span data-ttu-id="c553a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c553a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c553a-129">响应</span><span class="sxs-lookup"><span data-stu-id="c553a-129">Response</span></span>
<span data-ttu-id="c553a-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c553a-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c553a-131">示例</span><span class="sxs-lookup"><span data-stu-id="c553a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c553a-132">请求</span><span class="sxs-lookup"><span data-stu-id="c553a-132">Request</span></span>
<span data-ttu-id="c553a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c553a-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
```

### <a name="response"></a><span data-ttu-id="c553a-134">响应</span><span class="sxs-lookup"><span data-stu-id="c553a-134">Response</span></span>
<span data-ttu-id="c553a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c553a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





