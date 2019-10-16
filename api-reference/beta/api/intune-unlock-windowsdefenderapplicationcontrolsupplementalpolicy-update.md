---
title: 更新 windowsDefenderApplicationControlSupplementalPolicy
description: 更新 windowsDefenderApplicationControlSupplementalPolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bcffdbcd4b1e18cd97262850ba3fc44c5e955c5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536684"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="c8418-103">更新 windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="c8418-103">Update windowsDefenderApplicationControlSupplementalPolicy</span></span>

> <span data-ttu-id="c8418-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8418-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8418-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8418-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8418-106">更新[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8418-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8418-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c8418-107">Prerequisites</span></span>
<span data-ttu-id="c8418-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8418-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8418-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8418-110">Permission type</span></span>|<span data-ttu-id="c8418-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8418-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8418-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8418-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8418-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8418-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8418-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8418-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8418-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8418-115">Not supported.</span></span>|
|<span data-ttu-id="c8418-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8418-116">Application</span></span>|<span data-ttu-id="c8418-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8418-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8418-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8418-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a><span data-ttu-id="c8418-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8418-119">Request headers</span></span>
|<span data-ttu-id="c8418-120">标头</span><span class="sxs-lookup"><span data-stu-id="c8418-120">Header</span></span>|<span data-ttu-id="c8418-121">值</span><span class="sxs-lookup"><span data-stu-id="c8418-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8418-122">授权</span><span class="sxs-lookup"><span data-stu-id="c8418-122">Authorization</span></span>|<span data-ttu-id="c8418-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c8418-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8418-124">接受</span><span class="sxs-lookup"><span data-stu-id="c8418-124">Accept</span></span>|<span data-ttu-id="c8418-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8418-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8418-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8418-126">Request body</span></span>
<span data-ttu-id="c8418-127">在请求正文中，提供[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8418-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

<span data-ttu-id="c8418-128">下表显示创建[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c8418-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span></span>

|<span data-ttu-id="c8418-129">属性</span><span class="sxs-lookup"><span data-stu-id="c8418-129">Property</span></span>|<span data-ttu-id="c8418-130">类型</span><span class="sxs-lookup"><span data-stu-id="c8418-130">Type</span></span>|<span data-ttu-id="c8418-131">说明</span><span class="sxs-lookup"><span data-stu-id="c8418-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8418-132">id</span><span class="sxs-lookup"><span data-stu-id="c8418-132">id</span></span>|<span data-ttu-id="c8418-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c8418-133">String</span></span>|<span data-ttu-id="c8418-134">WindowsDefenderApplicationControl 补充策略的键。</span><span class="sxs-lookup"><span data-stu-id="c8418-134">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="c8418-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c8418-135">displayName</span></span>|<span data-ttu-id="c8418-136">字符串</span><span class="sxs-lookup"><span data-stu-id="c8418-136">String</span></span>|<span data-ttu-id="c8418-137">WindowsDefenderApplicationControl 补充策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c8418-137">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="c8418-138">说明</span><span class="sxs-lookup"><span data-stu-id="c8418-138">description</span></span>|<span data-ttu-id="c8418-139">String</span><span class="sxs-lookup"><span data-stu-id="c8418-139">String</span></span>|<span data-ttu-id="c8418-140">WindowsDefenderApplicationControl 补充策略的说明。</span><span class="sxs-lookup"><span data-stu-id="c8418-140">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="c8418-141">content</span><span class="sxs-lookup"><span data-stu-id="c8418-141">content</span></span>|<span data-ttu-id="c8418-142">Binary</span><span class="sxs-lookup"><span data-stu-id="c8418-142">Binary</span></span>|<span data-ttu-id="c8418-143">WindowsDefenderApplicationControl 补充策略内容（以字节数组格式为单位）。</span><span class="sxs-lookup"><span data-stu-id="c8418-143">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="c8418-144">contentFileName</span><span class="sxs-lookup"><span data-stu-id="c8418-144">contentFileName</span></span>|<span data-ttu-id="c8418-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c8418-145">String</span></span>|<span data-ttu-id="c8418-146">WindowsDefenderApplicationControl 补充策略内容的文件名。</span><span class="sxs-lookup"><span data-stu-id="c8418-146">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="c8418-147">version</span><span class="sxs-lookup"><span data-stu-id="c8418-147">version</span></span>|<span data-ttu-id="c8418-148">String</span><span class="sxs-lookup"><span data-stu-id="c8418-148">String</span></span>|<span data-ttu-id="c8418-149">WindowsDefenderApplicationControl 补充策略的版本。</span><span class="sxs-lookup"><span data-stu-id="c8418-149">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="c8418-150">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="c8418-150">creationDateTime</span></span>|<span data-ttu-id="c8418-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8418-151">DateTimeOffset</span></span>|<span data-ttu-id="c8418-152">上传 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c8418-152">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="c8418-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8418-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c8418-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8418-154">DateTimeOffset</span></span>|<span data-ttu-id="c8418-155">上次修改 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c8418-155">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="c8418-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c8418-156">roleScopeTagIds</span></span>|<span data-ttu-id="c8418-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="c8418-157">String collection</span></span>|<span data-ttu-id="c8418-158">此 WindowsDefenderApplicationControl 补充策略实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="c8418-158">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c8418-159">响应</span><span class="sxs-lookup"><span data-stu-id="c8418-159">Response</span></span>
<span data-ttu-id="c8418-160">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8418-160">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8418-161">示例</span><span class="sxs-lookup"><span data-stu-id="c8418-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8418-162">请求</span><span class="sxs-lookup"><span data-stu-id="c8418-162">Request</span></span>
<span data-ttu-id="c8418-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8418-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
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

### <a name="response"></a><span data-ttu-id="c8418-164">响应</span><span class="sxs-lookup"><span data-stu-id="c8418-164">Response</span></span>
<span data-ttu-id="c8418-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8418-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






