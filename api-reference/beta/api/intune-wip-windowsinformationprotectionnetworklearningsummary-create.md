---
title: 创建 windowsInformationProtectionNetworkLearningSummary
description: 创建新的 windowsInformationProtectionNetworkLearningSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bffb54852f72881b3ea4b48ca69e3bf0f6e9179
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150937"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="31963-103">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="31963-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="31963-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="31963-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31963-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31963-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31963-106">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31963-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31963-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="31963-107">Prerequisites</span></span>
<span data-ttu-id="31963-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="31963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="31963-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="31963-110">Permission type</span></span>|<span data-ttu-id="31963-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31963-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31963-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31963-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31963-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31963-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31963-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31963-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31963-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31963-115">Not supported.</span></span>|
|<span data-ttu-id="31963-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="31963-116">Application</span></span>|<span data-ttu-id="31963-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="31963-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31963-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31963-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="31963-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="31963-119">Request headers</span></span>
|<span data-ttu-id="31963-120">标头</span><span class="sxs-lookup"><span data-stu-id="31963-120">Header</span></span>|<span data-ttu-id="31963-121">值</span><span class="sxs-lookup"><span data-stu-id="31963-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31963-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31963-122">Authorization</span></span>|<span data-ttu-id="31963-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31963-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31963-124">Accept</span><span class="sxs-lookup"><span data-stu-id="31963-124">Accept</span></span>|<span data-ttu-id="31963-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31963-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31963-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="31963-126">Request body</span></span>
<span data-ttu-id="31963-127">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31963-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="31963-128">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="31963-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="31963-129">属性</span><span class="sxs-lookup"><span data-stu-id="31963-129">Property</span></span>|<span data-ttu-id="31963-130">类型</span><span class="sxs-lookup"><span data-stu-id="31963-130">Type</span></span>|<span data-ttu-id="31963-131">说明</span><span class="sxs-lookup"><span data-stu-id="31963-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31963-132">id</span><span class="sxs-lookup"><span data-stu-id="31963-132">id</span></span>|<span data-ttu-id="31963-133">字符串</span><span class="sxs-lookup"><span data-stu-id="31963-133">String</span></span>|<span data-ttu-id="31963-134">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31963-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="31963-135">url</span><span class="sxs-lookup"><span data-stu-id="31963-135">url</span></span>|<span data-ttu-id="31963-136">String</span><span class="sxs-lookup"><span data-stu-id="31963-136">String</span></span>|<span data-ttu-id="31963-137">网站 URL</span><span class="sxs-lookup"><span data-stu-id="31963-137">Website url</span></span>|
|<span data-ttu-id="31963-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="31963-138">deviceCount</span></span>|<span data-ttu-id="31963-139">Int32</span><span class="sxs-lookup"><span data-stu-id="31963-139">Int32</span></span>|<span data-ttu-id="31963-140">设备计数</span><span class="sxs-lookup"><span data-stu-id="31963-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="31963-141">响应</span><span class="sxs-lookup"><span data-stu-id="31963-141">Response</span></span>
<span data-ttu-id="31963-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31963-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31963-143">示例</span><span class="sxs-lookup"><span data-stu-id="31963-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="31963-144">请求</span><span class="sxs-lookup"><span data-stu-id="31963-144">Request</span></span>
<span data-ttu-id="31963-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31963-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31963-146">响应</span><span class="sxs-lookup"><span data-stu-id="31963-146">Response</span></span>
<span data-ttu-id="31963-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31963-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




