---
title: 创建 windowsInformationProtectionNetworkLearningSummary
description: 创建新的 windowsInformationProtectionNetworkLearningSummary 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1591e782fa816e9e3d43485e13e4f123a0fa641
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360935"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="96817-103">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="96817-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="96817-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96817-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96817-105">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96817-105">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96817-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="96817-106">Prerequisites</span></span>
<span data-ttu-id="96817-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96817-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96817-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96817-109">Permission type</span></span>|<span data-ttu-id="96817-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96817-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96817-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96817-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96817-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96817-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96817-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96817-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96817-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="96817-114">Not supported.</span></span>|
|<span data-ttu-id="96817-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="96817-115">Application</span></span>|<span data-ttu-id="96817-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96817-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96817-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96817-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="96817-118">请求头</span><span class="sxs-lookup"><span data-stu-id="96817-118">Request headers</span></span>
|<span data-ttu-id="96817-119">标头</span><span class="sxs-lookup"><span data-stu-id="96817-119">Header</span></span>|<span data-ttu-id="96817-120">值</span><span class="sxs-lookup"><span data-stu-id="96817-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96817-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96817-121">Authorization</span></span>|<span data-ttu-id="96817-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96817-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96817-123">接受</span><span class="sxs-lookup"><span data-stu-id="96817-123">Accept</span></span>|<span data-ttu-id="96817-124">application/json</span><span class="sxs-lookup"><span data-stu-id="96817-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96817-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="96817-125">Request body</span></span>
<span data-ttu-id="96817-126">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96817-126">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="96817-127">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="96817-127">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="96817-128">属性</span><span class="sxs-lookup"><span data-stu-id="96817-128">Property</span></span>|<span data-ttu-id="96817-129">类型</span><span class="sxs-lookup"><span data-stu-id="96817-129">Type</span></span>|<span data-ttu-id="96817-130">说明</span><span class="sxs-lookup"><span data-stu-id="96817-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96817-131">id</span><span class="sxs-lookup"><span data-stu-id="96817-131">id</span></span>|<span data-ttu-id="96817-132">String</span><span class="sxs-lookup"><span data-stu-id="96817-132">String</span></span>|<span data-ttu-id="96817-133">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96817-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="96817-134">url</span><span class="sxs-lookup"><span data-stu-id="96817-134">url</span></span>|<span data-ttu-id="96817-135">String</span><span class="sxs-lookup"><span data-stu-id="96817-135">String</span></span>|<span data-ttu-id="96817-136">网站 URL</span><span class="sxs-lookup"><span data-stu-id="96817-136">Website url</span></span>|
|<span data-ttu-id="96817-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="96817-137">deviceCount</span></span>|<span data-ttu-id="96817-138">Int32</span><span class="sxs-lookup"><span data-stu-id="96817-138">Int32</span></span>|<span data-ttu-id="96817-139">设备计数</span><span class="sxs-lookup"><span data-stu-id="96817-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="96817-140">响应</span><span class="sxs-lookup"><span data-stu-id="96817-140">Response</span></span>
<span data-ttu-id="96817-141">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96817-141">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96817-142">示例</span><span class="sxs-lookup"><span data-stu-id="96817-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="96817-143">请求</span><span class="sxs-lookup"><span data-stu-id="96817-143">Request</span></span>
<span data-ttu-id="96817-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96817-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="96817-145">响应</span><span class="sxs-lookup"><span data-stu-id="96817-145">Response</span></span>
<span data-ttu-id="96817-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96817-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```




