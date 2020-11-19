---
title: 创建 windowsDefenderApplicationControlSupplementalPolicy
description: 创建新的 windowsDefenderApplicationControlSupplementalPolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc0c4da7196b5fb679f5e3addf0826ff0d8dd6fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49289130"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="bfaff-103">创建 windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="bfaff-103">Create windowsDefenderApplicationControlSupplementalPolicy</span></span>

<span data-ttu-id="bfaff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfaff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfaff-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bfaff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfaff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bfaff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfaff-107">创建新的 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bfaff-107">Create a new [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfaff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bfaff-108">Prerequisites</span></span>
<span data-ttu-id="bfaff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfaff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfaff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfaff-111">Permission type</span></span>|<span data-ttu-id="bfaff-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bfaff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfaff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfaff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfaff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfaff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bfaff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfaff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfaff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfaff-116">Not supported.</span></span>|
|<span data-ttu-id="bfaff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfaff-117">Application</span></span>|<span data-ttu-id="bfaff-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfaff-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfaff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfaff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies
```

## <a name="request-headers"></a><span data-ttu-id="bfaff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfaff-120">Request headers</span></span>
|<span data-ttu-id="bfaff-121">标头</span><span class="sxs-lookup"><span data-stu-id="bfaff-121">Header</span></span>|<span data-ttu-id="bfaff-122">值</span><span class="sxs-lookup"><span data-stu-id="bfaff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfaff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfaff-123">Authorization</span></span>|<span data-ttu-id="bfaff-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bfaff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfaff-125">接受</span><span class="sxs-lookup"><span data-stu-id="bfaff-125">Accept</span></span>|<span data-ttu-id="bfaff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfaff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfaff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfaff-127">Request body</span></span>
<span data-ttu-id="bfaff-128">在请求正文中，提供 windowsDefenderApplicationControlSupplementalPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfaff-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicy object.</span></span>

<span data-ttu-id="bfaff-129">下表显示创建 windowsDefenderApplicationControlSupplementalPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bfaff-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicy.</span></span>

|<span data-ttu-id="bfaff-130">属性</span><span class="sxs-lookup"><span data-stu-id="bfaff-130">Property</span></span>|<span data-ttu-id="bfaff-131">类型</span><span class="sxs-lookup"><span data-stu-id="bfaff-131">Type</span></span>|<span data-ttu-id="bfaff-132">说明</span><span class="sxs-lookup"><span data-stu-id="bfaff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfaff-133">id</span><span class="sxs-lookup"><span data-stu-id="bfaff-133">id</span></span>|<span data-ttu-id="bfaff-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bfaff-134">String</span></span>|<span data-ttu-id="bfaff-135">WindowsDefenderApplicationControl 补充策略的键。</span><span class="sxs-lookup"><span data-stu-id="bfaff-135">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="bfaff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bfaff-136">displayName</span></span>|<span data-ttu-id="bfaff-137">字符串</span><span class="sxs-lookup"><span data-stu-id="bfaff-137">String</span></span>|<span data-ttu-id="bfaff-138">WindowsDefenderApplicationControl 补充策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bfaff-138">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="bfaff-139">description</span><span class="sxs-lookup"><span data-stu-id="bfaff-139">description</span></span>|<span data-ttu-id="bfaff-140">字符串</span><span class="sxs-lookup"><span data-stu-id="bfaff-140">String</span></span>|<span data-ttu-id="bfaff-141">WindowsDefenderApplicationControl 补充策略的说明。</span><span class="sxs-lookup"><span data-stu-id="bfaff-141">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="bfaff-142">content</span><span class="sxs-lookup"><span data-stu-id="bfaff-142">content</span></span>|<span data-ttu-id="bfaff-143">Binary</span><span class="sxs-lookup"><span data-stu-id="bfaff-143">Binary</span></span>|<span data-ttu-id="bfaff-144">WindowsDefenderApplicationControl 补充策略内容（以字节数组格式为单位）。</span><span class="sxs-lookup"><span data-stu-id="bfaff-144">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="bfaff-145">contentFileName</span><span class="sxs-lookup"><span data-stu-id="bfaff-145">contentFileName</span></span>|<span data-ttu-id="bfaff-146">字符串</span><span class="sxs-lookup"><span data-stu-id="bfaff-146">String</span></span>|<span data-ttu-id="bfaff-147">WindowsDefenderApplicationControl 补充策略内容的文件名。</span><span class="sxs-lookup"><span data-stu-id="bfaff-147">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="bfaff-148">version</span><span class="sxs-lookup"><span data-stu-id="bfaff-148">version</span></span>|<span data-ttu-id="bfaff-149">String</span><span class="sxs-lookup"><span data-stu-id="bfaff-149">String</span></span>|<span data-ttu-id="bfaff-150">WindowsDefenderApplicationControl 补充策略的版本。</span><span class="sxs-lookup"><span data-stu-id="bfaff-150">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="bfaff-151">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="bfaff-151">creationDateTime</span></span>|<span data-ttu-id="bfaff-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfaff-152">DateTimeOffset</span></span>|<span data-ttu-id="bfaff-153">上传 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bfaff-153">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="bfaff-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfaff-154">lastModifiedDateTime</span></span>|<span data-ttu-id="bfaff-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfaff-155">DateTimeOffset</span></span>|<span data-ttu-id="bfaff-156">上次修改 WindowsDefenderApplicationControl 补充策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bfaff-156">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="bfaff-157">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bfaff-157">roleScopeTagIds</span></span>|<span data-ttu-id="bfaff-158">String 集合</span><span class="sxs-lookup"><span data-stu-id="bfaff-158">String collection</span></span>|<span data-ttu-id="bfaff-159">此 WindowsDefenderApplicationControl 补充策略实体的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="bfaff-159">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="bfaff-160">响应</span><span class="sxs-lookup"><span data-stu-id="bfaff-160">Response</span></span>
<span data-ttu-id="bfaff-161">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bfaff-161">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfaff-162">示例</span><span class="sxs-lookup"><span data-stu-id="bfaff-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfaff-163">请求</span><span class="sxs-lookup"><span data-stu-id="bfaff-163">Request</span></span>
<span data-ttu-id="bfaff-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfaff-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bfaff-165">响应</span><span class="sxs-lookup"><span data-stu-id="bfaff-165">Response</span></span>
<span data-ttu-id="bfaff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bfaff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




