---
title: 获取用户
description: 读取 user 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: b58485112929f39be76f1f908f3097d8971ac564
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303302"
---
# <a name="get-user"></a><span data-ttu-id="1a190-103">获取 user</span><span class="sxs-lookup"><span data-stu-id="1a190-103">Get user</span></span>

> <span data-ttu-id="1a190-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1a190-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a190-105">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a190-105">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a190-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a190-106">Prerequisites</span></span>
<span data-ttu-id="1a190-107">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1a190-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1a190-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a190-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="1a190-109">特定权限取决于的上下文。</span><span class="sxs-lookup"><span data-stu-id="1a190-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="1a190-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a190-110">Permission type</span></span>|<span data-ttu-id="1a190-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a190-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a190-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a190-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1a190-113">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="1a190-113">_varies by context_</span></span>|
| <span data-ttu-id="1a190-114">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="1a190-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="1a190-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a190-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="1a190-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="1a190-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="1a190-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a190-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="1a190-118">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="1a190-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="1a190-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a190-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1a190-120">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="1a190-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="1a190-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a190-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="1a190-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a190-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a190-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a190-123">Not supported.</span></span>|
|<span data-ttu-id="1a190-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a190-124">Application</span></span>|<span data-ttu-id="1a190-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a190-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a190-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a190-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a190-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a190-127">Optional query parameters</span></span>
<span data-ttu-id="1a190-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1a190-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1a190-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a190-129">Request headers</span></span>
|<span data-ttu-id="1a190-130">标头</span><span class="sxs-lookup"><span data-stu-id="1a190-130">Header</span></span>|<span data-ttu-id="1a190-131">值</span><span class="sxs-lookup"><span data-stu-id="1a190-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a190-132">授权</span><span class="sxs-lookup"><span data-stu-id="1a190-132">Authorization</span></span>|<span data-ttu-id="1a190-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a190-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a190-134">Accept</span><span class="sxs-lookup"><span data-stu-id="1a190-134">Accept</span></span>|<span data-ttu-id="1a190-135">application/json</span><span class="sxs-lookup"><span data-stu-id="1a190-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a190-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a190-136">Request body</span></span>
<span data-ttu-id="1a190-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a190-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a190-138">响应</span><span class="sxs-lookup"><span data-stu-id="1a190-138">Response</span></span>
<span data-ttu-id="1a190-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a190-139">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a190-140">示例</span><span class="sxs-lookup"><span data-stu-id="1a190-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a190-141">请求</span><span class="sxs-lookup"><span data-stu-id="1a190-141">Request</span></span>
<span data-ttu-id="1a190-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a190-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="1a190-143">响应</span><span class="sxs-lookup"><span data-stu-id="1a190-143">Response</span></span>
<span data-ttu-id="1a190-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a190-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



