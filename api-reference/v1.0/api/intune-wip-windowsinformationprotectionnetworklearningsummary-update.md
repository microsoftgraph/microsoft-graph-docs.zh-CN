---
title: 更新 windowsInformationProtectionNetworkLearningSummary
description: 更新 windowsInformationProtectionNetworkLearningSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54a0e5b33cd8897f6b0b243baca2ebb7bb91f0f4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751424"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="dd59f-103">更新 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="dd59f-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="dd59f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd59f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd59f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd59f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd59f-106">更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dd59f-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd59f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd59f-107">Prerequisites</span></span>
<span data-ttu-id="dd59f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd59f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd59f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd59f-110">Permission type</span></span>|<span data-ttu-id="dd59f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd59f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd59f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd59f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd59f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd59f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd59f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd59f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd59f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd59f-115">Not supported.</span></span>|
|<span data-ttu-id="dd59f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd59f-116">Application</span></span>|<span data-ttu-id="dd59f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd59f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd59f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd59f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="dd59f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd59f-119">Request headers</span></span>
|<span data-ttu-id="dd59f-120">标头</span><span class="sxs-lookup"><span data-stu-id="dd59f-120">Header</span></span>|<span data-ttu-id="dd59f-121">值</span><span class="sxs-lookup"><span data-stu-id="dd59f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd59f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd59f-122">Authorization</span></span>|<span data-ttu-id="dd59f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd59f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd59f-124">接受</span><span class="sxs-lookup"><span data-stu-id="dd59f-124">Accept</span></span>|<span data-ttu-id="dd59f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd59f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd59f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd59f-126">Request body</span></span>
<span data-ttu-id="dd59f-127">在请求正文中，提供 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd59f-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="dd59f-128">下表显示创建 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dd59f-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="dd59f-129">属性</span><span class="sxs-lookup"><span data-stu-id="dd59f-129">Property</span></span>|<span data-ttu-id="dd59f-130">类型</span><span class="sxs-lookup"><span data-stu-id="dd59f-130">Type</span></span>|<span data-ttu-id="dd59f-131">说明</span><span class="sxs-lookup"><span data-stu-id="dd59f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd59f-132">id</span><span class="sxs-lookup"><span data-stu-id="dd59f-132">id</span></span>|<span data-ttu-id="dd59f-133">String</span><span class="sxs-lookup"><span data-stu-id="dd59f-133">String</span></span>|<span data-ttu-id="dd59f-134">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dd59f-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="dd59f-135">url</span><span class="sxs-lookup"><span data-stu-id="dd59f-135">url</span></span>|<span data-ttu-id="dd59f-136">String</span><span class="sxs-lookup"><span data-stu-id="dd59f-136">String</span></span>|<span data-ttu-id="dd59f-137">网站 URL</span><span class="sxs-lookup"><span data-stu-id="dd59f-137">Website url</span></span>|
|<span data-ttu-id="dd59f-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="dd59f-138">deviceCount</span></span>|<span data-ttu-id="dd59f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="dd59f-139">Int32</span></span>|<span data-ttu-id="dd59f-140">设备计数</span><span class="sxs-lookup"><span data-stu-id="dd59f-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="dd59f-141">响应</span><span class="sxs-lookup"><span data-stu-id="dd59f-141">Response</span></span>
<span data-ttu-id="dd59f-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd59f-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd59f-143">示例</span><span class="sxs-lookup"><span data-stu-id="dd59f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd59f-144">请求</span><span class="sxs-lookup"><span data-stu-id="dd59f-144">Request</span></span>
<span data-ttu-id="dd59f-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd59f-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="dd59f-146">响应</span><span class="sxs-lookup"><span data-stu-id="dd59f-146">Response</span></span>
<span data-ttu-id="dd59f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd59f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




