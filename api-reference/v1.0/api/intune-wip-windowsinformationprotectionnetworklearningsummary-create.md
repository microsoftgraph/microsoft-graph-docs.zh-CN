---
title: 创建 windowsInformationProtectionNetworkLearningSummary
description: 创建新的 windowsInformationProtectionNetworkLearningSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 57cfde950bc4152c605e41e0caff8d18d919eb46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876459"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="d63e5-103">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="d63e5-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="d63e5-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d63e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d63e5-105">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d63e5-105">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d63e5-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d63e5-106">Prerequisites</span></span>
<span data-ttu-id="d63e5-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d63e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d63e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d63e5-109">Permission type</span></span>|<span data-ttu-id="d63e5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d63e5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d63e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d63e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d63e5-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d63e5-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d63e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d63e5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d63e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d63e5-114">Not supported.</span></span>|
|<span data-ttu-id="d63e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d63e5-115">Application</span></span>|<span data-ttu-id="d63e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d63e5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d63e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d63e5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d63e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d63e5-118">Request headers</span></span>
|<span data-ttu-id="d63e5-119">标头</span><span class="sxs-lookup"><span data-stu-id="d63e5-119">Header</span></span>|<span data-ttu-id="d63e5-120">值</span><span class="sxs-lookup"><span data-stu-id="d63e5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d63e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d63e5-121">Authorization</span></span>|<span data-ttu-id="d63e5-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d63e5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d63e5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d63e5-123">Accept</span></span>|<span data-ttu-id="d63e5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d63e5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d63e5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d63e5-125">Request body</span></span>
<span data-ttu-id="d63e5-126">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d63e5-126">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="d63e5-127">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d63e5-127">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="d63e5-128">属性</span><span class="sxs-lookup"><span data-stu-id="d63e5-128">Property</span></span>|<span data-ttu-id="d63e5-129">类型</span><span class="sxs-lookup"><span data-stu-id="d63e5-129">Type</span></span>|<span data-ttu-id="d63e5-130">说明</span><span class="sxs-lookup"><span data-stu-id="d63e5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d63e5-131">id</span><span class="sxs-lookup"><span data-stu-id="d63e5-131">id</span></span>|<span data-ttu-id="d63e5-132">String</span><span class="sxs-lookup"><span data-stu-id="d63e5-132">String</span></span>|<span data-ttu-id="d63e5-133">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d63e5-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="d63e5-134">url</span><span class="sxs-lookup"><span data-stu-id="d63e5-134">url</span></span>|<span data-ttu-id="d63e5-135">String</span><span class="sxs-lookup"><span data-stu-id="d63e5-135">String</span></span>|<span data-ttu-id="d63e5-136">网站 URL</span><span class="sxs-lookup"><span data-stu-id="d63e5-136">Website url</span></span>|
|<span data-ttu-id="d63e5-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d63e5-137">deviceCount</span></span>|<span data-ttu-id="d63e5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d63e5-138">Int32</span></span>|<span data-ttu-id="d63e5-139">设备计数</span><span class="sxs-lookup"><span data-stu-id="d63e5-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="d63e5-140">响应</span><span class="sxs-lookup"><span data-stu-id="d63e5-140">Response</span></span>
<span data-ttu-id="d63e5-141">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d63e5-141">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d63e5-142">示例</span><span class="sxs-lookup"><span data-stu-id="d63e5-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="d63e5-143">请求</span><span class="sxs-lookup"><span data-stu-id="d63e5-143">Request</span></span>
<span data-ttu-id="d63e5-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d63e5-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d63e5-145">响应</span><span class="sxs-lookup"><span data-stu-id="d63e5-145">Response</span></span>
<span data-ttu-id="d63e5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d63e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



