---
title: 更新 windowsInformationProtectionNetworkLearningSummary
description: 更新 windowsInformationProtectionNetworkLearningSummary 对象的属性。
author: tfitzmac
ms.openlocfilehash: 335fee7e664000584fa4542985a3b014d827f0d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344434"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="e5cfa-103">更新 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="e5cfa-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="e5cfa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5cfa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5cfa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5cfa-107">更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5cfa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5cfa-108">Prerequisites</span></span>
<span data-ttu-id="e5cfa-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e5cfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cfa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5cfa-111">Permission type</span></span>|<span data-ttu-id="e5cfa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e5cfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5cfa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5cfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5cfa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cfa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5cfa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5cfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5cfa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-116">Not supported.</span></span>|
|<span data-ttu-id="e5cfa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5cfa-117">Application</span></span>|<span data-ttu-id="e5cfa-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5cfa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5cfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e5cfa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5cfa-120">Request headers</span></span>
|<span data-ttu-id="e5cfa-121">标头</span><span class="sxs-lookup"><span data-stu-id="e5cfa-121">Header</span></span>|<span data-ttu-id="e5cfa-122">值</span><span class="sxs-lookup"><span data-stu-id="e5cfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5cfa-123">授权</span><span class="sxs-lookup"><span data-stu-id="e5cfa-123">Authorization</span></span>|<span data-ttu-id="e5cfa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5cfa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5cfa-125">Accept</span></span>|<span data-ttu-id="e5cfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5cfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5cfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5cfa-127">Request body</span></span>
<span data-ttu-id="e5cfa-128">在请求正文中，提供 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="e5cfa-129">下表显示创建 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="e5cfa-130">属性</span><span class="sxs-lookup"><span data-stu-id="e5cfa-130">Property</span></span>|<span data-ttu-id="e5cfa-131">类型</span><span class="sxs-lookup"><span data-stu-id="e5cfa-131">Type</span></span>|<span data-ttu-id="e5cfa-132">说明</span><span class="sxs-lookup"><span data-stu-id="e5cfa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5cfa-133">id</span><span class="sxs-lookup"><span data-stu-id="e5cfa-133">id</span></span>|<span data-ttu-id="e5cfa-134">String</span><span class="sxs-lookup"><span data-stu-id="e5cfa-134">String</span></span>|<span data-ttu-id="e5cfa-135">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="e5cfa-136">url</span><span class="sxs-lookup"><span data-stu-id="e5cfa-136">url</span></span>|<span data-ttu-id="e5cfa-137">String</span><span class="sxs-lookup"><span data-stu-id="e5cfa-137">String</span></span>|<span data-ttu-id="e5cfa-138">网站 URL</span><span class="sxs-lookup"><span data-stu-id="e5cfa-138">Website url</span></span>|
|<span data-ttu-id="e5cfa-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e5cfa-139">deviceCount</span></span>|<span data-ttu-id="e5cfa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cfa-140">Int32</span></span>|<span data-ttu-id="e5cfa-141">设备计数</span><span class="sxs-lookup"><span data-stu-id="e5cfa-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="e5cfa-142">响应</span><span class="sxs-lookup"><span data-stu-id="e5cfa-142">Response</span></span>
<span data-ttu-id="e5cfa-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5cfa-144">示例</span><span class="sxs-lookup"><span data-stu-id="e5cfa-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5cfa-145">请求</span><span class="sxs-lookup"><span data-stu-id="e5cfa-145">Request</span></span>
<span data-ttu-id="e5cfa-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="e5cfa-147">响应</span><span class="sxs-lookup"><span data-stu-id="e5cfa-147">Response</span></span>
<span data-ttu-id="e5cfa-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5cfa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





