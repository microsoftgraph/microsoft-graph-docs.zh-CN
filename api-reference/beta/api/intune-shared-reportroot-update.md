---
title: 更新 reportRoot
description: 更新 reportRoot 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 930300d1d657ccb795597193ab414e4248500641
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537914"
---
# <a name="update-reportroot"></a><span data-ttu-id="dc138-103">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="dc138-103">Update reportRoot</span></span>

> <span data-ttu-id="dc138-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dc138-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dc138-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dc138-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc138-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc138-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc138-107">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc138-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc138-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dc138-108">Prerequisites</span></span>
<span data-ttu-id="dc138-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc138-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc138-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc138-111">Permission type</span></span>|<span data-ttu-id="dc138-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dc138-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc138-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc138-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dc138-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="dc138-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="dc138-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc138-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="dc138-116">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="dc138-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="dc138-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc138-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dc138-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc138-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc138-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc138-119">Not supported.</span></span>|
|<span data-ttu-id="dc138-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc138-120">Application</span></span>||
| <span data-ttu-id="dc138-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="dc138-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="dc138-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc138-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="dc138-123">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="dc138-123">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="dc138-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc138-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc138-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc138-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="dc138-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc138-126">Request headers</span></span>
|<span data-ttu-id="dc138-127">标头</span><span class="sxs-lookup"><span data-stu-id="dc138-127">Header</span></span>|<span data-ttu-id="dc138-128">值</span><span class="sxs-lookup"><span data-stu-id="dc138-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc138-129">授权</span><span class="sxs-lookup"><span data-stu-id="dc138-129">Authorization</span></span>|<span data-ttu-id="dc138-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dc138-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc138-131">接受</span><span class="sxs-lookup"><span data-stu-id="dc138-131">Accept</span></span>|<span data-ttu-id="dc138-132">application/json</span><span class="sxs-lookup"><span data-stu-id="dc138-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc138-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc138-133">Request body</span></span>
<span data-ttu-id="dc138-134">在请求正文中，提供 [reportRoot](../resources/intune-shared-reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc138-134">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="dc138-135">下表显示了创建 [reportRoot](../resources/intune-shared-reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dc138-135">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="dc138-136">属性</span><span class="sxs-lookup"><span data-stu-id="dc138-136">Property</span></span>|<span data-ttu-id="dc138-137">类型</span><span class="sxs-lookup"><span data-stu-id="dc138-137">Type</span></span>|<span data-ttu-id="dc138-138">说明</span><span class="sxs-lookup"><span data-stu-id="dc138-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc138-139">id</span><span class="sxs-lookup"><span data-stu-id="dc138-139">id</span></span>|<span data-ttu-id="dc138-140">字符串</span><span class="sxs-lookup"><span data-stu-id="dc138-140">String</span></span>|<span data-ttu-id="dc138-141">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dc138-141">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="dc138-142">响应</span><span class="sxs-lookup"><span data-stu-id="dc138-142">Response</span></span>
<span data-ttu-id="dc138-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc138-143">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc138-144">示例</span><span class="sxs-lookup"><span data-stu-id="dc138-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc138-145">请求</span><span class="sxs-lookup"><span data-stu-id="dc138-145">Request</span></span>
<span data-ttu-id="dc138-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc138-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="dc138-147">响应</span><span class="sxs-lookup"><span data-stu-id="dc138-147">Response</span></span>
<span data-ttu-id="dc138-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc138-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```









