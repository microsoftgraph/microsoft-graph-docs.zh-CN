---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a636e407b0fbe01f2fe6341dd09f675e1a5af6e3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751843"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="be91d-103">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="be91d-103">Update deviceAppManagement</span></span>

<span data-ttu-id="be91d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be91d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be91d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be91d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be91d-106">更新 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be91d-106">Update the properties of a [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be91d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="be91d-107">Prerequisites</span></span>
<span data-ttu-id="be91d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be91d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be91d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="be91d-110">Permission type</span></span>|<span data-ttu-id="be91d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be91d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be91d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be91d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be91d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be91d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be91d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be91d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be91d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be91d-115">Not supported.</span></span>|
|<span data-ttu-id="be91d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="be91d-116">Application</span></span>|<span data-ttu-id="be91d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be91d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be91d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be91d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="be91d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="be91d-119">Request headers</span></span>
|<span data-ttu-id="be91d-120">标头</span><span class="sxs-lookup"><span data-stu-id="be91d-120">Header</span></span>|<span data-ttu-id="be91d-121">值</span><span class="sxs-lookup"><span data-stu-id="be91d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be91d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be91d-122">Authorization</span></span>|<span data-ttu-id="be91d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be91d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be91d-124">接受</span><span class="sxs-lookup"><span data-stu-id="be91d-124">Accept</span></span>|<span data-ttu-id="be91d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be91d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be91d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="be91d-126">Request body</span></span>
<span data-ttu-id="be91d-127">在请求正文中，提供 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be91d-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="be91d-128">下表显示创建 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be91d-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md).</span></span>

|<span data-ttu-id="be91d-129">属性</span><span class="sxs-lookup"><span data-stu-id="be91d-129">Property</span></span>|<span data-ttu-id="be91d-130">类型</span><span class="sxs-lookup"><span data-stu-id="be91d-130">Type</span></span>|<span data-ttu-id="be91d-131">说明</span><span class="sxs-lookup"><span data-stu-id="be91d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be91d-132">id</span><span class="sxs-lookup"><span data-stu-id="be91d-132">id</span></span>|<span data-ttu-id="be91d-133">String</span><span class="sxs-lookup"><span data-stu-id="be91d-133">String</span></span>|<span data-ttu-id="be91d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be91d-134">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="be91d-135">响应</span><span class="sxs-lookup"><span data-stu-id="be91d-135">Response</span></span>
<span data-ttu-id="be91d-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be91d-136">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be91d-137">示例</span><span class="sxs-lookup"><span data-stu-id="be91d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="be91d-138">请求</span><span class="sxs-lookup"><span data-stu-id="be91d-138">Request</span></span>
<span data-ttu-id="be91d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be91d-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 61

{
  "@odata.type": "#microsoft.graph.deviceAppManagement"
}
```

### <a name="response"></a><span data-ttu-id="be91d-140">响应</span><span class="sxs-lookup"><span data-stu-id="be91d-140">Response</span></span>
<span data-ttu-id="be91d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be91d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```




