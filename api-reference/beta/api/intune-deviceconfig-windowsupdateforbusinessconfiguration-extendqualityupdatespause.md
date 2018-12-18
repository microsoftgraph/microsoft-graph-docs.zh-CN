---
title: extendQualityUpdatesPause 操作
description: 扩展的业务拨打 Windows Update 质量更新暂停。
author: tfitzmac
ms.openlocfilehash: ea6f36922b438e5f643e073c4d5d2697a6f77efc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355606"
---
# <a name="extendqualityupdatespause-action"></a><span data-ttu-id="f1548-103">extendQualityUpdatesPause 操作</span><span class="sxs-lookup"><span data-stu-id="f1548-103">extendQualityUpdatesPause action</span></span>

> <span data-ttu-id="f1548-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1548-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1548-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1548-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1548-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1548-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1548-107">扩展的业务拨打 Windows Update 质量更新暂停。</span><span class="sxs-lookup"><span data-stu-id="f1548-107">Extend Quality Updates Pause for a Windows Update for Business ring.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1548-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1548-108">Prerequisites</span></span>
<span data-ttu-id="f1548-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f1548-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1548-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1548-111">Permission type</span></span>|<span data-ttu-id="f1548-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1548-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1548-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1548-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1548-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1548-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1548-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1548-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1548-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1548-116">Not supported.</span></span>|
|<span data-ttu-id="f1548-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1548-117">Application</span></span>|<span data-ttu-id="f1548-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1548-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1548-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1548-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="f1548-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1548-120">Request headers</span></span>
|<span data-ttu-id="f1548-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1548-121">Header</span></span>|<span data-ttu-id="f1548-122">值</span><span class="sxs-lookup"><span data-stu-id="f1548-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1548-123">授权</span><span class="sxs-lookup"><span data-stu-id="f1548-123">Authorization</span></span>|<span data-ttu-id="f1548-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1548-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1548-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1548-125">Accept</span></span>|<span data-ttu-id="f1548-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1548-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1548-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1548-127">Request body</span></span>
<span data-ttu-id="f1548-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1548-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1548-129">响应</span><span class="sxs-lookup"><span data-stu-id="f1548-129">Response</span></span>
<span data-ttu-id="f1548-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f1548-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1548-131">示例</span><span class="sxs-lookup"><span data-stu-id="f1548-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1548-132">请求</span><span class="sxs-lookup"><span data-stu-id="f1548-132">Request</span></span>
<span data-ttu-id="f1548-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1548-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

### <a name="response"></a><span data-ttu-id="f1548-134">响应</span><span class="sxs-lookup"><span data-stu-id="f1548-134">Response</span></span>
<span data-ttu-id="f1548-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1548-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





