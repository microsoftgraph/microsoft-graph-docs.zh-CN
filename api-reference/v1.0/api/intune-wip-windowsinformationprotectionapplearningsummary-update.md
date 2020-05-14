---
title: 更新 windowsInformationProtectionAppLearningSummary
description: 更新 windowsInformationProtectionAppLearningSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99cbb3d9f1ad497039103c2ebb405ae94643376e
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43461178"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="6cc5c-103">更新 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="6cc5c-103">Update windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="6cc5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cc5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cc5c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cc5c-106">更新 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cc5c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6cc5c-107">Prerequisites</span></span>
<span data-ttu-id="6cc5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc5c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cc5c-110">Permission type</span></span>|<span data-ttu-id="6cc5c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6cc5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc5c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cc5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc5c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cc5c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6cc5c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cc5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc5c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-115">Not supported.</span></span>|
|<span data-ttu-id="6cc5c-116">Application</span><span class="sxs-lookup"><span data-stu-id="6cc5c-116">Application</span></span>|<span data-ttu-id="6cc5c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc5c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cc5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="6cc5c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cc5c-119">Request headers</span></span>
|<span data-ttu-id="6cc5c-120">标头</span><span class="sxs-lookup"><span data-stu-id="6cc5c-120">Header</span></span>|<span data-ttu-id="6cc5c-121">值</span><span class="sxs-lookup"><span data-stu-id="6cc5c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc5c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc5c-122">Authorization</span></span>|<span data-ttu-id="6cc5c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc5c-124">接受</span><span class="sxs-lookup"><span data-stu-id="6cc5c-124">Accept</span></span>|<span data-ttu-id="6cc5c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc5c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc5c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cc5c-126">Request body</span></span>
<span data-ttu-id="6cc5c-127">在请求正文中，提供 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="6cc5c-128">下表显示创建 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="6cc5c-129">属性</span><span class="sxs-lookup"><span data-stu-id="6cc5c-129">Property</span></span>|<span data-ttu-id="6cc5c-130">类型</span><span class="sxs-lookup"><span data-stu-id="6cc5c-130">Type</span></span>|<span data-ttu-id="6cc5c-131">说明</span><span class="sxs-lookup"><span data-stu-id="6cc5c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc5c-132">id</span><span class="sxs-lookup"><span data-stu-id="6cc5c-132">id</span></span>|<span data-ttu-id="6cc5c-133">String</span><span class="sxs-lookup"><span data-stu-id="6cc5c-133">String</span></span>|<span data-ttu-id="6cc5c-134">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="6cc5c-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="6cc5c-135">applicationName</span></span>|<span data-ttu-id="6cc5c-136">String</span><span class="sxs-lookup"><span data-stu-id="6cc5c-136">String</span></span>|<span data-ttu-id="6cc5c-137">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="6cc5c-137">Application Name</span></span>|
|<span data-ttu-id="6cc5c-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="6cc5c-138">applicationType</span></span>|[<span data-ttu-id="6cc5c-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="6cc5c-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="6cc5c-140">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-140">Application Type.</span></span> <span data-ttu-id="6cc5c-141">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="6cc5c-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="6cc5c-142">deviceCount</span></span>|<span data-ttu-id="6cc5c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc5c-143">Int32</span></span>|<span data-ttu-id="6cc5c-144">设备计数</span><span class="sxs-lookup"><span data-stu-id="6cc5c-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="6cc5c-145">响应</span><span class="sxs-lookup"><span data-stu-id="6cc5c-145">Response</span></span>
<span data-ttu-id="6cc5c-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc5c-147">示例</span><span class="sxs-lookup"><span data-stu-id="6cc5c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cc5c-148">请求</span><span class="sxs-lookup"><span data-stu-id="6cc5c-148">Request</span></span>
<span data-ttu-id="6cc5c-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="6cc5c-150">响应</span><span class="sxs-lookup"><span data-stu-id="6cc5c-150">Response</span></span>
<span data-ttu-id="6cc5c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6cc5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






