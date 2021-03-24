---
title: 创建 windows10XVpnConfiguration
description: 创建新的 windows10XVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f80bb41a3098931af7b10521dce9b803911a474a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145059"
---
# <a name="create-windows10xvpnconfiguration"></a><span data-ttu-id="9c7cc-103">创建 windows10XVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c7cc-103">Create windows10XVpnConfiguration</span></span>

<span data-ttu-id="9c7cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c7cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c7cc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c7cc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c7cc-107">创建新的 [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-107">Create a new [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c7cc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c7cc-108">Prerequisites</span></span>
<span data-ttu-id="9c7cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c7cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c7cc-111">Permission type</span></span>|<span data-ttu-id="9c7cc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c7cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c7cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c7cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c7cc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c7cc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9c7cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c7cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c7cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-116">Not supported.</span></span>|
|<span data-ttu-id="9c7cc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c7cc-117">Application</span></span>|<span data-ttu-id="9c7cc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c7cc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c7cc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c7cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9c7cc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c7cc-120">Request headers</span></span>
|<span data-ttu-id="9c7cc-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c7cc-121">Header</span></span>|<span data-ttu-id="9c7cc-122">值</span><span class="sxs-lookup"><span data-stu-id="9c7cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c7cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c7cc-123">Authorization</span></span>|<span data-ttu-id="9c7cc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c7cc-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c7cc-125">Accept</span></span>|<span data-ttu-id="9c7cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c7cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c7cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c7cc-127">Request body</span></span>
<span data-ttu-id="9c7cc-128">在请求正文中，提供 windows10XVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-128">In the request body, supply a JSON representation for the windows10XVpnConfiguration object.</span></span>

<span data-ttu-id="9c7cc-129">下表显示创建 windows10XVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-129">The following table shows the properties that are required when you create the windows10XVpnConfiguration.</span></span>

|<span data-ttu-id="9c7cc-130">属性</span><span class="sxs-lookup"><span data-stu-id="9c7cc-130">Property</span></span>|<span data-ttu-id="9c7cc-131">类型</span><span class="sxs-lookup"><span data-stu-id="9c7cc-131">Type</span></span>|<span data-ttu-id="9c7cc-132">说明</span><span class="sxs-lookup"><span data-stu-id="9c7cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c7cc-133">id</span><span class="sxs-lookup"><span data-stu-id="9c7cc-133">id</span></span>|<span data-ttu-id="9c7cc-134">String</span><span class="sxs-lookup"><span data-stu-id="9c7cc-134">String</span></span>|<span data-ttu-id="9c7cc-135">配置文件标识符 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c7cc-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9c7cc-136">version</span><span class="sxs-lookup"><span data-stu-id="9c7cc-136">version</span></span>|<span data-ttu-id="9c7cc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9c7cc-137">Int32</span></span>|<span data-ttu-id="9c7cc-138">配置文件的版本 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c7cc-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9c7cc-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9c7cc-139">displayName</span></span>|<span data-ttu-id="9c7cc-140">String</span><span class="sxs-lookup"><span data-stu-id="9c7cc-140">String</span></span>|<span data-ttu-id="9c7cc-141">配置文件显示名称继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c7cc-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9c7cc-142">说明</span><span class="sxs-lookup"><span data-stu-id="9c7cc-142">description</span></span>|<span data-ttu-id="9c7cc-143">String</span><span class="sxs-lookup"><span data-stu-id="9c7cc-143">String</span></span>|<span data-ttu-id="9c7cc-144">配置文件说明 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c7cc-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9c7cc-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="9c7cc-145">creationDateTime</span></span>|<span data-ttu-id="9c7cc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c7cc-146">DateTimeOffset</span></span>|<span data-ttu-id="9c7cc-147">DateTime 配置文件已创建 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c7cc-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9c7cc-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c7cc-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9c7cc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c7cc-149">DateTimeOffset</span></span>|<span data-ttu-id="9c7cc-150">DateTime 配置文件上次修改时间 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c7cc-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9c7cc-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c7cc-151">roleScopeTagIds</span></span>|<span data-ttu-id="9c7cc-152">String collection</span><span class="sxs-lookup"><span data-stu-id="9c7cc-152">String collection</span></span>|<span data-ttu-id="9c7cc-153">范围标记 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c7cc-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9c7cc-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="9c7cc-154">authenticationCertificateId</span></span>|<span data-ttu-id="9c7cc-155">Guid</span><span class="sxs-lookup"><span data-stu-id="9c7cc-155">Guid</span></span>|<span data-ttu-id="9c7cc-156">身份验证证书的 ID</span><span class="sxs-lookup"><span data-stu-id="9c7cc-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="9c7cc-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="9c7cc-157">customXmlFileName</span></span>|<span data-ttu-id="9c7cc-158">String</span><span class="sxs-lookup"><span data-stu-id="9c7cc-158">String</span></span>|<span data-ttu-id="9c7cc-159">自定义 Xml 文件名。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="9c7cc-160">customXml</span><span class="sxs-lookup"><span data-stu-id="9c7cc-160">customXml</span></span>|<span data-ttu-id="9c7cc-161">Binary</span><span class="sxs-lookup"><span data-stu-id="9c7cc-161">Binary</span></span>|<span data-ttu-id="9c7cc-162">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="9c7cc-163"> (UTF8 字节编码) </span><span class="sxs-lookup"><span data-stu-id="9c7cc-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="9c7cc-164">响应</span><span class="sxs-lookup"><span data-stu-id="9c7cc-164">Response</span></span>
<span data-ttu-id="9c7cc-165">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-165">If successful, this method returns a `201 Created` response code and a [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c7cc-166">示例</span><span class="sxs-lookup"><span data-stu-id="9c7cc-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c7cc-167">请求</span><span class="sxs-lookup"><span data-stu-id="9c7cc-167">Request</span></span>
<span data-ttu-id="9c7cc-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 446

{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
  "customXmlFileName": "Custom Xml File Name value",
  "customXml": "Y3VzdG9tWG1s"
}
```

### <a name="response"></a><span data-ttu-id="9c7cc-169">响应</span><span class="sxs-lookup"><span data-stu-id="9c7cc-169">Response</span></span>
<span data-ttu-id="9c7cc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c7cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 559

{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
  "id": "6ee1c04f-c04f-6ee1-4fc0-e16e4fc0e16e",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
  "customXmlFileName": "Custom Xml File Name value",
  "customXml": "Y3VzdG9tWG1s"
}
```




