---
title: 更新 reportRoot
description: 更新 reportRoot 对象的属性。
author: tfitzmac
ms.openlocfilehash: 4f3d0e297a9b7d122e9b21afd7555c1af307d2d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349530"
---
# <a name="update-reportroot"></a><span data-ttu-id="edc94-103">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="edc94-103">Update reportRoot</span></span>

> <span data-ttu-id="edc94-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="edc94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edc94-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="edc94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edc94-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="edc94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edc94-107">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="edc94-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edc94-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="edc94-108">Prerequisites</span></span>
<span data-ttu-id="edc94-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="edc94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edc94-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="edc94-111">Permission type</span></span>|<span data-ttu-id="edc94-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="edc94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edc94-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edc94-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="edc94-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="edc94-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="edc94-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc94-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="edc94-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="edc94-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="edc94-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc94-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="edc94-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edc94-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edc94-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc94-119">Not supported.</span></span>|
|<span data-ttu-id="edc94-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="edc94-120">Application</span></span>|<span data-ttu-id="edc94-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc94-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edc94-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edc94-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="edc94-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="edc94-123">Request headers</span></span>
|<span data-ttu-id="edc94-124">标头</span><span class="sxs-lookup"><span data-stu-id="edc94-124">Header</span></span>|<span data-ttu-id="edc94-125">值</span><span class="sxs-lookup"><span data-stu-id="edc94-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edc94-126">授权</span><span class="sxs-lookup"><span data-stu-id="edc94-126">Authorization</span></span>|<span data-ttu-id="edc94-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="edc94-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edc94-128">Accept</span><span class="sxs-lookup"><span data-stu-id="edc94-128">Accept</span></span>|<span data-ttu-id="edc94-129">application/json</span><span class="sxs-lookup"><span data-stu-id="edc94-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edc94-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="edc94-130">Request body</span></span>
<span data-ttu-id="edc94-131">在请求正文中，提供 [reportRoot](../resources/intune-shared-reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc94-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="edc94-132">下表显示了创建 [reportRoot](../resources/intune-shared-reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="edc94-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="edc94-133">属性</span><span class="sxs-lookup"><span data-stu-id="edc94-133">Property</span></span>|<span data-ttu-id="edc94-134">类型</span><span class="sxs-lookup"><span data-stu-id="edc94-134">Type</span></span>|<span data-ttu-id="edc94-135">说明</span><span class="sxs-lookup"><span data-stu-id="edc94-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc94-136">id</span><span class="sxs-lookup"><span data-stu-id="edc94-136">id</span></span>|<span data-ttu-id="edc94-137">String</span><span class="sxs-lookup"><span data-stu-id="edc94-137">String</span></span>|<span data-ttu-id="edc94-138">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="edc94-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="edc94-139">响应</span><span class="sxs-lookup"><span data-stu-id="edc94-139">Response</span></span>
<span data-ttu-id="edc94-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edc94-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edc94-141">示例</span><span class="sxs-lookup"><span data-stu-id="edc94-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="edc94-142">请求</span><span class="sxs-lookup"><span data-stu-id="edc94-142">Request</span></span>
<span data-ttu-id="edc94-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="edc94-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="edc94-144">响应</span><span class="sxs-lookup"><span data-stu-id="edc94-144">Response</span></span>
<span data-ttu-id="edc94-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="edc94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



