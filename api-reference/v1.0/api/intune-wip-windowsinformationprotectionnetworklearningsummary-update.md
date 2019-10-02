---
title: 更新 windowsInformationProtectionNetworkLearningSummary
description: 更新 windowsInformationProtectionNetworkLearningSummary 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cdbdb0532cc4c9e1992d8abcb993f0eaa9ae08e5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360886"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="76691-103">更新 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="76691-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="76691-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76691-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76691-105">更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="76691-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76691-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="76691-106">Prerequisites</span></span>
<span data-ttu-id="76691-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76691-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="76691-109">Permission type</span></span>|<span data-ttu-id="76691-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76691-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76691-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76691-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76691-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76691-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76691-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76691-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76691-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="76691-114">Not supported.</span></span>|
|<span data-ttu-id="76691-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="76691-115">Application</span></span>|<span data-ttu-id="76691-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76691-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76691-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76691-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="76691-118">请求头</span><span class="sxs-lookup"><span data-stu-id="76691-118">Request headers</span></span>
|<span data-ttu-id="76691-119">标头</span><span class="sxs-lookup"><span data-stu-id="76691-119">Header</span></span>|<span data-ttu-id="76691-120">值</span><span class="sxs-lookup"><span data-stu-id="76691-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76691-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="76691-121">Authorization</span></span>|<span data-ttu-id="76691-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76691-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76691-123">接受</span><span class="sxs-lookup"><span data-stu-id="76691-123">Accept</span></span>|<span data-ttu-id="76691-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76691-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76691-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="76691-125">Request body</span></span>
<span data-ttu-id="76691-126">在请求正文中，提供 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76691-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="76691-127">下表显示创建 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="76691-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="76691-128">属性</span><span class="sxs-lookup"><span data-stu-id="76691-128">Property</span></span>|<span data-ttu-id="76691-129">类型</span><span class="sxs-lookup"><span data-stu-id="76691-129">Type</span></span>|<span data-ttu-id="76691-130">说明</span><span class="sxs-lookup"><span data-stu-id="76691-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76691-131">id</span><span class="sxs-lookup"><span data-stu-id="76691-131">id</span></span>|<span data-ttu-id="76691-132">String</span><span class="sxs-lookup"><span data-stu-id="76691-132">String</span></span>|<span data-ttu-id="76691-133">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="76691-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="76691-134">url</span><span class="sxs-lookup"><span data-stu-id="76691-134">url</span></span>|<span data-ttu-id="76691-135">String</span><span class="sxs-lookup"><span data-stu-id="76691-135">String</span></span>|<span data-ttu-id="76691-136">网站 URL</span><span class="sxs-lookup"><span data-stu-id="76691-136">Website url</span></span>|
|<span data-ttu-id="76691-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="76691-137">deviceCount</span></span>|<span data-ttu-id="76691-138">Int32</span><span class="sxs-lookup"><span data-stu-id="76691-138">Int32</span></span>|<span data-ttu-id="76691-139">设备计数</span><span class="sxs-lookup"><span data-stu-id="76691-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="76691-140">响应</span><span class="sxs-lookup"><span data-stu-id="76691-140">Response</span></span>
<span data-ttu-id="76691-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76691-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76691-142">示例</span><span class="sxs-lookup"><span data-stu-id="76691-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="76691-143">请求</span><span class="sxs-lookup"><span data-stu-id="76691-143">Request</span></span>
<span data-ttu-id="76691-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76691-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76691-145">响应</span><span class="sxs-lookup"><span data-stu-id="76691-145">Response</span></span>
<span data-ttu-id="76691-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76691-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




