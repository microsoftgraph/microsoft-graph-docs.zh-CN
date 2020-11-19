---
title: 更新 windows10XTrustedRootCertificate
description: 更新 windows10XTrustedRootCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ea11d39cd1a5a29a52dca8ef9d1e043c634fed2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241550"
---
# <a name="update-windows10xtrustedrootcertificate"></a><span data-ttu-id="6b52e-103">更新 windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="6b52e-103">Update windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="6b52e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b52e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b52e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b52e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b52e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b52e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b52e-107">更新 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6b52e-107">Update the properties of a [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b52e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b52e-108">Prerequisites</span></span>
<span data-ttu-id="6b52e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b52e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b52e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b52e-111">Permission type</span></span>|<span data-ttu-id="6b52e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b52e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b52e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b52e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b52e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b52e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6b52e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b52e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b52e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b52e-116">Not supported.</span></span>|
|<span data-ttu-id="6b52e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b52e-117">Application</span></span>|<span data-ttu-id="6b52e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b52e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b52e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b52e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="6b52e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b52e-120">Request headers</span></span>
|<span data-ttu-id="6b52e-121">标头</span><span class="sxs-lookup"><span data-stu-id="6b52e-121">Header</span></span>|<span data-ttu-id="6b52e-122">值</span><span class="sxs-lookup"><span data-stu-id="6b52e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b52e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b52e-123">Authorization</span></span>|<span data-ttu-id="6b52e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b52e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b52e-125">接受</span><span class="sxs-lookup"><span data-stu-id="6b52e-125">Accept</span></span>|<span data-ttu-id="6b52e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b52e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b52e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b52e-127">Request body</span></span>
<span data-ttu-id="6b52e-128">在请求正文中，提供 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b52e-128">In the request body, supply a JSON representation for the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="6b52e-129">下表显示创建 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6b52e-129">The following table shows the properties that are required when you create the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span></span>

|<span data-ttu-id="6b52e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6b52e-130">Property</span></span>|<span data-ttu-id="6b52e-131">类型</span><span class="sxs-lookup"><span data-stu-id="6b52e-131">Type</span></span>|<span data-ttu-id="6b52e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6b52e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b52e-133">id</span><span class="sxs-lookup"><span data-stu-id="6b52e-133">id</span></span>|<span data-ttu-id="6b52e-134">String</span><span class="sxs-lookup"><span data-stu-id="6b52e-134">String</span></span>|<span data-ttu-id="6b52e-135">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件标识符</span><span class="sxs-lookup"><span data-stu-id="6b52e-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6b52e-136">version</span><span class="sxs-lookup"><span data-stu-id="6b52e-136">version</span></span>|<span data-ttu-id="6b52e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6b52e-137">Int32</span></span>|<span data-ttu-id="6b52e-138">继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的配置文件的版本</span><span class="sxs-lookup"><span data-stu-id="6b52e-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6b52e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6b52e-139">displayName</span></span>|<span data-ttu-id="6b52e-140">String</span><span class="sxs-lookup"><span data-stu-id="6b52e-140">String</span></span>|<span data-ttu-id="6b52e-141">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件显示名称</span><span class="sxs-lookup"><span data-stu-id="6b52e-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6b52e-142">description</span><span class="sxs-lookup"><span data-stu-id="6b52e-142">description</span></span>|<span data-ttu-id="6b52e-143">String</span><span class="sxs-lookup"><span data-stu-id="6b52e-143">String</span></span>|<span data-ttu-id="6b52e-144">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件说明</span><span class="sxs-lookup"><span data-stu-id="6b52e-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6b52e-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="6b52e-145">creationDateTime</span></span>|<span data-ttu-id="6b52e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b52e-146">DateTimeOffset</span></span>|<span data-ttu-id="6b52e-147">已创建从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的 DateTime 配置文件</span><span class="sxs-lookup"><span data-stu-id="6b52e-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6b52e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b52e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6b52e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b52e-149">DateTimeOffset</span></span>|<span data-ttu-id="6b52e-150">上次修改的日期时间配置文件继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6b52e-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6b52e-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b52e-151">roleScopeTagIds</span></span>|<span data-ttu-id="6b52e-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="6b52e-152">String collection</span></span>|<span data-ttu-id="6b52e-153">继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的范围标记</span><span class="sxs-lookup"><span data-stu-id="6b52e-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6b52e-154">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="6b52e-154">trustedRootCertificate</span></span>|<span data-ttu-id="6b52e-155">Binary</span><span class="sxs-lookup"><span data-stu-id="6b52e-155">Binary</span></span>|<span data-ttu-id="6b52e-156">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="6b52e-156">Trusted Root Certificate</span></span>|
|<span data-ttu-id="6b52e-157">certFileName</span><span class="sxs-lookup"><span data-stu-id="6b52e-157">certFileName</span></span>|<span data-ttu-id="6b52e-158">String</span><span class="sxs-lookup"><span data-stu-id="6b52e-158">String</span></span>|<span data-ttu-id="6b52e-159">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="6b52e-159">File name to display in UI.</span></span>|
|<span data-ttu-id="6b52e-160">destinationStore</span><span class="sxs-lookup"><span data-stu-id="6b52e-160">destinationStore</span></span>|[<span data-ttu-id="6b52e-161">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="6b52e-161">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="6b52e-162">受信任的根证书的目标存储位置。</span><span class="sxs-lookup"><span data-stu-id="6b52e-162">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="6b52e-163">可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。</span><span class="sxs-lookup"><span data-stu-id="6b52e-163">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="6b52e-164">响应</span><span class="sxs-lookup"><span data-stu-id="6b52e-164">Response</span></span>
<span data-ttu-id="6b52e-165">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b52e-165">If successful, this method returns a `200 OK` response code and an updated [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b52e-166">示例</span><span class="sxs-lookup"><span data-stu-id="6b52e-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b52e-167">请求</span><span class="sxs-lookup"><span data-stu-id="6b52e-167">Request</span></span>
<span data-ttu-id="6b52e-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b52e-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
Content-type: application/json
Content-length: 456

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="6b52e-169">响应</span><span class="sxs-lookup"><span data-stu-id="6b52e-169">Response</span></span>
<span data-ttu-id="6b52e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b52e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "be0bfd01-fd01-be0b-01fd-0bbe01fd0bbe",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




