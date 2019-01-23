---
title: 创建 windowsInformationProtectionNetworkLearningSummary
description: 创建新的 windowsInformationProtectionNetworkLearningSummary 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ef10a71e9e6b59c86e1450cea8e40465bc0f70af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403250"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="36d5c-103">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="36d5c-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="36d5c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="36d5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36d5c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36d5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36d5c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36d5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36d5c-107">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36d5c-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36d5c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="36d5c-108">Prerequisites</span></span>
<span data-ttu-id="36d5c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="36d5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36d5c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36d5c-111">Permission type</span></span>|<span data-ttu-id="36d5c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36d5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36d5c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36d5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36d5c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36d5c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36d5c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36d5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36d5c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36d5c-116">Not supported.</span></span>|
|<span data-ttu-id="36d5c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36d5c-117">Application</span></span>|<span data-ttu-id="36d5c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="36d5c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36d5c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36d5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="36d5c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36d5c-120">Request headers</span></span>
|<span data-ttu-id="36d5c-121">标头</span><span class="sxs-lookup"><span data-stu-id="36d5c-121">Header</span></span>|<span data-ttu-id="36d5c-122">值</span><span class="sxs-lookup"><span data-stu-id="36d5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36d5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36d5c-123">Authorization</span></span>|<span data-ttu-id="36d5c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36d5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36d5c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36d5c-125">Accept</span></span>|<span data-ttu-id="36d5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36d5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36d5c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36d5c-127">Request body</span></span>
<span data-ttu-id="36d5c-128">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36d5c-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="36d5c-129">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36d5c-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="36d5c-130">属性</span><span class="sxs-lookup"><span data-stu-id="36d5c-130">Property</span></span>|<span data-ttu-id="36d5c-131">类型</span><span class="sxs-lookup"><span data-stu-id="36d5c-131">Type</span></span>|<span data-ttu-id="36d5c-132">说明</span><span class="sxs-lookup"><span data-stu-id="36d5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36d5c-133">id</span><span class="sxs-lookup"><span data-stu-id="36d5c-133">id</span></span>|<span data-ttu-id="36d5c-134">String</span><span class="sxs-lookup"><span data-stu-id="36d5c-134">String</span></span>|<span data-ttu-id="36d5c-135">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="36d5c-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="36d5c-136">url</span><span class="sxs-lookup"><span data-stu-id="36d5c-136">url</span></span>|<span data-ttu-id="36d5c-137">String</span><span class="sxs-lookup"><span data-stu-id="36d5c-137">String</span></span>|<span data-ttu-id="36d5c-138">网站 URL</span><span class="sxs-lookup"><span data-stu-id="36d5c-138">Website url</span></span>|
|<span data-ttu-id="36d5c-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="36d5c-139">deviceCount</span></span>|<span data-ttu-id="36d5c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="36d5c-140">Int32</span></span>|<span data-ttu-id="36d5c-141">设备计数</span><span class="sxs-lookup"><span data-stu-id="36d5c-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="36d5c-142">响应</span><span class="sxs-lookup"><span data-stu-id="36d5c-142">Response</span></span>
<span data-ttu-id="36d5c-143">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36d5c-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36d5c-144">示例</span><span class="sxs-lookup"><span data-stu-id="36d5c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="36d5c-145">请求</span><span class="sxs-lookup"><span data-stu-id="36d5c-145">Request</span></span>
<span data-ttu-id="36d5c-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36d5c-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36d5c-147">响应</span><span class="sxs-lookup"><span data-stu-id="36d5c-147">Response</span></span>
<span data-ttu-id="36d5c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36d5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




