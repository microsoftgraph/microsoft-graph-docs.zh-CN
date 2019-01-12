---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c28ff97747f6132edbd89951c4fdfd6aa13941a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919251"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="7de29-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="7de29-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="7de29-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7de29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7de29-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7de29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7de29-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7de29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7de29-107">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7de29-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7de29-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7de29-108">Prerequisites</span></span>
<span data-ttu-id="7de29-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7de29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7de29-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7de29-111">Permission type</span></span>|<span data-ttu-id="7de29-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7de29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7de29-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7de29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7de29-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7de29-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7de29-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7de29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7de29-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7de29-116">Not supported.</span></span>|
|<span data-ttu-id="7de29-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7de29-117">Application</span></span>|<span data-ttu-id="7de29-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7de29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7de29-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7de29-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7de29-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7de29-120">Request headers</span></span>
|<span data-ttu-id="7de29-121">标头</span><span class="sxs-lookup"><span data-stu-id="7de29-121">Header</span></span>|<span data-ttu-id="7de29-122">值</span><span class="sxs-lookup"><span data-stu-id="7de29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7de29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7de29-123">Authorization</span></span>|<span data-ttu-id="7de29-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7de29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7de29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7de29-125">Accept</span></span>|<span data-ttu-id="7de29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7de29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7de29-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7de29-127">Request body</span></span>
<span data-ttu-id="7de29-128">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7de29-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="7de29-129">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7de29-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="7de29-130">属性</span><span class="sxs-lookup"><span data-stu-id="7de29-130">Property</span></span>|<span data-ttu-id="7de29-131">类型</span><span class="sxs-lookup"><span data-stu-id="7de29-131">Type</span></span>|<span data-ttu-id="7de29-132">说明</span><span class="sxs-lookup"><span data-stu-id="7de29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7de29-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7de29-133">displayName</span></span>|<span data-ttu-id="7de29-134">String</span><span class="sxs-lookup"><span data-stu-id="7de29-134">String</span></span>|<span data-ttu-id="7de29-135">友好名称</span><span class="sxs-lookup"><span data-stu-id="7de29-135">The friendly name</span></span>|
|<span data-ttu-id="7de29-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="7de29-136">fileHash</span></span>|<span data-ttu-id="7de29-137">String</span><span class="sxs-lookup"><span data-stu-id="7de29-137">String</span></span>|<span data-ttu-id="7de29-138">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="7de29-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="7de29-139">file</span><span class="sxs-lookup"><span data-stu-id="7de29-139">file</span></span>|<span data-ttu-id="7de29-140">Binary</span><span class="sxs-lookup"><span data-stu-id="7de29-140">Binary</span></span>|<span data-ttu-id="7de29-141">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="7de29-141">File as a byte array</span></span>|
|<span data-ttu-id="7de29-142">id</span><span class="sxs-lookup"><span data-stu-id="7de29-142">id</span></span>|<span data-ttu-id="7de29-143">String</span><span class="sxs-lookup"><span data-stu-id="7de29-143">String</span></span>|<span data-ttu-id="7de29-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7de29-144">Key of the entity.</span></span>|
|<span data-ttu-id="7de29-145">version</span><span class="sxs-lookup"><span data-stu-id="7de29-145">version</span></span>|<span data-ttu-id="7de29-146">String</span><span class="sxs-lookup"><span data-stu-id="7de29-146">String</span></span>|<span data-ttu-id="7de29-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="7de29-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="7de29-148">响应</span><span class="sxs-lookup"><span data-stu-id="7de29-148">Response</span></span>
<span data-ttu-id="7de29-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7de29-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7de29-150">示例</span><span class="sxs-lookup"><span data-stu-id="7de29-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="7de29-151">请求</span><span class="sxs-lookup"><span data-stu-id="7de29-151">Request</span></span>
<span data-ttu-id="7de29-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7de29-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7de29-153">响应</span><span class="sxs-lookup"><span data-stu-id="7de29-153">Response</span></span>
<span data-ttu-id="7de29-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7de29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





