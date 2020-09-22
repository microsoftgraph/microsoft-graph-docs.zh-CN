---
title: 更新 windowsInformationProtectionNetworkLearningSummary
description: 更新 windowsInformationProtectionNetworkLearningSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee4b9e2f6a1c0ec29c41d7073737a9448ebb9f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980104"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="3efde-103">更新 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="3efde-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="3efde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3efde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3efde-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3efde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3efde-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3efde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3efde-107">更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3efde-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3efde-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3efde-108">Prerequisites</span></span>
<span data-ttu-id="3efde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3efde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3efde-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3efde-111">Permission type</span></span>|<span data-ttu-id="3efde-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3efde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3efde-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3efde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3efde-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3efde-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3efde-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3efde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3efde-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3efde-116">Not supported.</span></span>|
|<span data-ttu-id="3efde-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3efde-117">Application</span></span>|<span data-ttu-id="3efde-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3efde-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3efde-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3efde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3efde-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3efde-120">Request headers</span></span>
|<span data-ttu-id="3efde-121">标头</span><span class="sxs-lookup"><span data-stu-id="3efde-121">Header</span></span>|<span data-ttu-id="3efde-122">值</span><span class="sxs-lookup"><span data-stu-id="3efde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3efde-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3efde-123">Authorization</span></span>|<span data-ttu-id="3efde-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3efde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3efde-125">接受</span><span class="sxs-lookup"><span data-stu-id="3efde-125">Accept</span></span>|<span data-ttu-id="3efde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3efde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3efde-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3efde-127">Request body</span></span>
<span data-ttu-id="3efde-128">在请求正文中，提供 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3efde-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="3efde-129">下表显示创建 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3efde-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="3efde-130">属性</span><span class="sxs-lookup"><span data-stu-id="3efde-130">Property</span></span>|<span data-ttu-id="3efde-131">类型</span><span class="sxs-lookup"><span data-stu-id="3efde-131">Type</span></span>|<span data-ttu-id="3efde-132">说明</span><span class="sxs-lookup"><span data-stu-id="3efde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3efde-133">id</span><span class="sxs-lookup"><span data-stu-id="3efde-133">id</span></span>|<span data-ttu-id="3efde-134">String</span><span class="sxs-lookup"><span data-stu-id="3efde-134">String</span></span>|<span data-ttu-id="3efde-135">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3efde-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="3efde-136">url</span><span class="sxs-lookup"><span data-stu-id="3efde-136">url</span></span>|<span data-ttu-id="3efde-137">String</span><span class="sxs-lookup"><span data-stu-id="3efde-137">String</span></span>|<span data-ttu-id="3efde-138">网站 URL</span><span class="sxs-lookup"><span data-stu-id="3efde-138">Website url</span></span>|
|<span data-ttu-id="3efde-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3efde-139">deviceCount</span></span>|<span data-ttu-id="3efde-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3efde-140">Int32</span></span>|<span data-ttu-id="3efde-141">设备计数</span><span class="sxs-lookup"><span data-stu-id="3efde-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="3efde-142">响应</span><span class="sxs-lookup"><span data-stu-id="3efde-142">Response</span></span>
<span data-ttu-id="3efde-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3efde-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3efde-144">示例</span><span class="sxs-lookup"><span data-stu-id="3efde-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3efde-145">请求</span><span class="sxs-lookup"><span data-stu-id="3efde-145">Request</span></span>
<span data-ttu-id="3efde-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3efde-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="3efde-147">响应</span><span class="sxs-lookup"><span data-stu-id="3efde-147">Response</span></span>
<span data-ttu-id="3efde-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3efde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```






