---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
author: tfitzmac
ms.openlocfilehash: f2cbed922d6f2ac130169e5d9c85e3a5231184a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317120"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="66737-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="66737-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="66737-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="66737-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66737-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="66737-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66737-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="66737-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66737-107">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66737-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66737-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="66737-108">Prerequisites</span></span>
<span data-ttu-id="66737-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="66737-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66737-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="66737-111">Permission type</span></span>|<span data-ttu-id="66737-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66737-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66737-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66737-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66737-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66737-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66737-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66737-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66737-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="66737-116">Not supported.</span></span>|
|<span data-ttu-id="66737-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="66737-117">Application</span></span>|<span data-ttu-id="66737-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="66737-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66737-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66737-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="66737-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66737-120">Request headers</span></span>
|<span data-ttu-id="66737-121">标头</span><span class="sxs-lookup"><span data-stu-id="66737-121">Header</span></span>|<span data-ttu-id="66737-122">值</span><span class="sxs-lookup"><span data-stu-id="66737-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66737-123">授权</span><span class="sxs-lookup"><span data-stu-id="66737-123">Authorization</span></span>|<span data-ttu-id="66737-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66737-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66737-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66737-125">Accept</span></span>|<span data-ttu-id="66737-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66737-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66737-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="66737-127">Request body</span></span>
<span data-ttu-id="66737-128">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66737-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="66737-129">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66737-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="66737-130">属性</span><span class="sxs-lookup"><span data-stu-id="66737-130">Property</span></span>|<span data-ttu-id="66737-131">类型</span><span class="sxs-lookup"><span data-stu-id="66737-131">Type</span></span>|<span data-ttu-id="66737-132">说明</span><span class="sxs-lookup"><span data-stu-id="66737-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66737-133">displayName</span><span class="sxs-lookup"><span data-stu-id="66737-133">displayName</span></span>|<span data-ttu-id="66737-134">String</span><span class="sxs-lookup"><span data-stu-id="66737-134">String</span></span>|<span data-ttu-id="66737-135">友好名称</span><span class="sxs-lookup"><span data-stu-id="66737-135">The friendly name</span></span>|
|<span data-ttu-id="66737-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="66737-136">fileHash</span></span>|<span data-ttu-id="66737-137">String</span><span class="sxs-lookup"><span data-stu-id="66737-137">String</span></span>|<span data-ttu-id="66737-138">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="66737-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="66737-139">file</span><span class="sxs-lookup"><span data-stu-id="66737-139">file</span></span>|<span data-ttu-id="66737-140">Binary</span><span class="sxs-lookup"><span data-stu-id="66737-140">Binary</span></span>|<span data-ttu-id="66737-141">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="66737-141">File as a byte array</span></span>|
|<span data-ttu-id="66737-142">id</span><span class="sxs-lookup"><span data-stu-id="66737-142">id</span></span>|<span data-ttu-id="66737-143">String</span><span class="sxs-lookup"><span data-stu-id="66737-143">String</span></span>|<span data-ttu-id="66737-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66737-144">Key of the entity.</span></span>|
|<span data-ttu-id="66737-145">version</span><span class="sxs-lookup"><span data-stu-id="66737-145">version</span></span>|<span data-ttu-id="66737-146">String</span><span class="sxs-lookup"><span data-stu-id="66737-146">String</span></span>|<span data-ttu-id="66737-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="66737-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="66737-148">响应</span><span class="sxs-lookup"><span data-stu-id="66737-148">Response</span></span>
<span data-ttu-id="66737-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66737-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66737-150">示例</span><span class="sxs-lookup"><span data-stu-id="66737-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="66737-151">请求</span><span class="sxs-lookup"><span data-stu-id="66737-151">Request</span></span>
<span data-ttu-id="66737-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66737-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66737-153">响应</span><span class="sxs-lookup"><span data-stu-id="66737-153">Response</span></span>
<span data-ttu-id="66737-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66737-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





