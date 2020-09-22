---
title: 删除 officeClientConfigurationAssignment
description: 删除 officeClientConfigurationAssignment。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5c42d2819147dada0e953899ec4cdfb015389a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975295"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="eacce-103">删除 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eacce-103">Delete officeClientConfigurationAssignment</span></span>

<span data-ttu-id="eacce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eacce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eacce-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eacce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eacce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eacce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eacce-107">删除 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="eacce-107">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eacce-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eacce-108">Prerequisites</span></span>
<span data-ttu-id="eacce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eacce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eacce-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eacce-111">Permission type</span></span>|<span data-ttu-id="eacce-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eacce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eacce-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eacce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eacce-114">\* \* TODO：确定作用域 \* \*</span><span class="sxs-lookup"><span data-stu-id="eacce-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="eacce-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eacce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eacce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eacce-116">Not supported.</span></span>|
|<span data-ttu-id="eacce-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eacce-117">Application</span></span>|<span data-ttu-id="eacce-118">\* \* TODO：确定作用域 \* \*</span><span class="sxs-lookup"><span data-stu-id="eacce-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="eacce-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eacce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="eacce-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eacce-120">Request headers</span></span>
|<span data-ttu-id="eacce-121">标头</span><span class="sxs-lookup"><span data-stu-id="eacce-121">Header</span></span>|<span data-ttu-id="eacce-122">值</span><span class="sxs-lookup"><span data-stu-id="eacce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eacce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eacce-123">Authorization</span></span>|<span data-ttu-id="eacce-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eacce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eacce-125">接受</span><span class="sxs-lookup"><span data-stu-id="eacce-125">Accept</span></span>|<span data-ttu-id="eacce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eacce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eacce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eacce-127">Request body</span></span>
<span data-ttu-id="eacce-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eacce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eacce-129">响应</span><span class="sxs-lookup"><span data-stu-id="eacce-129">Response</span></span>
<span data-ttu-id="eacce-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eacce-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eacce-131">示例</span><span class="sxs-lookup"><span data-stu-id="eacce-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eacce-132">请求</span><span class="sxs-lookup"><span data-stu-id="eacce-132">Request</span></span>
<span data-ttu-id="eacce-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eacce-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="eacce-134">响应</span><span class="sxs-lookup"><span data-stu-id="eacce-134">Response</span></span>
<span data-ttu-id="eacce-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eacce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






