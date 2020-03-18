---
title: 更新 unsupportedGroupPolicyExtension
description: 更新 unsupportedGroupPolicyExtension 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b4e7d5656d78178a445d98c789d70246919ee07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804539"
---
# <a name="update-unsupportedgrouppolicyextension"></a><span data-ttu-id="46430-103">更新 unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="46430-103">Update unsupportedGroupPolicyExtension</span></span>

> <span data-ttu-id="46430-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46430-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46430-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46430-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46430-106">更新[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="46430-106">Update the properties of a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46430-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="46430-107">Prerequisites</span></span>
<span data-ttu-id="46430-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46430-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46430-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="46430-110">Permission type</span></span>|<span data-ttu-id="46430-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46430-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46430-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46430-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46430-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46430-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46430-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46430-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46430-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46430-115">Not supported.</span></span>|
|<span data-ttu-id="46430-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="46430-116">Application</span></span>|<span data-ttu-id="46430-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46430-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46430-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46430-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="request-headers"></a><span data-ttu-id="46430-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="46430-119">Request headers</span></span>
|<span data-ttu-id="46430-120">标头</span><span class="sxs-lookup"><span data-stu-id="46430-120">Header</span></span>|<span data-ttu-id="46430-121">值</span><span class="sxs-lookup"><span data-stu-id="46430-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46430-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46430-122">Authorization</span></span>|<span data-ttu-id="46430-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46430-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46430-124">接受</span><span class="sxs-lookup"><span data-stu-id="46430-124">Accept</span></span>|<span data-ttu-id="46430-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46430-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46430-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="46430-126">Request body</span></span>
<span data-ttu-id="46430-127">在请求正文中，提供[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46430-127">In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

<span data-ttu-id="46430-128">下表显示创建[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="46430-128">The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span></span>

|<span data-ttu-id="46430-129">属性</span><span class="sxs-lookup"><span data-stu-id="46430-129">Property</span></span>|<span data-ttu-id="46430-130">类型</span><span class="sxs-lookup"><span data-stu-id="46430-130">Type</span></span>|<span data-ttu-id="46430-131">说明</span><span class="sxs-lookup"><span data-stu-id="46430-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46430-132">id</span><span class="sxs-lookup"><span data-stu-id="46430-132">id</span></span>|<span data-ttu-id="46430-133">String</span><span class="sxs-lookup"><span data-stu-id="46430-133">String</span></span>|<span data-ttu-id="46430-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="46430-134">Not yet documented</span></span>|
|<span data-ttu-id="46430-135">settingScope</span><span class="sxs-lookup"><span data-stu-id="46430-135">settingScope</span></span>|[<span data-ttu-id="46430-136">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="46430-136">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="46430-137">设置不受支持的扩展的作用域。</span><span class="sxs-lookup"><span data-stu-id="46430-137">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="46430-138">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="46430-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="46430-139">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="46430-139">namespaceUrl</span></span>|<span data-ttu-id="46430-140">String</span><span class="sxs-lookup"><span data-stu-id="46430-140">String</span></span>|<span data-ttu-id="46430-141">不受支持的扩展名的命名空间 Url。</span><span class="sxs-lookup"><span data-stu-id="46430-141">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="46430-142">extensionType</span><span class="sxs-lookup"><span data-stu-id="46430-142">extensionType</span></span>|<span data-ttu-id="46430-143">String</span><span class="sxs-lookup"><span data-stu-id="46430-143">String</span></span>|<span data-ttu-id="46430-144">不支持的扩展名的 ExtensionType。</span><span class="sxs-lookup"><span data-stu-id="46430-144">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="46430-145">nodeName</span><span class="sxs-lookup"><span data-stu-id="46430-145">nodeName</span></span>|<span data-ttu-id="46430-146">String</span><span class="sxs-lookup"><span data-stu-id="46430-146">String</span></span>|<span data-ttu-id="46430-147">不受支持的扩展的节点名称。</span><span class="sxs-lookup"><span data-stu-id="46430-147">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="46430-148">响应</span><span class="sxs-lookup"><span data-stu-id="46430-148">Response</span></span>
<span data-ttu-id="46430-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="46430-149">If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46430-150">示例</span><span class="sxs-lookup"><span data-stu-id="46430-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="46430-151">请求</span><span class="sxs-lookup"><span data-stu-id="46430-151">Request</span></span>
<span data-ttu-id="46430-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46430-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
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

### <a name="response"></a><span data-ttu-id="46430-153">响应</span><span class="sxs-lookup"><span data-stu-id="46430-153">Response</span></span>
<span data-ttu-id="46430-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46430-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




