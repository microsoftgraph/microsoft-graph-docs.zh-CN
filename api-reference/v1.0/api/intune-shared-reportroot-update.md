---
title: 更新 reportRoot
description: 更新 reportRoot 对象的属性。
ms.openlocfilehash: a376cd399fbcb36b369839dc214b3e792bc8d104
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009541"
---
# <a name="update-reportroot"></a><span data-ttu-id="95ec9-103">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="95ec9-103">Update reportRoot</span></span>

> <span data-ttu-id="95ec9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="95ec9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95ec9-105">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95ec9-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95ec9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="95ec9-106">Prerequisites</span></span>
<span data-ttu-id="95ec9-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="95ec9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95ec9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="95ec9-109">Permission type</span></span>|<span data-ttu-id="95ec9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95ec9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95ec9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95ec9-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="95ec9-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="95ec9-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="95ec9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95ec9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="95ec9-114">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="95ec9-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="95ec9-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95ec9-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="95ec9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95ec9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95ec9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="95ec9-117">Not supported.</span></span>|
|<span data-ttu-id="95ec9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="95ec9-118">Application</span></span>|<span data-ttu-id="95ec9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="95ec9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95ec9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95ec9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="95ec9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="95ec9-121">Request headers</span></span>
|<span data-ttu-id="95ec9-122">标头</span><span class="sxs-lookup"><span data-stu-id="95ec9-122">Header</span></span>|<span data-ttu-id="95ec9-123">值</span><span class="sxs-lookup"><span data-stu-id="95ec9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95ec9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="95ec9-124">Authorization</span></span>|<span data-ttu-id="95ec9-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95ec9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95ec9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="95ec9-126">Accept</span></span>|<span data-ttu-id="95ec9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="95ec9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95ec9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="95ec9-128">Request body</span></span>
<span data-ttu-id="95ec9-129">在请求正文中，提供 [reportRoot](../resources/intune-shared-reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95ec9-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="95ec9-130">下表显示了创建 [reportRoot](../resources/intune-shared-reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95ec9-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="95ec9-131">属性</span><span class="sxs-lookup"><span data-stu-id="95ec9-131">Property</span></span>|<span data-ttu-id="95ec9-132">类型</span><span class="sxs-lookup"><span data-stu-id="95ec9-132">Type</span></span>|<span data-ttu-id="95ec9-133">说明</span><span class="sxs-lookup"><span data-stu-id="95ec9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95ec9-134">id</span><span class="sxs-lookup"><span data-stu-id="95ec9-134">id</span></span>|<span data-ttu-id="95ec9-135">String</span><span class="sxs-lookup"><span data-stu-id="95ec9-135">String</span></span>|<span data-ttu-id="95ec9-136">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="95ec9-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="95ec9-137">响应</span><span class="sxs-lookup"><span data-stu-id="95ec9-137">Response</span></span>
<span data-ttu-id="95ec9-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95ec9-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95ec9-139">示例</span><span class="sxs-lookup"><span data-stu-id="95ec9-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="95ec9-140">请求</span><span class="sxs-lookup"><span data-stu-id="95ec9-140">Request</span></span>
<span data-ttu-id="95ec9-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95ec9-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="95ec9-142">响应</span><span class="sxs-lookup"><span data-stu-id="95ec9-142">Response</span></span>
<span data-ttu-id="95ec9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95ec9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








