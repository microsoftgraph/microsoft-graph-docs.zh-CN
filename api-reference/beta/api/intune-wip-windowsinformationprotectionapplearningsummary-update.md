---
title: 更新 windowsInformationProtectionAppLearningSummary
description: 更新 windowsInformationProtectionAppLearningSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 885c5bd417f17ff81199e0fcf4afc122860a3731
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890018"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="0ab56-103">更新 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="0ab56-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="0ab56-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ab56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ab56-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ab56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ab56-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0ab56-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ab56-107">更新 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ab56-107">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ab56-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ab56-108">Prerequisites</span></span>
<span data-ttu-id="0ab56-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0ab56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ab56-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ab56-111">Permission type</span></span>|<span data-ttu-id="0ab56-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ab56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ab56-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ab56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ab56-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ab56-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0ab56-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ab56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ab56-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ab56-116">Not supported.</span></span>|
|<span data-ttu-id="0ab56-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ab56-117">Application</span></span>|<span data-ttu-id="0ab56-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ab56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ab56-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ab56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="0ab56-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ab56-120">Request headers</span></span>
|<span data-ttu-id="0ab56-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ab56-121">Header</span></span>|<span data-ttu-id="0ab56-122">值</span><span class="sxs-lookup"><span data-stu-id="0ab56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ab56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ab56-123">Authorization</span></span>|<span data-ttu-id="0ab56-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ab56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ab56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ab56-125">Accept</span></span>|<span data-ttu-id="0ab56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ab56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ab56-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ab56-127">Request body</span></span>
<span data-ttu-id="0ab56-128">在请求正文中，提供 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ab56-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="0ab56-129">下表显示创建 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ab56-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="0ab56-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ab56-130">Property</span></span>|<span data-ttu-id="0ab56-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ab56-131">Type</span></span>|<span data-ttu-id="0ab56-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ab56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ab56-133">id</span><span class="sxs-lookup"><span data-stu-id="0ab56-133">id</span></span>|<span data-ttu-id="0ab56-134">String</span><span class="sxs-lookup"><span data-stu-id="0ab56-134">String</span></span>|<span data-ttu-id="0ab56-135">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0ab56-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="0ab56-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="0ab56-136">applicationName</span></span>|<span data-ttu-id="0ab56-137">String</span><span class="sxs-lookup"><span data-stu-id="0ab56-137">String</span></span>|<span data-ttu-id="0ab56-138">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="0ab56-138">Application Name</span></span>|
|<span data-ttu-id="0ab56-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="0ab56-139">applicationType</span></span>|[<span data-ttu-id="0ab56-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="0ab56-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="0ab56-141">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="0ab56-141">Application Type.</span></span> <span data-ttu-id="0ab56-142">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="0ab56-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="0ab56-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="0ab56-143">deviceCount</span></span>|<span data-ttu-id="0ab56-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0ab56-144">Int32</span></span>|<span data-ttu-id="0ab56-145">设备计数</span><span class="sxs-lookup"><span data-stu-id="0ab56-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="0ab56-146">响应</span><span class="sxs-lookup"><span data-stu-id="0ab56-146">Response</span></span>
<span data-ttu-id="0ab56-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ab56-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ab56-148">示例</span><span class="sxs-lookup"><span data-stu-id="0ab56-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ab56-149">请求</span><span class="sxs-lookup"><span data-stu-id="0ab56-149">Request</span></span>
<span data-ttu-id="0ab56-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ab56-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 106

{
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="0ab56-151">响应</span><span class="sxs-lookup"><span data-stu-id="0ab56-151">Response</span></span>
<span data-ttu-id="0ab56-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ab56-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```





