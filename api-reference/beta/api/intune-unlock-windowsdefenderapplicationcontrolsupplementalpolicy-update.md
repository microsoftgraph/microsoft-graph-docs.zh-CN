---
title: 更新 windowsDefenderApplicationControlSupplementalPolicy
description: 更新 windowsDefenderApplicationControlSupplementalPolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 508abb01a53264a7e206b5f5756c7cf7b7716365
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731461"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="d60c1-103">更新 windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="d60c1-103">Update windowsDefenderApplicationControlSupplementalPolicy</span></span>

<span data-ttu-id="d60c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d60c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d60c1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d60c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d60c1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d60c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d60c1-107">更新 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d60c1-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d60c1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d60c1-108">Prerequisites</span></span>
<span data-ttu-id="d60c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d60c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d60c1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d60c1-111">Permission type</span></span>|<span data-ttu-id="d60c1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d60c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d60c1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d60c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d60c1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d60c1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d60c1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d60c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d60c1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d60c1-116">Not supported.</span></span>|
|<span data-ttu-id="d60c1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d60c1-117">Application</span></span>|<span data-ttu-id="d60c1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d60c1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d60c1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d60c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a><span data-ttu-id="d60c1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d60c1-120">Request headers</span></span>
|<span data-ttu-id="d60c1-121">标头</span><span class="sxs-lookup"><span data-stu-id="d60c1-121">Header</span></span>|<span data-ttu-id="d60c1-122">值</span><span class="sxs-lookup"><span data-stu-id="d60c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d60c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d60c1-123">Authorization</span></span>|<span data-ttu-id="d60c1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d60c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d60c1-125">接受</span><span class="sxs-lookup"><span data-stu-id="d60c1-125">Accept</span></span>|<span data-ttu-id="d60c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d60c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d60c1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d60c1-127">Request body</span></span>
<span data-ttu-id="d60c1-128">在请求正文中，提供 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d60c1-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

<span data-ttu-id="d60c1-129">下表显示创建 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d60c1-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span></span>

|<span data-ttu-id="d60c1-130">属性</span><span class="sxs-lookup"><span data-stu-id="d60c1-130">Property</span></span>|<span data-ttu-id="d60c1-131">类型</span><span class="sxs-lookup"><span data-stu-id="d60c1-131">Type</span></span>|<span data-ttu-id="d60c1-132">说明</span><span class="sxs-lookup"><span data-stu-id="d60c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d60c1-133">id</span><span class="sxs-lookup"><span data-stu-id="d60c1-133">id</span></span>|<span data-ttu-id="d60c1-134">String</span><span class="sxs-lookup"><span data-stu-id="d60c1-134">String</span></span>|<span data-ttu-id="d60c1-135">WindowsDefenderApplicationControl 补充策略的键。</span><span class="sxs-lookup"><span data-stu-id="d60c1-135">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="d60c1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d60c1-136">displayName</span></span>|<span data-ttu-id="d60c1-137">String</span><span class="sxs-lookup"><span data-stu-id="d60c1-137">String</span></span>|<span data-ttu-id="d60c1-138">WindowsDefenderApplicationControl 补充策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d60c1-138">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="d60c1-139">说明</span><span class="sxs-lookup"><span data-stu-id="d60c1-139">description</span></span>|<span data-ttu-id="d60c1-140">String</span><span class="sxs-lookup"><span data-stu-id="d60c1-140">String</span></span>|<span data-ttu-id="d60c1-141">WindowsDefenderApplicationControl 补充策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d60c1-141">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="d60c1-142">content</span><span class="sxs-lookup"><span data-stu-id="d60c1-142">content</span></span>|<span data-ttu-id="d60c1-143">Binary</span><span class="sxs-lookup"><span data-stu-id="d60c1-143">Binary</span></span>|<span data-ttu-id="d60c1-144">WindowsDefenderApplicationControl 补充策略内容（以字节数组格式为单位）。</span><span class="sxs-lookup"><span data-stu-id="d60c1-144">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="d60c1-145">contentFileName</span><span class="sxs-lookup"><span data-stu-id="d60c1-145">contentFileName</span></span>|<span data-ttu-id="d60c1-146">String</span><span class="sxs-lookup"><span data-stu-id="d60c1-146">String</span></span>|<span data-ttu-id="d60c1-147">WindowsDefenderApplicationControl 补充策略内容的文件名。</span><span class="sxs-lookup"><span data-stu-id="d60c1-147">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="d60c1-148">version</span><span class="sxs-lookup"><span data-stu-id="d60c1-148">version</span></span>|<span data-ttu-id="d60c1-149">String</span><span class="sxs-lookup"><span data-stu-id="d60c1-149">String</span></span>|<span data-ttu-id="d60c1-150">WindowsDefenderApplicationControl 补充策略的版本。</span><span class="sxs-lookup"><span data-stu-id="d60c1-150">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="d60c1-151">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="d60c1-151">creationDateTime</span></span>|<span data-ttu-id="d60c1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d60c1-152">DateTimeOffset</span></span>|<span data-ttu-id="d60c1-153">上传 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d60c1-153">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="d60c1-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d60c1-154">lastModifiedDateTime</span></span>|<span data-ttu-id="d60c1-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d60c1-155">DateTimeOffset</span></span>|<span data-ttu-id="d60c1-156">上次修改 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d60c1-156">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="d60c1-157">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d60c1-157">roleScopeTagIds</span></span>|<span data-ttu-id="d60c1-158">String collection</span><span class="sxs-lookup"><span data-stu-id="d60c1-158">String collection</span></span>|<span data-ttu-id="d60c1-159">此 WindowsDefenderApplicationControl 补充策略实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="d60c1-159">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d60c1-160">响应</span><span class="sxs-lookup"><span data-stu-id="d60c1-160">Response</span></span>
<span data-ttu-id="d60c1-161">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d60c1-161">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d60c1-162">示例</span><span class="sxs-lookup"><span data-stu-id="d60c1-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="d60c1-163">请求</span><span class="sxs-lookup"><span data-stu-id="d60c1-163">Request</span></span>
<span data-ttu-id="d60c1-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d60c1-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d60c1-165">响应</span><span class="sxs-lookup"><span data-stu-id="d60c1-165">Response</span></span>
<span data-ttu-id="d60c1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d60c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





