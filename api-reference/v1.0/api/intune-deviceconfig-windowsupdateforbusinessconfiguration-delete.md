---
title: 删除 windowsUpdateForBusinessConfiguration
description: 删除 windowsUpdateForBusinessConfiguration。
author: tfitzmac
ms.openlocfilehash: 24ecae6bfa1fd00fa3a8c220e084db6062b67e6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301587"
---
# <a name="delete-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="d9125-103">删除 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9125-103">Delete windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="d9125-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9125-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9125-105">删除 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d9125-105">Deletes a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9125-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9125-106">Prerequisites</span></span>
<span data-ttu-id="d9125-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d9125-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9125-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9125-109">Permission type</span></span>|<span data-ttu-id="d9125-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9125-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9125-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9125-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9125-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9125-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9125-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9125-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9125-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9125-114">Not supported.</span></span>|
|<span data-ttu-id="d9125-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9125-115">Application</span></span>|<span data-ttu-id="d9125-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9125-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9125-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9125-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d9125-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9125-118">Request headers</span></span>
|<span data-ttu-id="d9125-119">标头</span><span class="sxs-lookup"><span data-stu-id="d9125-119">Header</span></span>|<span data-ttu-id="d9125-120">值</span><span class="sxs-lookup"><span data-stu-id="d9125-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9125-121">授权</span><span class="sxs-lookup"><span data-stu-id="d9125-121">Authorization</span></span>|<span data-ttu-id="d9125-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9125-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9125-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d9125-123">Accept</span></span>|<span data-ttu-id="d9125-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9125-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9125-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9125-125">Request body</span></span>
<span data-ttu-id="d9125-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9125-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9125-127">响应</span><span class="sxs-lookup"><span data-stu-id="d9125-127">Response</span></span>
<span data-ttu-id="d9125-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d9125-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9125-129">示例</span><span class="sxs-lookup"><span data-stu-id="d9125-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9125-130">请求</span><span class="sxs-lookup"><span data-stu-id="d9125-130">Request</span></span>
<span data-ttu-id="d9125-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9125-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d9125-132">响应</span><span class="sxs-lookup"><span data-stu-id="d9125-132">Response</span></span>
<span data-ttu-id="d9125-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9125-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



