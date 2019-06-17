---
title: 删除 securityBaselineTemplate
description: 删除 securityBaselineTemplate。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e71148aeb421283f1b8312c0f84710b761093ca
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959451"
---
# <a name="delete-securitybaselinetemplate"></a><span data-ttu-id="70478-103">删除 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="70478-103">Delete securityBaselineTemplate</span></span>

> <span data-ttu-id="70478-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70478-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70478-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70478-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70478-106">删除[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="70478-106">Deletes a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70478-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="70478-107">Prerequisites</span></span>
<span data-ttu-id="70478-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70478-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="70478-110">Permission type</span></span>|<span data-ttu-id="70478-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="70478-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70478-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70478-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70478-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70478-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70478-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70478-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70478-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="70478-115">Not supported.</span></span>|
|<span data-ttu-id="70478-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="70478-116">Application</span></span>|<span data-ttu-id="70478-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="70478-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70478-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70478-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/templates/{deviceManagementTemplateId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="70478-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="70478-119">Request headers</span></span>
|<span data-ttu-id="70478-120">标头</span><span class="sxs-lookup"><span data-stu-id="70478-120">Header</span></span>|<span data-ttu-id="70478-121">值</span><span class="sxs-lookup"><span data-stu-id="70478-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70478-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70478-122">Authorization</span></span>|<span data-ttu-id="70478-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70478-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70478-124">接受</span><span class="sxs-lookup"><span data-stu-id="70478-124">Accept</span></span>|<span data-ttu-id="70478-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70478-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70478-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70478-126">Request body</span></span>
<span data-ttu-id="70478-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70478-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70478-128">响应</span><span class="sxs-lookup"><span data-stu-id="70478-128">Response</span></span>
<span data-ttu-id="70478-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="70478-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70478-130">示例</span><span class="sxs-lookup"><span data-stu-id="70478-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="70478-131">请求</span><span class="sxs-lookup"><span data-stu-id="70478-131">Request</span></span>
<span data-ttu-id="70478-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70478-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="70478-133">响应</span><span class="sxs-lookup"><span data-stu-id="70478-133">Response</span></span>
<span data-ttu-id="70478-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70478-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





