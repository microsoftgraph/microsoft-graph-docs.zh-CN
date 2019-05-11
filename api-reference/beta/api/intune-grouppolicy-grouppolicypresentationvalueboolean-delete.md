---
title: 删除 groupPolicyPresentationValueBoolean
description: 删除 groupPolicyPresentationValueBoolean。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 616dc50cb217b910dcc5e334eafaa08d95f03b91
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904487"
---
# <a name="delete-grouppolicypresentationvalueboolean"></a><span data-ttu-id="0d2af-103">删除 groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="0d2af-103">Delete groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="0d2af-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d2af-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d2af-106">删除[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)。</span><span class="sxs-lookup"><span data-stu-id="0d2af-106">Deletes a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d2af-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0d2af-107">Prerequisites</span></span>
<span data-ttu-id="0d2af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d2af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d2af-110">Permission type</span></span>|<span data-ttu-id="0d2af-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0d2af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d2af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d2af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d2af-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d2af-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0d2af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d2af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d2af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d2af-115">Not supported.</span></span>|
|<span data-ttu-id="0d2af-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d2af-116">Application</span></span>|<span data-ttu-id="0d2af-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d2af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d2af-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d2af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="0d2af-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d2af-119">Request headers</span></span>
|<span data-ttu-id="0d2af-120">标头</span><span class="sxs-lookup"><span data-stu-id="0d2af-120">Header</span></span>|<span data-ttu-id="0d2af-121">值</span><span class="sxs-lookup"><span data-stu-id="0d2af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d2af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d2af-122">Authorization</span></span>|<span data-ttu-id="0d2af-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0d2af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d2af-124">接受</span><span class="sxs-lookup"><span data-stu-id="0d2af-124">Accept</span></span>|<span data-ttu-id="0d2af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d2af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d2af-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d2af-126">Request body</span></span>
<span data-ttu-id="0d2af-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d2af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d2af-128">响应</span><span class="sxs-lookup"><span data-stu-id="0d2af-128">Response</span></span>
<span data-ttu-id="0d2af-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0d2af-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d2af-130">示例</span><span class="sxs-lookup"><span data-stu-id="0d2af-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d2af-131">请求</span><span class="sxs-lookup"><span data-stu-id="0d2af-131">Request</span></span>
<span data-ttu-id="0d2af-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d2af-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="0d2af-133">响应</span><span class="sxs-lookup"><span data-stu-id="0d2af-133">Response</span></span>
<span data-ttu-id="0d2af-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d2af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




