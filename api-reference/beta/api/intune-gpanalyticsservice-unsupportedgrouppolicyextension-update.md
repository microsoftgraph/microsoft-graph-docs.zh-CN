---
title: 更新 unsupportedGroupPolicyExtension
description: 更新 unsupportedGroupPolicyExtension 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00c5b7be1421c4591d4b4f615cb394402c362114
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685112"
---
# <a name="update-unsupportedgrouppolicyextension"></a><span data-ttu-id="32721-103">更新 unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="32721-103">Update unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="32721-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32721-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32721-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32721-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32721-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32721-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32721-107">更新 [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="32721-107">Update the properties of a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32721-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="32721-108">Prerequisites</span></span>
<span data-ttu-id="32721-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32721-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="32721-111">Permission type</span></span>|<span data-ttu-id="32721-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32721-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32721-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32721-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32721-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32721-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32721-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32721-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32721-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="32721-116">Not supported.</span></span>|
|<span data-ttu-id="32721-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="32721-117">Application</span></span>|<span data-ttu-id="32721-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32721-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32721-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32721-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="request-headers"></a><span data-ttu-id="32721-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="32721-120">Request headers</span></span>
|<span data-ttu-id="32721-121">标头</span><span class="sxs-lookup"><span data-stu-id="32721-121">Header</span></span>|<span data-ttu-id="32721-122">值</span><span class="sxs-lookup"><span data-stu-id="32721-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32721-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32721-123">Authorization</span></span>|<span data-ttu-id="32721-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32721-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32721-125">接受</span><span class="sxs-lookup"><span data-stu-id="32721-125">Accept</span></span>|<span data-ttu-id="32721-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32721-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32721-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="32721-127">Request body</span></span>
<span data-ttu-id="32721-128">在请求正文中，提供 [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32721-128">In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

<span data-ttu-id="32721-129">下表显示创建 [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="32721-129">The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span></span>

|<span data-ttu-id="32721-130">属性</span><span class="sxs-lookup"><span data-stu-id="32721-130">Property</span></span>|<span data-ttu-id="32721-131">类型</span><span class="sxs-lookup"><span data-stu-id="32721-131">Type</span></span>|<span data-ttu-id="32721-132">说明</span><span class="sxs-lookup"><span data-stu-id="32721-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32721-133">id</span><span class="sxs-lookup"><span data-stu-id="32721-133">id</span></span>|<span data-ttu-id="32721-134">String</span><span class="sxs-lookup"><span data-stu-id="32721-134">String</span></span>|<span data-ttu-id="32721-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="32721-135">Not yet documented</span></span>|
|<span data-ttu-id="32721-136">settingScope</span><span class="sxs-lookup"><span data-stu-id="32721-136">settingScope</span></span>|[<span data-ttu-id="32721-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="32721-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="32721-138">设置不受支持的扩展的作用域。</span><span class="sxs-lookup"><span data-stu-id="32721-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="32721-139">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="32721-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="32721-140">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="32721-140">namespaceUrl</span></span>|<span data-ttu-id="32721-141">String</span><span class="sxs-lookup"><span data-stu-id="32721-141">String</span></span>|<span data-ttu-id="32721-142">不受支持的扩展名的命名空间 Url。</span><span class="sxs-lookup"><span data-stu-id="32721-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="32721-143">extensionType</span><span class="sxs-lookup"><span data-stu-id="32721-143">extensionType</span></span>|<span data-ttu-id="32721-144">String</span><span class="sxs-lookup"><span data-stu-id="32721-144">String</span></span>|<span data-ttu-id="32721-145">不支持的扩展名的 ExtensionType。</span><span class="sxs-lookup"><span data-stu-id="32721-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="32721-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="32721-146">nodeName</span></span>|<span data-ttu-id="32721-147">String</span><span class="sxs-lookup"><span data-stu-id="32721-147">String</span></span>|<span data-ttu-id="32721-148">不受支持的扩展的节点名称。</span><span class="sxs-lookup"><span data-stu-id="32721-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="32721-149">响应</span><span class="sxs-lookup"><span data-stu-id="32721-149">Response</span></span>
<span data-ttu-id="32721-150">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32721-150">If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32721-151">示例</span><span class="sxs-lookup"><span data-stu-id="32721-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="32721-152">请求</span><span class="sxs-lookup"><span data-stu-id="32721-152">Request</span></span>
<span data-ttu-id="32721-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32721-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32721-154">响应</span><span class="sxs-lookup"><span data-stu-id="32721-154">Response</span></span>
<span data-ttu-id="32721-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32721-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





