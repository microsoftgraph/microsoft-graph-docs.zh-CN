---
title: 更新 windowsInformationProtectionNetworkLearningSummary
description: 更新 windowsInformationProtectionNetworkLearningSummary 对象的属性。
author: tfitzmac
ms.openlocfilehash: 30f5585149a1130a92c203394950c581655cc78b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329419"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="933d2-103">更新 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="933d2-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="933d2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="933d2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="933d2-105">更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="933d2-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="933d2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="933d2-106">Prerequisites</span></span>
<span data-ttu-id="933d2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="933d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="933d2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="933d2-109">Permission type</span></span>|<span data-ttu-id="933d2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="933d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="933d2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="933d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="933d2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="933d2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="933d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="933d2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="933d2-114">Not supported.</span></span>|
|<span data-ttu-id="933d2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="933d2-115">Application</span></span>|<span data-ttu-id="933d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="933d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="933d2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="933d2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="933d2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="933d2-118">Request headers</span></span>
|<span data-ttu-id="933d2-119">标头</span><span class="sxs-lookup"><span data-stu-id="933d2-119">Header</span></span>|<span data-ttu-id="933d2-120">值</span><span class="sxs-lookup"><span data-stu-id="933d2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="933d2-121">授权</span><span class="sxs-lookup"><span data-stu-id="933d2-121">Authorization</span></span>|<span data-ttu-id="933d2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="933d2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="933d2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="933d2-123">Accept</span></span>|<span data-ttu-id="933d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="933d2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="933d2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="933d2-125">Request body</span></span>
<span data-ttu-id="933d2-126">在请求正文中，提供 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="933d2-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="933d2-127">下表显示创建 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="933d2-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="933d2-128">属性</span><span class="sxs-lookup"><span data-stu-id="933d2-128">Property</span></span>|<span data-ttu-id="933d2-129">类型</span><span class="sxs-lookup"><span data-stu-id="933d2-129">Type</span></span>|<span data-ttu-id="933d2-130">说明</span><span class="sxs-lookup"><span data-stu-id="933d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="933d2-131">id</span><span class="sxs-lookup"><span data-stu-id="933d2-131">id</span></span>|<span data-ttu-id="933d2-132">String</span><span class="sxs-lookup"><span data-stu-id="933d2-132">String</span></span>|<span data-ttu-id="933d2-133">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="933d2-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="933d2-134">url</span><span class="sxs-lookup"><span data-stu-id="933d2-134">url</span></span>|<span data-ttu-id="933d2-135">String</span><span class="sxs-lookup"><span data-stu-id="933d2-135">String</span></span>|<span data-ttu-id="933d2-136">网站 URL</span><span class="sxs-lookup"><span data-stu-id="933d2-136">Website url</span></span>|
|<span data-ttu-id="933d2-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="933d2-137">deviceCount</span></span>|<span data-ttu-id="933d2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="933d2-138">Int32</span></span>|<span data-ttu-id="933d2-139">设备计数</span><span class="sxs-lookup"><span data-stu-id="933d2-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="933d2-140">响应</span><span class="sxs-lookup"><span data-stu-id="933d2-140">Response</span></span>
<span data-ttu-id="933d2-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="933d2-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="933d2-142">示例</span><span class="sxs-lookup"><span data-stu-id="933d2-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="933d2-143">请求</span><span class="sxs-lookup"><span data-stu-id="933d2-143">Request</span></span>
<span data-ttu-id="933d2-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="933d2-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="933d2-145">响应</span><span class="sxs-lookup"><span data-stu-id="933d2-145">Response</span></span>
<span data-ttu-id="933d2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="933d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



