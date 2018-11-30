---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
ms.openlocfilehash: 380b4b9358c3bc30337272ced4b92563978d7ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046131"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="04f98-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="04f98-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="04f98-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04f98-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04f98-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04f98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04f98-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04f98-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04f98-107">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04f98-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04f98-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="04f98-108">Prerequisites</span></span>
<span data-ttu-id="04f98-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="04f98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f98-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="04f98-111">Permission type</span></span>|<span data-ttu-id="04f98-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04f98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04f98-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04f98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04f98-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f98-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04f98-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04f98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04f98-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04f98-116">Not supported.</span></span>|
|<span data-ttu-id="04f98-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="04f98-117">Application</span></span>|<span data-ttu-id="04f98-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="04f98-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04f98-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04f98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="04f98-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="04f98-120">Request headers</span></span>
|<span data-ttu-id="04f98-121">标头</span><span class="sxs-lookup"><span data-stu-id="04f98-121">Header</span></span>|<span data-ttu-id="04f98-122">值</span><span class="sxs-lookup"><span data-stu-id="04f98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04f98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f98-123">Authorization</span></span>|<span data-ttu-id="04f98-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04f98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04f98-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04f98-125">Accept</span></span>|<span data-ttu-id="04f98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04f98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04f98-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="04f98-127">Request body</span></span>
<span data-ttu-id="04f98-128">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04f98-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="04f98-129">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04f98-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="04f98-130">属性</span><span class="sxs-lookup"><span data-stu-id="04f98-130">Property</span></span>|<span data-ttu-id="04f98-131">类型</span><span class="sxs-lookup"><span data-stu-id="04f98-131">Type</span></span>|<span data-ttu-id="04f98-132">说明</span><span class="sxs-lookup"><span data-stu-id="04f98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f98-133">displayName</span><span class="sxs-lookup"><span data-stu-id="04f98-133">displayName</span></span>|<span data-ttu-id="04f98-134">String</span><span class="sxs-lookup"><span data-stu-id="04f98-134">String</span></span>|<span data-ttu-id="04f98-135">友好名称</span><span class="sxs-lookup"><span data-stu-id="04f98-135">The friendly name</span></span>|
|<span data-ttu-id="04f98-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="04f98-136">fileHash</span></span>|<span data-ttu-id="04f98-137">String</span><span class="sxs-lookup"><span data-stu-id="04f98-137">String</span></span>|<span data-ttu-id="04f98-138">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="04f98-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="04f98-139">file</span><span class="sxs-lookup"><span data-stu-id="04f98-139">file</span></span>|<span data-ttu-id="04f98-140">Binary</span><span class="sxs-lookup"><span data-stu-id="04f98-140">Binary</span></span>|<span data-ttu-id="04f98-141">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="04f98-141">File as a byte array</span></span>|
|<span data-ttu-id="04f98-142">id</span><span class="sxs-lookup"><span data-stu-id="04f98-142">id</span></span>|<span data-ttu-id="04f98-143">String</span><span class="sxs-lookup"><span data-stu-id="04f98-143">String</span></span>|<span data-ttu-id="04f98-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="04f98-144">Key of the entity.</span></span>|
|<span data-ttu-id="04f98-145">version</span><span class="sxs-lookup"><span data-stu-id="04f98-145">version</span></span>|<span data-ttu-id="04f98-146">String</span><span class="sxs-lookup"><span data-stu-id="04f98-146">String</span></span>|<span data-ttu-id="04f98-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="04f98-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="04f98-148">响应</span><span class="sxs-lookup"><span data-stu-id="04f98-148">Response</span></span>
<span data-ttu-id="04f98-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04f98-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04f98-150">示例</span><span class="sxs-lookup"><span data-stu-id="04f98-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="04f98-151">请求</span><span class="sxs-lookup"><span data-stu-id="04f98-151">Request</span></span>
<span data-ttu-id="04f98-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04f98-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="04f98-153">响应</span><span class="sxs-lookup"><span data-stu-id="04f98-153">Response</span></span>
<span data-ttu-id="04f98-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04f98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```





