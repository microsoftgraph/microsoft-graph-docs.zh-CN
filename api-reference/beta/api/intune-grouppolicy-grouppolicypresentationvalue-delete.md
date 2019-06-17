---
title: 删除 groupPolicyPresentationValue
description: 删除 groupPolicyPresentationValue。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2928438c8fdf88f8237ef78fe9a7053f37e33cc6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965989"
---
# <a name="delete-grouppolicypresentationvalue"></a><span data-ttu-id="54997-103">删除 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="54997-103">Delete groupPolicyPresentationValue</span></span>

> <span data-ttu-id="54997-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54997-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54997-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54997-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54997-106">删除[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="54997-106">Deletes a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54997-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="54997-107">Prerequisites</span></span>
<span data-ttu-id="54997-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54997-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="54997-110">Permission type</span></span>|<span data-ttu-id="54997-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="54997-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54997-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54997-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54997-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54997-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54997-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54997-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54997-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="54997-115">Not supported.</span></span>|
|<span data-ttu-id="54997-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="54997-116">Application</span></span>|<span data-ttu-id="54997-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="54997-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54997-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54997-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="54997-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54997-119">Request headers</span></span>
|<span data-ttu-id="54997-120">标头</span><span class="sxs-lookup"><span data-stu-id="54997-120">Header</span></span>|<span data-ttu-id="54997-121">值</span><span class="sxs-lookup"><span data-stu-id="54997-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54997-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54997-122">Authorization</span></span>|<span data-ttu-id="54997-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54997-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54997-124">接受</span><span class="sxs-lookup"><span data-stu-id="54997-124">Accept</span></span>|<span data-ttu-id="54997-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54997-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54997-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="54997-126">Request body</span></span>
<span data-ttu-id="54997-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54997-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54997-128">响应</span><span class="sxs-lookup"><span data-stu-id="54997-128">Response</span></span>
<span data-ttu-id="54997-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="54997-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="54997-130">示例</span><span class="sxs-lookup"><span data-stu-id="54997-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="54997-131">请求</span><span class="sxs-lookup"><span data-stu-id="54997-131">Request</span></span>
<span data-ttu-id="54997-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54997-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="54997-133">响应</span><span class="sxs-lookup"><span data-stu-id="54997-133">Response</span></span>
<span data-ttu-id="54997-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54997-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





