---
title: 创建 windowsInformationProtectionAppLearningSummary
description: 创建新的 windowsInformationProtectionAppLearningSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a4145594557f526ea9dfaf70736529cd83eee5b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743061"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="67872-103">创建 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="67872-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="67872-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67872-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67872-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67872-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67872-106">创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67872-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67872-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="67872-107">Prerequisites</span></span>
<span data-ttu-id="67872-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67872-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67872-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="67872-110">Permission type</span></span>|<span data-ttu-id="67872-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67872-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67872-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67872-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67872-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67872-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67872-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67872-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67872-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="67872-115">Not supported.</span></span>|
|<span data-ttu-id="67872-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="67872-116">Application</span></span>|<span data-ttu-id="67872-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67872-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67872-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67872-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="67872-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="67872-119">Request headers</span></span>
|<span data-ttu-id="67872-120">标头</span><span class="sxs-lookup"><span data-stu-id="67872-120">Header</span></span>|<span data-ttu-id="67872-121">值</span><span class="sxs-lookup"><span data-stu-id="67872-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67872-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67872-122">Authorization</span></span>|<span data-ttu-id="67872-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="67872-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67872-124">接受</span><span class="sxs-lookup"><span data-stu-id="67872-124">Accept</span></span>|<span data-ttu-id="67872-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67872-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67872-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="67872-126">Request body</span></span>
<span data-ttu-id="67872-127">在请求正文中，提供 windowsInformationProtectionAppLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67872-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="67872-128">下表显示创建 windowsInformationProtectionAppLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="67872-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="67872-129">属性</span><span class="sxs-lookup"><span data-stu-id="67872-129">Property</span></span>|<span data-ttu-id="67872-130">类型</span><span class="sxs-lookup"><span data-stu-id="67872-130">Type</span></span>|<span data-ttu-id="67872-131">说明</span><span class="sxs-lookup"><span data-stu-id="67872-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67872-132">id</span><span class="sxs-lookup"><span data-stu-id="67872-132">id</span></span>|<span data-ttu-id="67872-133">String</span><span class="sxs-lookup"><span data-stu-id="67872-133">String</span></span>|<span data-ttu-id="67872-134">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67872-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="67872-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="67872-135">applicationName</span></span>|<span data-ttu-id="67872-136">String</span><span class="sxs-lookup"><span data-stu-id="67872-136">String</span></span>|<span data-ttu-id="67872-137">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="67872-137">Application Name</span></span>|
|<span data-ttu-id="67872-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="67872-138">applicationType</span></span>|[<span data-ttu-id="67872-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="67872-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="67872-140">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="67872-140">Application Type.</span></span> <span data-ttu-id="67872-141">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="67872-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="67872-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="67872-142">deviceCount</span></span>|<span data-ttu-id="67872-143">Int32</span><span class="sxs-lookup"><span data-stu-id="67872-143">Int32</span></span>|<span data-ttu-id="67872-144">设备计数</span><span class="sxs-lookup"><span data-stu-id="67872-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="67872-145">响应</span><span class="sxs-lookup"><span data-stu-id="67872-145">Response</span></span>
<span data-ttu-id="67872-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67872-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67872-147">示例</span><span class="sxs-lookup"><span data-stu-id="67872-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="67872-148">请求</span><span class="sxs-lookup"><span data-stu-id="67872-148">Request</span></span>
<span data-ttu-id="67872-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67872-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="67872-150">响应</span><span class="sxs-lookup"><span data-stu-id="67872-150">Response</span></span>
<span data-ttu-id="67872-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67872-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




