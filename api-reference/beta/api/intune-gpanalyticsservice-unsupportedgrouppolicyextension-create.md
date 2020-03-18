---
title: 创建 unsupportedGroupPolicyExtension
description: 创建新的 unsupportedGroupPolicyExtension 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5a7826e00c2b0bccb6fa7e3832995fa67ea9dbd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804567"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="1dbde-103">创建 unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="1dbde-103">Create unsupportedGroupPolicyExtension</span></span>

> <span data-ttu-id="1dbde-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1dbde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dbde-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1dbde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dbde-106">创建新的[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1dbde-106">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dbde-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1dbde-107">Prerequisites</span></span>
<span data-ttu-id="1dbde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1dbde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dbde-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dbde-110">Permission type</span></span>|<span data-ttu-id="1dbde-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1dbde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dbde-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dbde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dbde-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dbde-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1dbde-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dbde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dbde-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dbde-115">Not supported.</span></span>|
|<span data-ttu-id="1dbde-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1dbde-116">Application</span></span>|<span data-ttu-id="1dbde-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dbde-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dbde-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dbde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="1dbde-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dbde-119">Request headers</span></span>
|<span data-ttu-id="1dbde-120">标头</span><span class="sxs-lookup"><span data-stu-id="1dbde-120">Header</span></span>|<span data-ttu-id="1dbde-121">值</span><span class="sxs-lookup"><span data-stu-id="1dbde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dbde-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dbde-122">Authorization</span></span>|<span data-ttu-id="1dbde-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1dbde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dbde-124">接受</span><span class="sxs-lookup"><span data-stu-id="1dbde-124">Accept</span></span>|<span data-ttu-id="1dbde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1dbde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dbde-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dbde-126">Request body</span></span>
<span data-ttu-id="1dbde-127">在请求正文中，提供 unsupportedGroupPolicyExtension 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dbde-127">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="1dbde-128">下表显示创建 unsupportedGroupPolicyExtension 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1dbde-128">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="1dbde-129">属性</span><span class="sxs-lookup"><span data-stu-id="1dbde-129">Property</span></span>|<span data-ttu-id="1dbde-130">类型</span><span class="sxs-lookup"><span data-stu-id="1dbde-130">Type</span></span>|<span data-ttu-id="1dbde-131">说明</span><span class="sxs-lookup"><span data-stu-id="1dbde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dbde-132">id</span><span class="sxs-lookup"><span data-stu-id="1dbde-132">id</span></span>|<span data-ttu-id="1dbde-133">String</span><span class="sxs-lookup"><span data-stu-id="1dbde-133">String</span></span>|<span data-ttu-id="1dbde-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1dbde-134">Not yet documented</span></span>|
|<span data-ttu-id="1dbde-135">settingScope</span><span class="sxs-lookup"><span data-stu-id="1dbde-135">settingScope</span></span>|[<span data-ttu-id="1dbde-136">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="1dbde-136">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="1dbde-137">设置不受支持的扩展的作用域。</span><span class="sxs-lookup"><span data-stu-id="1dbde-137">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="1dbde-138">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="1dbde-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="1dbde-139">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="1dbde-139">namespaceUrl</span></span>|<span data-ttu-id="1dbde-140">String</span><span class="sxs-lookup"><span data-stu-id="1dbde-140">String</span></span>|<span data-ttu-id="1dbde-141">不受支持的扩展名的命名空间 Url。</span><span class="sxs-lookup"><span data-stu-id="1dbde-141">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="1dbde-142">extensionType</span><span class="sxs-lookup"><span data-stu-id="1dbde-142">extensionType</span></span>|<span data-ttu-id="1dbde-143">String</span><span class="sxs-lookup"><span data-stu-id="1dbde-143">String</span></span>|<span data-ttu-id="1dbde-144">不支持的扩展名的 ExtensionType。</span><span class="sxs-lookup"><span data-stu-id="1dbde-144">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="1dbde-145">nodeName</span><span class="sxs-lookup"><span data-stu-id="1dbde-145">nodeName</span></span>|<span data-ttu-id="1dbde-146">String</span><span class="sxs-lookup"><span data-stu-id="1dbde-146">String</span></span>|<span data-ttu-id="1dbde-147">不受支持的扩展的节点名称。</span><span class="sxs-lookup"><span data-stu-id="1dbde-147">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="1dbde-148">响应</span><span class="sxs-lookup"><span data-stu-id="1dbde-148">Response</span></span>
<span data-ttu-id="1dbde-149">如果成功，此方法在响应`201 Created`正文中返回响应代码和[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1dbde-149">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dbde-150">示例</span><span class="sxs-lookup"><span data-stu-id="1dbde-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dbde-151">请求</span><span class="sxs-lookup"><span data-stu-id="1dbde-151">Request</span></span>
<span data-ttu-id="1dbde-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1dbde-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1dbde-153">响应</span><span class="sxs-lookup"><span data-stu-id="1dbde-153">Response</span></span>
<span data-ttu-id="1dbde-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1dbde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




