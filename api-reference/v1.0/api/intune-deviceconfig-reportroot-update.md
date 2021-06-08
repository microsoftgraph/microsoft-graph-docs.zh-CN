---
title: 更新 reportRoot
description: 更新 reportRoot 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef3ebef270c79af26a663c88cdc4857d5fb175fb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760738"
---
# <a name="update-reportroot"></a><span data-ttu-id="98ef8-103">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="98ef8-103">Update reportRoot</span></span>

<span data-ttu-id="98ef8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98ef8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98ef8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98ef8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98ef8-106">更新 [reportRoot](../resources/intune-deviceconfig-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="98ef8-106">Update the properties of a [reportRoot](../resources/intune-deviceconfig-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98ef8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="98ef8-107">Prerequisites</span></span>
<span data-ttu-id="98ef8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98ef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98ef8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="98ef8-110">Permission type</span></span>|<span data-ttu-id="98ef8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98ef8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98ef8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98ef8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98ef8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98ef8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98ef8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98ef8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98ef8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="98ef8-115">Not supported.</span></span>|
|<span data-ttu-id="98ef8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="98ef8-116">Application</span></span>|<span data-ttu-id="98ef8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98ef8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98ef8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98ef8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="98ef8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="98ef8-119">Request headers</span></span>
|<span data-ttu-id="98ef8-120">标头</span><span class="sxs-lookup"><span data-stu-id="98ef8-120">Header</span></span>|<span data-ttu-id="98ef8-121">值</span><span class="sxs-lookup"><span data-stu-id="98ef8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98ef8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98ef8-122">Authorization</span></span>|<span data-ttu-id="98ef8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="98ef8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98ef8-124">接受</span><span class="sxs-lookup"><span data-stu-id="98ef8-124">Accept</span></span>|<span data-ttu-id="98ef8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98ef8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98ef8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="98ef8-126">Request body</span></span>
<span data-ttu-id="98ef8-127">在请求正文中，提供 [reportRoot](../resources/intune-deviceconfig-reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98ef8-127">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-deviceconfig-reportroot.md) object.</span></span>

<span data-ttu-id="98ef8-128">下表显示了创建 [reportRoot](../resources/intune-deviceconfig-reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="98ef8-128">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-deviceconfig-reportroot.md).</span></span>

|<span data-ttu-id="98ef8-129">属性</span><span class="sxs-lookup"><span data-stu-id="98ef8-129">Property</span></span>|<span data-ttu-id="98ef8-130">类型</span><span class="sxs-lookup"><span data-stu-id="98ef8-130">Type</span></span>|<span data-ttu-id="98ef8-131">说明</span><span class="sxs-lookup"><span data-stu-id="98ef8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98ef8-132">id</span><span class="sxs-lookup"><span data-stu-id="98ef8-132">id</span></span>|<span data-ttu-id="98ef8-133">String</span><span class="sxs-lookup"><span data-stu-id="98ef8-133">String</span></span>|<span data-ttu-id="98ef8-134">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="98ef8-134">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="98ef8-135">响应</span><span class="sxs-lookup"><span data-stu-id="98ef8-135">Response</span></span>
<span data-ttu-id="98ef8-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune-deviceconfig-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98ef8-136">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-deviceconfig-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98ef8-137">示例</span><span class="sxs-lookup"><span data-stu-id="98ef8-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="98ef8-138">请求</span><span class="sxs-lookup"><span data-stu-id="98ef8-138">Request</span></span>
<span data-ttu-id="98ef8-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98ef8-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 52

{
  "@odata.type": "#microsoft.graph.reportRoot"
}
```

### <a name="response"></a><span data-ttu-id="98ef8-140">响应</span><span class="sxs-lookup"><span data-stu-id="98ef8-140">Response</span></span>
<span data-ttu-id="98ef8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98ef8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```




