---
title: 创建 windowsInformationProtectionAppLearningSummary
description: 创建新的 windowsInformationProtectionAppLearningSummary 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c39303154cbf09d6aedb1080d0560885e91133e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407758"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="ab885-103">创建 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="ab885-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="ab885-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ab885-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab885-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab885-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab885-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab885-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab885-107">创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab885-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab885-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab885-108">Prerequisites</span></span>
<span data-ttu-id="ab885-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ab885-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ab885-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab885-111">Permission type</span></span>|<span data-ttu-id="ab885-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab885-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab885-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab885-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab885-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab885-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab885-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab885-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab885-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab885-116">Not supported.</span></span>|
|<span data-ttu-id="ab885-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab885-117">Application</span></span>|<span data-ttu-id="ab885-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab885-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab885-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab885-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ab885-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab885-120">Request headers</span></span>
|<span data-ttu-id="ab885-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab885-121">Header</span></span>|<span data-ttu-id="ab885-122">值</span><span class="sxs-lookup"><span data-stu-id="ab885-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab885-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab885-123">Authorization</span></span>|<span data-ttu-id="ab885-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab885-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab885-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab885-125">Accept</span></span>|<span data-ttu-id="ab885-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab885-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab885-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab885-127">Request body</span></span>
<span data-ttu-id="ab885-128">在请求正文中，提供 windowsInformationProtectionAppLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab885-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="ab885-129">下表显示创建 windowsInformationProtectionAppLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab885-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="ab885-130">属性</span><span class="sxs-lookup"><span data-stu-id="ab885-130">Property</span></span>|<span data-ttu-id="ab885-131">类型</span><span class="sxs-lookup"><span data-stu-id="ab885-131">Type</span></span>|<span data-ttu-id="ab885-132">说明</span><span class="sxs-lookup"><span data-stu-id="ab885-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab885-133">id</span><span class="sxs-lookup"><span data-stu-id="ab885-133">id</span></span>|<span data-ttu-id="ab885-134">String</span><span class="sxs-lookup"><span data-stu-id="ab885-134">String</span></span>|<span data-ttu-id="ab885-135">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ab885-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="ab885-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="ab885-136">applicationName</span></span>|<span data-ttu-id="ab885-137">String</span><span class="sxs-lookup"><span data-stu-id="ab885-137">String</span></span>|<span data-ttu-id="ab885-138">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="ab885-138">Application Name</span></span>|
|<span data-ttu-id="ab885-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="ab885-139">applicationType</span></span>|[<span data-ttu-id="ab885-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="ab885-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="ab885-141">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="ab885-141">Application Type.</span></span> <span data-ttu-id="ab885-142">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="ab885-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="ab885-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ab885-143">deviceCount</span></span>|<span data-ttu-id="ab885-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ab885-144">Int32</span></span>|<span data-ttu-id="ab885-145">设备计数</span><span class="sxs-lookup"><span data-stu-id="ab885-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="ab885-146">响应</span><span class="sxs-lookup"><span data-stu-id="ab885-146">Response</span></span>
<span data-ttu-id="ab885-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab885-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab885-148">示例</span><span class="sxs-lookup"><span data-stu-id="ab885-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab885-149">请求</span><span class="sxs-lookup"><span data-stu-id="ab885-149">Request</span></span>
<span data-ttu-id="ab885-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab885-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ab885-151">响应</span><span class="sxs-lookup"><span data-stu-id="ab885-151">Response</span></span>
<span data-ttu-id="ab885-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab885-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




