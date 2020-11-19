---
title: 创建 windows10XWifiConfiguration
description: 创建新的 windows10XWifiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0ea55ddb4c2992758f42a0eb479ae8e04403114
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241516"
---
# <a name="create-windows10xwificonfiguration"></a><span data-ttu-id="2370c-103">创建 windows10XWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="2370c-103">Create windows10XWifiConfiguration</span></span>

<span data-ttu-id="2370c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2370c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2370c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2370c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2370c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2370c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2370c-107">创建新的 [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2370c-107">Create a new [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2370c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2370c-108">Prerequisites</span></span>
<span data-ttu-id="2370c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2370c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2370c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2370c-111">Permission type</span></span>|<span data-ttu-id="2370c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2370c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2370c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2370c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2370c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2370c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2370c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2370c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2370c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2370c-116">Not supported.</span></span>|
|<span data-ttu-id="2370c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2370c-117">Application</span></span>|<span data-ttu-id="2370c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2370c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2370c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2370c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2370c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2370c-120">Request headers</span></span>
|<span data-ttu-id="2370c-121">标头</span><span class="sxs-lookup"><span data-stu-id="2370c-121">Header</span></span>|<span data-ttu-id="2370c-122">值</span><span class="sxs-lookup"><span data-stu-id="2370c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2370c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2370c-123">Authorization</span></span>|<span data-ttu-id="2370c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2370c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2370c-125">接受</span><span class="sxs-lookup"><span data-stu-id="2370c-125">Accept</span></span>|<span data-ttu-id="2370c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2370c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2370c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2370c-127">Request body</span></span>
<span data-ttu-id="2370c-128">在请求正文中，提供 windows10XWifiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2370c-128">In the request body, supply a JSON representation for the windows10XWifiConfiguration object.</span></span>

<span data-ttu-id="2370c-129">下表显示创建 windows10XWifiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2370c-129">The following table shows the properties that are required when you create the windows10XWifiConfiguration.</span></span>

|<span data-ttu-id="2370c-130">属性</span><span class="sxs-lookup"><span data-stu-id="2370c-130">Property</span></span>|<span data-ttu-id="2370c-131">类型</span><span class="sxs-lookup"><span data-stu-id="2370c-131">Type</span></span>|<span data-ttu-id="2370c-132">说明</span><span class="sxs-lookup"><span data-stu-id="2370c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2370c-133">id</span><span class="sxs-lookup"><span data-stu-id="2370c-133">id</span></span>|<span data-ttu-id="2370c-134">String</span><span class="sxs-lookup"><span data-stu-id="2370c-134">String</span></span>|<span data-ttu-id="2370c-135">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件标识符</span><span class="sxs-lookup"><span data-stu-id="2370c-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="2370c-136">version</span><span class="sxs-lookup"><span data-stu-id="2370c-136">version</span></span>|<span data-ttu-id="2370c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2370c-137">Int32</span></span>|<span data-ttu-id="2370c-138">继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的配置文件的版本</span><span class="sxs-lookup"><span data-stu-id="2370c-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="2370c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2370c-139">displayName</span></span>|<span data-ttu-id="2370c-140">String</span><span class="sxs-lookup"><span data-stu-id="2370c-140">String</span></span>|<span data-ttu-id="2370c-141">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件显示名称</span><span class="sxs-lookup"><span data-stu-id="2370c-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="2370c-142">description</span><span class="sxs-lookup"><span data-stu-id="2370c-142">description</span></span>|<span data-ttu-id="2370c-143">String</span><span class="sxs-lookup"><span data-stu-id="2370c-143">String</span></span>|<span data-ttu-id="2370c-144">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件说明</span><span class="sxs-lookup"><span data-stu-id="2370c-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="2370c-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="2370c-145">creationDateTime</span></span>|<span data-ttu-id="2370c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2370c-146">DateTimeOffset</span></span>|<span data-ttu-id="2370c-147">已创建从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的 DateTime 配置文件</span><span class="sxs-lookup"><span data-stu-id="2370c-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="2370c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2370c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="2370c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2370c-149">DateTimeOffset</span></span>|<span data-ttu-id="2370c-150">上次修改的日期时间配置文件继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2370c-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="2370c-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2370c-151">roleScopeTagIds</span></span>|<span data-ttu-id="2370c-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="2370c-152">String collection</span></span>|<span data-ttu-id="2370c-153">继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的范围标记</span><span class="sxs-lookup"><span data-stu-id="2370c-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="2370c-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="2370c-154">authenticationCertificateId</span></span>|<span data-ttu-id="2370c-155">Guid</span><span class="sxs-lookup"><span data-stu-id="2370c-155">Guid</span></span>|<span data-ttu-id="2370c-156">身份验证证书的 ID</span><span class="sxs-lookup"><span data-stu-id="2370c-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="2370c-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="2370c-157">customXmlFileName</span></span>|<span data-ttu-id="2370c-158">String</span><span class="sxs-lookup"><span data-stu-id="2370c-158">String</span></span>|<span data-ttu-id="2370c-159">自定义 Xml 文件名。</span><span class="sxs-lookup"><span data-stu-id="2370c-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="2370c-160">customXml</span><span class="sxs-lookup"><span data-stu-id="2370c-160">customXml</span></span>|<span data-ttu-id="2370c-161">Binary</span><span class="sxs-lookup"><span data-stu-id="2370c-161">Binary</span></span>|<span data-ttu-id="2370c-162">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="2370c-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="2370c-163"> (UTF8 字节编码) </span><span class="sxs-lookup"><span data-stu-id="2370c-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="2370c-164">响应</span><span class="sxs-lookup"><span data-stu-id="2370c-164">Response</span></span>
<span data-ttu-id="2370c-165">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2370c-165">If successful, this method returns a `201 Created` response code and a [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2370c-166">示例</span><span class="sxs-lookup"><span data-stu-id="2370c-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="2370c-167">请求</span><span class="sxs-lookup"><span data-stu-id="2370c-167">Request</span></span>
<span data-ttu-id="2370c-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2370c-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
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

### <a name="response"></a><span data-ttu-id="2370c-169">响应</span><span class="sxs-lookup"><span data-stu-id="2370c-169">Response</span></span>
<span data-ttu-id="2370c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2370c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
  "id": "31063b86-3b86-3106-863b-0631863b0631",
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




