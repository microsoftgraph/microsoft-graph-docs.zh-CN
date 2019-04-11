---
title: 更新 windowsInformationProtectionNetworkLearningSummary
description: 更新 windowsInformationProtectionNetworkLearningSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e22260808237797c14d8cf77f14ed07ff0add8e2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802406"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="469f6-103">更新 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="469f6-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="469f6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="469f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="469f6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="469f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="469f6-106">更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="469f6-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="469f6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="469f6-107">Prerequisites</span></span>
<span data-ttu-id="469f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="469f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="469f6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="469f6-110">Permission type</span></span>|<span data-ttu-id="469f6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="469f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="469f6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="469f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="469f6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469f6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="469f6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="469f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="469f6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="469f6-115">Not supported.</span></span>|
|<span data-ttu-id="469f6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="469f6-116">Application</span></span>|<span data-ttu-id="469f6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="469f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="469f6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="469f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="469f6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="469f6-119">Request headers</span></span>
|<span data-ttu-id="469f6-120">标头</span><span class="sxs-lookup"><span data-stu-id="469f6-120">Header</span></span>|<span data-ttu-id="469f6-121">值</span><span class="sxs-lookup"><span data-stu-id="469f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="469f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="469f6-122">Authorization</span></span>|<span data-ttu-id="469f6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="469f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="469f6-124">接受</span><span class="sxs-lookup"><span data-stu-id="469f6-124">Accept</span></span>|<span data-ttu-id="469f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="469f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="469f6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="469f6-126">Request body</span></span>
<span data-ttu-id="469f6-127">在请求正文中，提供 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="469f6-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="469f6-128">下表显示创建 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="469f6-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="469f6-129">属性</span><span class="sxs-lookup"><span data-stu-id="469f6-129">Property</span></span>|<span data-ttu-id="469f6-130">类型</span><span class="sxs-lookup"><span data-stu-id="469f6-130">Type</span></span>|<span data-ttu-id="469f6-131">说明</span><span class="sxs-lookup"><span data-stu-id="469f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="469f6-132">id</span><span class="sxs-lookup"><span data-stu-id="469f6-132">id</span></span>|<span data-ttu-id="469f6-133">String</span><span class="sxs-lookup"><span data-stu-id="469f6-133">String</span></span>|<span data-ttu-id="469f6-134">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="469f6-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="469f6-135">url</span><span class="sxs-lookup"><span data-stu-id="469f6-135">url</span></span>|<span data-ttu-id="469f6-136">String</span><span class="sxs-lookup"><span data-stu-id="469f6-136">String</span></span>|<span data-ttu-id="469f6-137">网站 URL</span><span class="sxs-lookup"><span data-stu-id="469f6-137">Website url</span></span>|
|<span data-ttu-id="469f6-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="469f6-138">deviceCount</span></span>|<span data-ttu-id="469f6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="469f6-139">Int32</span></span>|<span data-ttu-id="469f6-140">设备计数</span><span class="sxs-lookup"><span data-stu-id="469f6-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="469f6-141">响应</span><span class="sxs-lookup"><span data-stu-id="469f6-141">Response</span></span>
<span data-ttu-id="469f6-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="469f6-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="469f6-143">示例</span><span class="sxs-lookup"><span data-stu-id="469f6-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="469f6-144">请求</span><span class="sxs-lookup"><span data-stu-id="469f6-144">Request</span></span>
<span data-ttu-id="469f6-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="469f6-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="469f6-146">响应</span><span class="sxs-lookup"><span data-stu-id="469f6-146">Response</span></span>
<span data-ttu-id="469f6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="469f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





