---
title: 创建 unsupportedGroupPolicyExtension
description: 创建新的 unsupportedGroupPolicyExtension 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4527a57e68325e18634587661f1a15634ec8c75a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074557"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="bd0c7-103">创建 unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="bd0c7-103">Create unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="bd0c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd0c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd0c7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd0c7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd0c7-107">创建新的 [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-107">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd0c7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd0c7-108">Prerequisites</span></span>
<span data-ttu-id="bd0c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd0c7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd0c7-111">Permission type</span></span>|<span data-ttu-id="bd0c7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd0c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd0c7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd0c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd0c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd0c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd0c7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd0c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd0c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-116">Not supported.</span></span>|
|<span data-ttu-id="bd0c7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd0c7-117">Application</span></span>|<span data-ttu-id="bd0c7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd0c7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd0c7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd0c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="bd0c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd0c7-120">Request headers</span></span>
|<span data-ttu-id="bd0c7-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd0c7-121">Header</span></span>|<span data-ttu-id="bd0c7-122">值</span><span class="sxs-lookup"><span data-stu-id="bd0c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd0c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd0c7-123">Authorization</span></span>|<span data-ttu-id="bd0c7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd0c7-125">接受</span><span class="sxs-lookup"><span data-stu-id="bd0c7-125">Accept</span></span>|<span data-ttu-id="bd0c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd0c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd0c7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd0c7-127">Request body</span></span>
<span data-ttu-id="bd0c7-128">在请求正文中，提供 unsupportedGroupPolicyExtension 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-128">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="bd0c7-129">下表显示创建 unsupportedGroupPolicyExtension 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-129">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="bd0c7-130">属性</span><span class="sxs-lookup"><span data-stu-id="bd0c7-130">Property</span></span>|<span data-ttu-id="bd0c7-131">类型</span><span class="sxs-lookup"><span data-stu-id="bd0c7-131">Type</span></span>|<span data-ttu-id="bd0c7-132">说明</span><span class="sxs-lookup"><span data-stu-id="bd0c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd0c7-133">id</span><span class="sxs-lookup"><span data-stu-id="bd0c7-133">id</span></span>|<span data-ttu-id="bd0c7-134">String</span><span class="sxs-lookup"><span data-stu-id="bd0c7-134">String</span></span>|<span data-ttu-id="bd0c7-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bd0c7-135">Not yet documented</span></span>|
|<span data-ttu-id="bd0c7-136">settingScope</span><span class="sxs-lookup"><span data-stu-id="bd0c7-136">settingScope</span></span>|[<span data-ttu-id="bd0c7-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="bd0c7-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="bd0c7-138">设置不受支持的扩展的作用域。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="bd0c7-139">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="bd0c7-140">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="bd0c7-140">namespaceUrl</span></span>|<span data-ttu-id="bd0c7-141">String</span><span class="sxs-lookup"><span data-stu-id="bd0c7-141">String</span></span>|<span data-ttu-id="bd0c7-142">不受支持的扩展名的命名空间 Url。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="bd0c7-143">extensionType</span><span class="sxs-lookup"><span data-stu-id="bd0c7-143">extensionType</span></span>|<span data-ttu-id="bd0c7-144">String</span><span class="sxs-lookup"><span data-stu-id="bd0c7-144">String</span></span>|<span data-ttu-id="bd0c7-145">不支持的扩展名的 ExtensionType。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="bd0c7-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="bd0c7-146">nodeName</span></span>|<span data-ttu-id="bd0c7-147">String</span><span class="sxs-lookup"><span data-stu-id="bd0c7-147">String</span></span>|<span data-ttu-id="bd0c7-148">不受支持的扩展的节点名称。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="bd0c7-149">响应</span><span class="sxs-lookup"><span data-stu-id="bd0c7-149">Response</span></span>
<span data-ttu-id="bd0c7-150">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-150">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd0c7-151">示例</span><span class="sxs-lookup"><span data-stu-id="bd0c7-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd0c7-152">请求</span><span class="sxs-lookup"><span data-stu-id="bd0c7-152">Request</span></span>
<span data-ttu-id="bd0c7-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```

### <a name="response"></a><span data-ttu-id="bd0c7-154">响应</span><span class="sxs-lookup"><span data-stu-id="bd0c7-154">Response</span></span>
<span data-ttu-id="bd0c7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd0c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "e59ecce2-cce2-e59e-e2cc-9ee5e2cc9ee5",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```






