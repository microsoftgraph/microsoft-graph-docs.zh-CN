---
title: 删除 windowsOfficeClientConfiguration
description: 删除特定的非安全策略。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0d9ebcdbccd11576fd418a4962001da19063f4d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753052"
---
# <a name="delete-windowsofficeclientconfiguration"></a><span data-ttu-id="828de-103">删除 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="828de-103">Delete windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="828de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="828de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="828de-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="828de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="828de-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="828de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="828de-107">删除特定的非安全策略。</span><span class="sxs-lookup"><span data-stu-id="828de-107">Delete a specific non-security policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="828de-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="828de-108">Prerequisites</span></span>
<span data-ttu-id="828de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="828de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="828de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="828de-111">Permission type</span></span>|<span data-ttu-id="828de-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="828de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="828de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="828de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="828de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="828de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="828de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="828de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="828de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="828de-116">Not supported.</span></span>|
|<span data-ttu-id="828de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="828de-117">Application</span></span>|<span data-ttu-id="828de-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="828de-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="828de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="828de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="828de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="828de-120">Request headers</span></span>
|<span data-ttu-id="828de-121">标头</span><span class="sxs-lookup"><span data-stu-id="828de-121">Header</span></span>|<span data-ttu-id="828de-122">值</span><span class="sxs-lookup"><span data-stu-id="828de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="828de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="828de-123">Authorization</span></span>|<span data-ttu-id="828de-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="828de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="828de-125">接受</span><span class="sxs-lookup"><span data-stu-id="828de-125">Accept</span></span>|<span data-ttu-id="828de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="828de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="828de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="828de-127">Request body</span></span>
<span data-ttu-id="828de-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="828de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="828de-129">响应</span><span class="sxs-lookup"><span data-stu-id="828de-129">Response</span></span>
<span data-ttu-id="828de-130">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="828de-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="828de-131">示例</span><span class="sxs-lookup"><span data-stu-id="828de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="828de-132">请求</span><span class="sxs-lookup"><span data-stu-id="828de-132">Request</span></span>
<span data-ttu-id="828de-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="828de-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="828de-134">响应</span><span class="sxs-lookup"><span data-stu-id="828de-134">Response</span></span>
<span data-ttu-id="828de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="828de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




