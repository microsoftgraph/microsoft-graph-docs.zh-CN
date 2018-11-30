---
title: wipeManagedAppRegistrationsByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
ms.openlocfilehash: d6f56fa50b3162ecaebc0bb1adb02af3b4b0e9f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010170"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="8c172-103">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="8c172-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="8c172-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c172-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c172-105">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="8c172-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c172-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c172-106">Prerequisites</span></span>
<span data-ttu-id="8c172-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8c172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c172-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c172-109">Permission type</span></span>|<span data-ttu-id="8c172-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c172-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c172-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c172-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8c172-112">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="8c172-112">_varies by context_</span></span> |
| <span data-ttu-id="8c172-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="8c172-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="8c172-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c172-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="8c172-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c172-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c172-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c172-116">Not supported.</span></span>|
|<span data-ttu-id="8c172-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c172-117">Application</span></span>|<span data-ttu-id="8c172-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c172-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c172-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c172-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="8c172-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c172-120">Request headers</span></span>
|<span data-ttu-id="8c172-121">标头</span><span class="sxs-lookup"><span data-stu-id="8c172-121">Header</span></span>|<span data-ttu-id="8c172-122">值</span><span class="sxs-lookup"><span data-stu-id="8c172-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c172-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c172-123">Authorization</span></span>|<span data-ttu-id="8c172-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c172-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c172-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c172-125">Accept</span></span>|<span data-ttu-id="8c172-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c172-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c172-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c172-127">Request body</span></span>
<span data-ttu-id="8c172-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c172-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8c172-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="8c172-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8c172-130">属性</span><span class="sxs-lookup"><span data-stu-id="8c172-130">Property</span></span>|<span data-ttu-id="8c172-131">类型</span><span class="sxs-lookup"><span data-stu-id="8c172-131">Type</span></span>|<span data-ttu-id="8c172-132">说明</span><span class="sxs-lookup"><span data-stu-id="8c172-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c172-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8c172-133">deviceTag</span></span>|<span data-ttu-id="8c172-134">String</span><span class="sxs-lookup"><span data-stu-id="8c172-134">String</span></span>|<span data-ttu-id="8c172-135">设备标记</span><span class="sxs-lookup"><span data-stu-id="8c172-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="8c172-136">响应</span><span class="sxs-lookup"><span data-stu-id="8c172-136">Response</span></span>
<span data-ttu-id="8c172-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8c172-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c172-138">示例</span><span class="sxs-lookup"><span data-stu-id="8c172-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c172-139">请求</span><span class="sxs-lookup"><span data-stu-id="8c172-139">Request</span></span>
<span data-ttu-id="8c172-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c172-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="8c172-141">响应</span><span class="sxs-lookup"><span data-stu-id="8c172-141">Response</span></span>
<span data-ttu-id="8c172-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c172-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



