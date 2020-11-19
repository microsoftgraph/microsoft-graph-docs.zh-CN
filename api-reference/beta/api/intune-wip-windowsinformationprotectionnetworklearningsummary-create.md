---
title: 创建 windowsInformationProtectionNetworkLearningSummary
description: 创建新的 windowsInformationProtectionNetworkLearningSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55b9561f36006b27aa3fb918a76bfb6735b5e470
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261410"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="c7a2a-103">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="c7a2a-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="c7a2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7a2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7a2a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7a2a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7a2a-107">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7a2a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7a2a-108">Prerequisites</span></span>
<span data-ttu-id="c7a2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7a2a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7a2a-111">Permission type</span></span>|<span data-ttu-id="c7a2a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7a2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7a2a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7a2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7a2a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a2a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7a2a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7a2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7a2a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-116">Not supported.</span></span>|
|<span data-ttu-id="c7a2a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7a2a-117">Application</span></span>|<span data-ttu-id="c7a2a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a2a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7a2a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7a2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="c7a2a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7a2a-120">Request headers</span></span>
|<span data-ttu-id="c7a2a-121">标头</span><span class="sxs-lookup"><span data-stu-id="c7a2a-121">Header</span></span>|<span data-ttu-id="c7a2a-122">值</span><span class="sxs-lookup"><span data-stu-id="c7a2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7a2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7a2a-123">Authorization</span></span>|<span data-ttu-id="c7a2a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7a2a-125">接受</span><span class="sxs-lookup"><span data-stu-id="c7a2a-125">Accept</span></span>|<span data-ttu-id="c7a2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7a2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7a2a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7a2a-127">Request body</span></span>
<span data-ttu-id="c7a2a-128">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="c7a2a-129">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="c7a2a-130">属性</span><span class="sxs-lookup"><span data-stu-id="c7a2a-130">Property</span></span>|<span data-ttu-id="c7a2a-131">类型</span><span class="sxs-lookup"><span data-stu-id="c7a2a-131">Type</span></span>|<span data-ttu-id="c7a2a-132">说明</span><span class="sxs-lookup"><span data-stu-id="c7a2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7a2a-133">id</span><span class="sxs-lookup"><span data-stu-id="c7a2a-133">id</span></span>|<span data-ttu-id="c7a2a-134">String</span><span class="sxs-lookup"><span data-stu-id="c7a2a-134">String</span></span>|<span data-ttu-id="c7a2a-135">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="c7a2a-136">url</span><span class="sxs-lookup"><span data-stu-id="c7a2a-136">url</span></span>|<span data-ttu-id="c7a2a-137">String</span><span class="sxs-lookup"><span data-stu-id="c7a2a-137">String</span></span>|<span data-ttu-id="c7a2a-138">网站 URL</span><span class="sxs-lookup"><span data-stu-id="c7a2a-138">Website url</span></span>|
|<span data-ttu-id="c7a2a-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c7a2a-139">deviceCount</span></span>|<span data-ttu-id="c7a2a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c7a2a-140">Int32</span></span>|<span data-ttu-id="c7a2a-141">设备计数</span><span class="sxs-lookup"><span data-stu-id="c7a2a-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="c7a2a-142">响应</span><span class="sxs-lookup"><span data-stu-id="c7a2a-142">Response</span></span>
<span data-ttu-id="c7a2a-143">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7a2a-144">示例</span><span class="sxs-lookup"><span data-stu-id="c7a2a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7a2a-145">请求</span><span class="sxs-lookup"><span data-stu-id="c7a2a-145">Request</span></span>
<span data-ttu-id="c7a2a-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7a2a-147">响应</span><span class="sxs-lookup"><span data-stu-id="c7a2a-147">Response</span></span>
<span data-ttu-id="c7a2a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7a2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




