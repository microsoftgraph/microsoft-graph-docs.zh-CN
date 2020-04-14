---
title: 创建 windowsDefenderApplicationControlSupplementalPolicy
description: 创建新的 windowsDefenderApplicationControlSupplementalPolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2aaaa2d1933e8067a0830ad202a245c87441eccb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455388"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="4c8f0-103">创建 windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="4c8f0-103">Create windowsDefenderApplicationControlSupplementalPolicy</span></span>

<span data-ttu-id="4c8f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c8f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c8f0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c8f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c8f0-107">创建新的[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-107">Create a new [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c8f0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4c8f0-108">Prerequisites</span></span>
<span data-ttu-id="4c8f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c8f0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c8f0-111">Permission type</span></span>|<span data-ttu-id="4c8f0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4c8f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c8f0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c8f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c8f0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c8f0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c8f0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c8f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c8f0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-116">Not supported.</span></span>|
|<span data-ttu-id="4c8f0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c8f0-117">Application</span></span>|<span data-ttu-id="4c8f0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c8f0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c8f0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c8f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies
```

## <a name="request-headers"></a><span data-ttu-id="4c8f0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c8f0-120">Request headers</span></span>
|<span data-ttu-id="4c8f0-121">标头</span><span class="sxs-lookup"><span data-stu-id="4c8f0-121">Header</span></span>|<span data-ttu-id="4c8f0-122">值</span><span class="sxs-lookup"><span data-stu-id="4c8f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c8f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c8f0-123">Authorization</span></span>|<span data-ttu-id="4c8f0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c8f0-125">接受</span><span class="sxs-lookup"><span data-stu-id="4c8f0-125">Accept</span></span>|<span data-ttu-id="4c8f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c8f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c8f0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c8f0-127">Request body</span></span>
<span data-ttu-id="4c8f0-128">在请求正文中，提供 windowsDefenderApplicationControlSupplementalPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicy object.</span></span>

<span data-ttu-id="4c8f0-129">下表显示创建 windowsDefenderApplicationControlSupplementalPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicy.</span></span>

|<span data-ttu-id="4c8f0-130">属性</span><span class="sxs-lookup"><span data-stu-id="4c8f0-130">Property</span></span>|<span data-ttu-id="4c8f0-131">类型</span><span class="sxs-lookup"><span data-stu-id="4c8f0-131">Type</span></span>|<span data-ttu-id="4c8f0-132">说明</span><span class="sxs-lookup"><span data-stu-id="4c8f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c8f0-133">id</span><span class="sxs-lookup"><span data-stu-id="4c8f0-133">id</span></span>|<span data-ttu-id="4c8f0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4c8f0-134">String</span></span>|<span data-ttu-id="4c8f0-135">WindowsDefenderApplicationControl 补充策略的键。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-135">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="4c8f0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4c8f0-136">displayName</span></span>|<span data-ttu-id="4c8f0-137">字符串</span><span class="sxs-lookup"><span data-stu-id="4c8f0-137">String</span></span>|<span data-ttu-id="4c8f0-138">WindowsDefenderApplicationControl 补充策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-138">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="4c8f0-139">description</span><span class="sxs-lookup"><span data-stu-id="4c8f0-139">description</span></span>|<span data-ttu-id="4c8f0-140">String</span><span class="sxs-lookup"><span data-stu-id="4c8f0-140">String</span></span>|<span data-ttu-id="4c8f0-141">WindowsDefenderApplicationControl 补充策略的说明。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-141">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="4c8f0-142">content</span><span class="sxs-lookup"><span data-stu-id="4c8f0-142">content</span></span>|<span data-ttu-id="4c8f0-143">Binary</span><span class="sxs-lookup"><span data-stu-id="4c8f0-143">Binary</span></span>|<span data-ttu-id="4c8f0-144">WindowsDefenderApplicationControl 补充策略内容（以字节数组格式为单位）。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-144">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="4c8f0-145">contentFileName</span><span class="sxs-lookup"><span data-stu-id="4c8f0-145">contentFileName</span></span>|<span data-ttu-id="4c8f0-146">String</span><span class="sxs-lookup"><span data-stu-id="4c8f0-146">String</span></span>|<span data-ttu-id="4c8f0-147">WindowsDefenderApplicationControl 补充策略内容的文件名。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-147">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="4c8f0-148">version</span><span class="sxs-lookup"><span data-stu-id="4c8f0-148">version</span></span>|<span data-ttu-id="4c8f0-149">String</span><span class="sxs-lookup"><span data-stu-id="4c8f0-149">String</span></span>|<span data-ttu-id="4c8f0-150">WindowsDefenderApplicationControl 补充策略的版本。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-150">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="4c8f0-151">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="4c8f0-151">creationDateTime</span></span>|<span data-ttu-id="4c8f0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c8f0-152">DateTimeOffset</span></span>|<span data-ttu-id="4c8f0-153">上传 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-153">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="4c8f0-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c8f0-154">lastModifiedDateTime</span></span>|<span data-ttu-id="4c8f0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c8f0-155">DateTimeOffset</span></span>|<span data-ttu-id="4c8f0-156">上次修改 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-156">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="4c8f0-157">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4c8f0-157">roleScopeTagIds</span></span>|<span data-ttu-id="4c8f0-158">String 集合</span><span class="sxs-lookup"><span data-stu-id="4c8f0-158">String collection</span></span>|<span data-ttu-id="4c8f0-159">此 WindowsDefenderApplicationControl 补充策略实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-159">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4c8f0-160">响应</span><span class="sxs-lookup"><span data-stu-id="4c8f0-160">Response</span></span>
<span data-ttu-id="4c8f0-161">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-161">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c8f0-162">示例</span><span class="sxs-lookup"><span data-stu-id="4c8f0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c8f0-163">请求</span><span class="sxs-lookup"><span data-stu-id="4c8f0-163">Request</span></span>
<span data-ttu-id="4c8f0-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4c8f0-165">响应</span><span class="sxs-lookup"><span data-stu-id="4c8f0-165">Response</span></span>
<span data-ttu-id="4c8f0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c8f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "83d0c39e-c39e-83d0-9ec3-d0839ec3d083",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



