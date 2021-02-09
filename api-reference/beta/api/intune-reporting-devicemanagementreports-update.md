---
title: 更新 deviceManagementReports
description: 更新 deviceManagementReports 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4282a518e5594c88b421a301e7377fa2973e504c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159246"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="44afc-103">更新 deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="44afc-103">Update deviceManagementReports</span></span>

<span data-ttu-id="44afc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44afc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44afc-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44afc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44afc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44afc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44afc-107">更新 [deviceManagementReports 对象](../resources/intune-reporting-devicemanagementreports.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="44afc-107">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44afc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44afc-108">Prerequisites</span></span>
<span data-ttu-id="44afc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44afc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44afc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44afc-111">Permission type</span></span>|<span data-ttu-id="44afc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44afc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44afc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44afc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44afc-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44afc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44afc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44afc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44afc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44afc-116">Not supported.</span></span>|
|<span data-ttu-id="44afc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="44afc-117">Application</span></span>|<span data-ttu-id="44afc-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44afc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44afc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44afc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="44afc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44afc-120">Request headers</span></span>
|<span data-ttu-id="44afc-121">标头</span><span class="sxs-lookup"><span data-stu-id="44afc-121">Header</span></span>|<span data-ttu-id="44afc-122">值</span><span class="sxs-lookup"><span data-stu-id="44afc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44afc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44afc-123">Authorization</span></span>|<span data-ttu-id="44afc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44afc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44afc-125">接受</span><span class="sxs-lookup"><span data-stu-id="44afc-125">Accept</span></span>|<span data-ttu-id="44afc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44afc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44afc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44afc-127">Request body</span></span>
<span data-ttu-id="44afc-128">在请求正文中，提供 [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44afc-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="44afc-129">下表显示创建 [deviceManagementReports 时所需的属性](../resources/intune-reporting-devicemanagementreports.md)。</span><span class="sxs-lookup"><span data-stu-id="44afc-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="44afc-130">属性</span><span class="sxs-lookup"><span data-stu-id="44afc-130">Property</span></span>|<span data-ttu-id="44afc-131">类型</span><span class="sxs-lookup"><span data-stu-id="44afc-131">Type</span></span>|<span data-ttu-id="44afc-132">说明</span><span class="sxs-lookup"><span data-stu-id="44afc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44afc-133">id</span><span class="sxs-lookup"><span data-stu-id="44afc-133">id</span></span>|<span data-ttu-id="44afc-134">String</span><span class="sxs-lookup"><span data-stu-id="44afc-134">String</span></span>|<span data-ttu-id="44afc-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="44afc-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="44afc-136">响应</span><span class="sxs-lookup"><span data-stu-id="44afc-136">Response</span></span>
<span data-ttu-id="44afc-137">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44afc-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44afc-138">示例</span><span class="sxs-lookup"><span data-stu-id="44afc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="44afc-139">请求</span><span class="sxs-lookup"><span data-stu-id="44afc-139">Request</span></span>
<span data-ttu-id="44afc-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44afc-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="44afc-141">响应</span><span class="sxs-lookup"><span data-stu-id="44afc-141">Response</span></span>
<span data-ttu-id="44afc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44afc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




