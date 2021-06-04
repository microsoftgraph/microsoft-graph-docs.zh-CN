---
title: 更新 reportRoot
description: 更新 reportRoot 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d67e334b0f9ff3329bfa3bdfbd5436527461d9f
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732422"
---
# <a name="update-reportroot"></a><span data-ttu-id="a95ad-103">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="a95ad-103">Update reportRoot</span></span>

<span data-ttu-id="a95ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a95ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a95ad-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a95ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a95ad-106">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a95ad-106">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a95ad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a95ad-107">Prerequisites</span></span>
<span data-ttu-id="a95ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a95ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a95ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a95ad-110">Permission type</span></span>|<span data-ttu-id="a95ad-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a95ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a95ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a95ad-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a95ad-113">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="a95ad-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="a95ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a95ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="a95ad-115">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="a95ad-115">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="a95ad-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a95ad-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a95ad-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a95ad-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a95ad-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a95ad-118">Not supported.</span></span>|
|<span data-ttu-id="a95ad-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a95ad-119">Application</span></span>|<span data-ttu-id="a95ad-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="a95ad-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a95ad-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a95ad-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="a95ad-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a95ad-122">Request headers</span></span>
|<span data-ttu-id="a95ad-123">标头</span><span class="sxs-lookup"><span data-stu-id="a95ad-123">Header</span></span>|<span data-ttu-id="a95ad-124">值</span><span class="sxs-lookup"><span data-stu-id="a95ad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a95ad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a95ad-125">Authorization</span></span>|<span data-ttu-id="a95ad-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a95ad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a95ad-127">接受</span><span class="sxs-lookup"><span data-stu-id="a95ad-127">Accept</span></span>|<span data-ttu-id="a95ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a95ad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a95ad-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a95ad-129">Request body</span></span>
<span data-ttu-id="a95ad-130">在请求正文中，提供 [reportRoot](../resources/intune-shared-reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a95ad-130">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="a95ad-131">下表显示了创建 [reportRoot](../resources/intune-shared-reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a95ad-131">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="a95ad-132">属性</span><span class="sxs-lookup"><span data-stu-id="a95ad-132">Property</span></span>|<span data-ttu-id="a95ad-133">类型</span><span class="sxs-lookup"><span data-stu-id="a95ad-133">Type</span></span>|<span data-ttu-id="a95ad-134">说明</span><span class="sxs-lookup"><span data-stu-id="a95ad-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a95ad-135">id</span><span class="sxs-lookup"><span data-stu-id="a95ad-135">id</span></span>|<span data-ttu-id="a95ad-136">String</span><span class="sxs-lookup"><span data-stu-id="a95ad-136">String</span></span>|<span data-ttu-id="a95ad-137">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a95ad-137">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a95ad-138">响应</span><span class="sxs-lookup"><span data-stu-id="a95ad-138">Response</span></span>
<span data-ttu-id="a95ad-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a95ad-139">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a95ad-140">示例</span><span class="sxs-lookup"><span data-stu-id="a95ad-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="a95ad-141">请求</span><span class="sxs-lookup"><span data-stu-id="a95ad-141">Request</span></span>
<span data-ttu-id="a95ad-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a95ad-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="a95ad-143">响应</span><span class="sxs-lookup"><span data-stu-id="a95ad-143">Response</span></span>
<span data-ttu-id="a95ad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a95ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```














