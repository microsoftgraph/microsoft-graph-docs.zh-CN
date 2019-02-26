---
title: 更新 reportRoot
description: 更新 reportRoot 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0039490379054ddb98c687957c1af0462a2e7f02
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255449"
---
# <a name="update-reportroot"></a><span data-ttu-id="8cb87-103">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="8cb87-103">Update reportRoot</span></span>

> <span data-ttu-id="8cb87-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8cb87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb87-105">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8cb87-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cb87-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8cb87-106">Prerequisites</span></span>
<span data-ttu-id="8cb87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cb87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb87-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cb87-109">Permission type</span></span>|<span data-ttu-id="8cb87-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8cb87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cb87-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cb87-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8cb87-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="8cb87-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="8cb87-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb87-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8cb87-114">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="8cb87-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="8cb87-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb87-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8cb87-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cb87-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cb87-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cb87-117">Not supported.</span></span>|
|<span data-ttu-id="8cb87-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cb87-118">Application</span></span>|<span data-ttu-id="8cb87-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cb87-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cb87-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cb87-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="8cb87-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cb87-121">Request headers</span></span>
|<span data-ttu-id="8cb87-122">标头</span><span class="sxs-lookup"><span data-stu-id="8cb87-122">Header</span></span>|<span data-ttu-id="8cb87-123">值</span><span class="sxs-lookup"><span data-stu-id="8cb87-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cb87-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb87-124">Authorization</span></span>|<span data-ttu-id="8cb87-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8cb87-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cb87-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8cb87-126">Accept</span></span>|<span data-ttu-id="8cb87-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8cb87-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cb87-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cb87-128">Request body</span></span>
<span data-ttu-id="8cb87-129">在请求正文中，提供 [reportRoot](../resources/intune-shared-reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cb87-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="8cb87-130">下表显示了创建 [reportRoot](../resources/intune-shared-reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8cb87-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="8cb87-131">属性</span><span class="sxs-lookup"><span data-stu-id="8cb87-131">Property</span></span>|<span data-ttu-id="8cb87-132">类型</span><span class="sxs-lookup"><span data-stu-id="8cb87-132">Type</span></span>|<span data-ttu-id="8cb87-133">说明</span><span class="sxs-lookup"><span data-stu-id="8cb87-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb87-134">id</span><span class="sxs-lookup"><span data-stu-id="8cb87-134">id</span></span>|<span data-ttu-id="8cb87-135">String</span><span class="sxs-lookup"><span data-stu-id="8cb87-135">String</span></span>|<span data-ttu-id="8cb87-136">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8cb87-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8cb87-137">响应</span><span class="sxs-lookup"><span data-stu-id="8cb87-137">Response</span></span>
<span data-ttu-id="8cb87-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8cb87-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb87-139">示例</span><span class="sxs-lookup"><span data-stu-id="8cb87-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cb87-140">请求</span><span class="sxs-lookup"><span data-stu-id="8cb87-140">Request</span></span>
<span data-ttu-id="8cb87-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8cb87-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="8cb87-142">响应</span><span class="sxs-lookup"><span data-stu-id="8cb87-142">Response</span></span>
<span data-ttu-id="8cb87-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8cb87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








