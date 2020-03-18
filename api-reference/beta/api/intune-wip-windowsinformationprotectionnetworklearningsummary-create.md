---
title: 创建 windowsInformationProtectionNetworkLearningSummary
description: 创建新的 windowsInformationProtectionNetworkLearningSummary 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f4ead9b9c1948ebf78b60718e57e12f7fe8fa4c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799616"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="72e13-103">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="72e13-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="72e13-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="72e13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72e13-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72e13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72e13-106">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72e13-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72e13-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="72e13-107">Prerequisites</span></span>
<span data-ttu-id="72e13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72e13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72e13-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72e13-110">Permission type</span></span>|<span data-ttu-id="72e13-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="72e13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72e13-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72e13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72e13-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72e13-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72e13-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72e13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72e13-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72e13-115">Not supported.</span></span>|
|<span data-ttu-id="72e13-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72e13-116">Application</span></span>|<span data-ttu-id="72e13-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72e13-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72e13-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72e13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="72e13-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="72e13-119">Request headers</span></span>
|<span data-ttu-id="72e13-120">标头</span><span class="sxs-lookup"><span data-stu-id="72e13-120">Header</span></span>|<span data-ttu-id="72e13-121">值</span><span class="sxs-lookup"><span data-stu-id="72e13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72e13-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72e13-122">Authorization</span></span>|<span data-ttu-id="72e13-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="72e13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72e13-124">接受</span><span class="sxs-lookup"><span data-stu-id="72e13-124">Accept</span></span>|<span data-ttu-id="72e13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72e13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72e13-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="72e13-126">Request body</span></span>
<span data-ttu-id="72e13-127">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72e13-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="72e13-128">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="72e13-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="72e13-129">属性</span><span class="sxs-lookup"><span data-stu-id="72e13-129">Property</span></span>|<span data-ttu-id="72e13-130">类型</span><span class="sxs-lookup"><span data-stu-id="72e13-130">Type</span></span>|<span data-ttu-id="72e13-131">说明</span><span class="sxs-lookup"><span data-stu-id="72e13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72e13-132">id</span><span class="sxs-lookup"><span data-stu-id="72e13-132">id</span></span>|<span data-ttu-id="72e13-133">String</span><span class="sxs-lookup"><span data-stu-id="72e13-133">String</span></span>|<span data-ttu-id="72e13-134">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="72e13-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="72e13-135">url</span><span class="sxs-lookup"><span data-stu-id="72e13-135">url</span></span>|<span data-ttu-id="72e13-136">String</span><span class="sxs-lookup"><span data-stu-id="72e13-136">String</span></span>|<span data-ttu-id="72e13-137">网站 URL</span><span class="sxs-lookup"><span data-stu-id="72e13-137">Website url</span></span>|
|<span data-ttu-id="72e13-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="72e13-138">deviceCount</span></span>|<span data-ttu-id="72e13-139">Int32</span><span class="sxs-lookup"><span data-stu-id="72e13-139">Int32</span></span>|<span data-ttu-id="72e13-140">设备计数</span><span class="sxs-lookup"><span data-stu-id="72e13-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="72e13-141">响应</span><span class="sxs-lookup"><span data-stu-id="72e13-141">Response</span></span>
<span data-ttu-id="72e13-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72e13-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72e13-143">示例</span><span class="sxs-lookup"><span data-stu-id="72e13-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="72e13-144">请求</span><span class="sxs-lookup"><span data-stu-id="72e13-144">Request</span></span>
<span data-ttu-id="72e13-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72e13-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="72e13-146">响应</span><span class="sxs-lookup"><span data-stu-id="72e13-146">Response</span></span>
<span data-ttu-id="72e13-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72e13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




