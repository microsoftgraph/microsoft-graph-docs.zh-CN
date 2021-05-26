---
title: 删除 windowsOfficeClientConfiguration
description: 删除特定的非安全策略。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0d9ebcdbccd11576fd418a4962001da19063f4d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666824"
---
# <a name="delete-windowsofficeclientconfiguration"></a><span data-ttu-id="f0404-103">删除 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0404-103">Delete windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="f0404-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0404-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0404-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0404-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0404-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0404-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0404-107">删除特定的非安全策略。</span><span class="sxs-lookup"><span data-stu-id="f0404-107">Delete a specific non-security policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0404-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0404-108">Prerequisites</span></span>
<span data-ttu-id="f0404-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0404-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0404-111">Permission type</span></span>|<span data-ttu-id="f0404-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0404-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0404-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0404-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0404-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0404-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0404-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0404-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0404-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0404-116">Not supported.</span></span>|
|<span data-ttu-id="f0404-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0404-117">Application</span></span>|<span data-ttu-id="f0404-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0404-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0404-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0404-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="f0404-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0404-120">Request headers</span></span>
|<span data-ttu-id="f0404-121">标头</span><span class="sxs-lookup"><span data-stu-id="f0404-121">Header</span></span>|<span data-ttu-id="f0404-122">值</span><span class="sxs-lookup"><span data-stu-id="f0404-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0404-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0404-123">Authorization</span></span>|<span data-ttu-id="f0404-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0404-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0404-125">接受</span><span class="sxs-lookup"><span data-stu-id="f0404-125">Accept</span></span>|<span data-ttu-id="f0404-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0404-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0404-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0404-127">Request body</span></span>
<span data-ttu-id="f0404-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0404-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0404-129">响应</span><span class="sxs-lookup"><span data-stu-id="f0404-129">Response</span></span>
<span data-ttu-id="f0404-130">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f0404-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f0404-131">示例</span><span class="sxs-lookup"><span data-stu-id="f0404-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0404-132">请求</span><span class="sxs-lookup"><span data-stu-id="f0404-132">Request</span></span>
<span data-ttu-id="f0404-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0404-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="f0404-134">响应</span><span class="sxs-lookup"><span data-stu-id="f0404-134">Response</span></span>
<span data-ttu-id="f0404-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0404-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




