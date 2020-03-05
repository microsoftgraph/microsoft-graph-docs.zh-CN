---
title: 删除 officeClientConfigurationAssignment
description: 删除 officeClientConfigurationAssignment。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc42c8cabb7328f43865fb10985b367f2aa2901d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444439"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="cd498-103">删除 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cd498-103">Delete officeClientConfigurationAssignment</span></span>

<span data-ttu-id="cd498-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cd498-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd498-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd498-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd498-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd498-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd498-107">删除[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="cd498-107">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd498-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd498-108">Prerequisites</span></span>
<span data-ttu-id="cd498-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd498-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd498-111">Permission type</span></span>|<span data-ttu-id="cd498-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd498-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd498-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd498-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd498-114">\* \* TODO：确定作用域 \* \*</span><span class="sxs-lookup"><span data-stu-id="cd498-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="cd498-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd498-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd498-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd498-116">Not supported.</span></span>|
|<span data-ttu-id="cd498-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd498-117">Application</span></span>|<span data-ttu-id="cd498-118">\* \* TODO：确定作用域 \* \*</span><span class="sxs-lookup"><span data-stu-id="cd498-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd498-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd498-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cd498-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd498-120">Request headers</span></span>
|<span data-ttu-id="cd498-121">标头</span><span class="sxs-lookup"><span data-stu-id="cd498-121">Header</span></span>|<span data-ttu-id="cd498-122">值</span><span class="sxs-lookup"><span data-stu-id="cd498-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd498-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd498-123">Authorization</span></span>|<span data-ttu-id="cd498-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd498-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd498-125">接受</span><span class="sxs-lookup"><span data-stu-id="cd498-125">Accept</span></span>|<span data-ttu-id="cd498-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd498-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd498-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd498-127">Request body</span></span>
<span data-ttu-id="cd498-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd498-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd498-129">响应</span><span class="sxs-lookup"><span data-stu-id="cd498-129">Response</span></span>
<span data-ttu-id="cd498-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cd498-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd498-131">示例</span><span class="sxs-lookup"><span data-stu-id="cd498-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd498-132">请求</span><span class="sxs-lookup"><span data-stu-id="cd498-132">Request</span></span>
<span data-ttu-id="cd498-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd498-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="cd498-134">响应</span><span class="sxs-lookup"><span data-stu-id="cd498-134">Response</span></span>
<span data-ttu-id="cd498-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd498-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





