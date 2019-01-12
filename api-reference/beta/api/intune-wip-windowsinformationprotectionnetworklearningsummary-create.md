---
title: 创建 windowsInformationProtectionNetworkLearningSummary
description: 创建新的 windowsInformationProtectionNetworkLearningSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 59b55111a022c1172abb9ab9f65ccf23e153c8cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915527"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="c51e6-103">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="c51e6-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="c51e6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c51e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c51e6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c51e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c51e6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c51e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c51e6-107">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c51e6-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c51e6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c51e6-108">Prerequisites</span></span>
<span data-ttu-id="c51e6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c51e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51e6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c51e6-111">Permission type</span></span>|<span data-ttu-id="c51e6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c51e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c51e6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c51e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c51e6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c51e6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c51e6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c51e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c51e6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c51e6-116">Not supported.</span></span>|
|<span data-ttu-id="c51e6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c51e6-117">Application</span></span>|<span data-ttu-id="c51e6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c51e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c51e6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c51e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="c51e6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c51e6-120">Request headers</span></span>
|<span data-ttu-id="c51e6-121">标头</span><span class="sxs-lookup"><span data-stu-id="c51e6-121">Header</span></span>|<span data-ttu-id="c51e6-122">值</span><span class="sxs-lookup"><span data-stu-id="c51e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c51e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c51e6-123">Authorization</span></span>|<span data-ttu-id="c51e6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c51e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c51e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c51e6-125">Accept</span></span>|<span data-ttu-id="c51e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c51e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c51e6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c51e6-127">Request body</span></span>
<span data-ttu-id="c51e6-128">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c51e6-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="c51e6-129">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c51e6-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="c51e6-130">属性</span><span class="sxs-lookup"><span data-stu-id="c51e6-130">Property</span></span>|<span data-ttu-id="c51e6-131">类型</span><span class="sxs-lookup"><span data-stu-id="c51e6-131">Type</span></span>|<span data-ttu-id="c51e6-132">说明</span><span class="sxs-lookup"><span data-stu-id="c51e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c51e6-133">id</span><span class="sxs-lookup"><span data-stu-id="c51e6-133">id</span></span>|<span data-ttu-id="c51e6-134">String</span><span class="sxs-lookup"><span data-stu-id="c51e6-134">String</span></span>|<span data-ttu-id="c51e6-135">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c51e6-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="c51e6-136">url</span><span class="sxs-lookup"><span data-stu-id="c51e6-136">url</span></span>|<span data-ttu-id="c51e6-137">String</span><span class="sxs-lookup"><span data-stu-id="c51e6-137">String</span></span>|<span data-ttu-id="c51e6-138">网站 URL</span><span class="sxs-lookup"><span data-stu-id="c51e6-138">Website url</span></span>|
|<span data-ttu-id="c51e6-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c51e6-139">deviceCount</span></span>|<span data-ttu-id="c51e6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c51e6-140">Int32</span></span>|<span data-ttu-id="c51e6-141">设备计数</span><span class="sxs-lookup"><span data-stu-id="c51e6-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="c51e6-142">响应</span><span class="sxs-lookup"><span data-stu-id="c51e6-142">Response</span></span>
<span data-ttu-id="c51e6-143">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c51e6-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c51e6-144">示例</span><span class="sxs-lookup"><span data-stu-id="c51e6-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="c51e6-145">请求</span><span class="sxs-lookup"><span data-stu-id="c51e6-145">Request</span></span>
<span data-ttu-id="c51e6-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c51e6-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c51e6-147">响应</span><span class="sxs-lookup"><span data-stu-id="c51e6-147">Response</span></span>
<span data-ttu-id="c51e6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c51e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





