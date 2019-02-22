---
title: 创建 windowsInformationProtectionAppLearningSummary
description: 创建新的 windowsInformationProtectionAppLearningSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 165664c3977ede205c406da712d5a331ff9de7c7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174655"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="cc633-103">创建 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="cc633-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="cc633-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc633-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc633-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc633-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc633-106">创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc633-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc633-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cc633-107">Prerequisites</span></span>
<span data-ttu-id="cc633-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cc633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc633-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc633-110">Permission type</span></span>|<span data-ttu-id="cc633-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cc633-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc633-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc633-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc633-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc633-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cc633-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc633-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc633-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc633-115">Not supported.</span></span>|
|<span data-ttu-id="cc633-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc633-116">Application</span></span>|<span data-ttu-id="cc633-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc633-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc633-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc633-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="cc633-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc633-119">Request headers</span></span>
|<span data-ttu-id="cc633-120">标头</span><span class="sxs-lookup"><span data-stu-id="cc633-120">Header</span></span>|<span data-ttu-id="cc633-121">值</span><span class="sxs-lookup"><span data-stu-id="cc633-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc633-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc633-122">Authorization</span></span>|<span data-ttu-id="cc633-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cc633-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc633-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cc633-124">Accept</span></span>|<span data-ttu-id="cc633-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc633-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc633-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc633-126">Request body</span></span>
<span data-ttu-id="cc633-127">在请求正文中，提供 windowsInformationProtectionAppLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc633-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="cc633-128">下表显示创建 windowsInformationProtectionAppLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cc633-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="cc633-129">属性</span><span class="sxs-lookup"><span data-stu-id="cc633-129">Property</span></span>|<span data-ttu-id="cc633-130">类型</span><span class="sxs-lookup"><span data-stu-id="cc633-130">Type</span></span>|<span data-ttu-id="cc633-131">说明</span><span class="sxs-lookup"><span data-stu-id="cc633-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc633-132">id</span><span class="sxs-lookup"><span data-stu-id="cc633-132">id</span></span>|<span data-ttu-id="cc633-133">字符串</span><span class="sxs-lookup"><span data-stu-id="cc633-133">String</span></span>|<span data-ttu-id="cc633-134">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cc633-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="cc633-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="cc633-135">applicationName</span></span>|<span data-ttu-id="cc633-136">String</span><span class="sxs-lookup"><span data-stu-id="cc633-136">String</span></span>|<span data-ttu-id="cc633-137">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="cc633-137">Application Name</span></span>|
|<span data-ttu-id="cc633-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="cc633-138">applicationType</span></span>|[<span data-ttu-id="cc633-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="cc633-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="cc633-140">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="cc633-140">Application Type.</span></span> <span data-ttu-id="cc633-141">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="cc633-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="cc633-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="cc633-142">deviceCount</span></span>|<span data-ttu-id="cc633-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cc633-143">Int32</span></span>|<span data-ttu-id="cc633-144">设备计数</span><span class="sxs-lookup"><span data-stu-id="cc633-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="cc633-145">响应</span><span class="sxs-lookup"><span data-stu-id="cc633-145">Response</span></span>
<span data-ttu-id="cc633-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc633-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc633-147">示例</span><span class="sxs-lookup"><span data-stu-id="cc633-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc633-148">请求</span><span class="sxs-lookup"><span data-stu-id="cc633-148">Request</span></span>
<span data-ttu-id="cc633-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc633-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="cc633-150">响应</span><span class="sxs-lookup"><span data-stu-id="cc633-150">Response</span></span>
<span data-ttu-id="cc633-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc633-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




