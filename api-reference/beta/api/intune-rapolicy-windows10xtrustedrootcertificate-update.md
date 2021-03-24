---
title: 更新 windows10XTrustedRootCertificate
description: 更新 windows10XTrustedRootCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c8ba77096df428f7c5c99429c2b6bdeebac3e26
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145066"
---
# <a name="update-windows10xtrustedrootcertificate"></a><span data-ttu-id="03951-103">更新 windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="03951-103">Update windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="03951-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03951-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03951-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03951-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03951-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03951-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03951-107">更新 [windows10XTrustedRootCertificate 对象](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="03951-107">Update the properties of a [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03951-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03951-108">Prerequisites</span></span>
<span data-ttu-id="03951-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03951-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03951-111">Permission type</span></span>|<span data-ttu-id="03951-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03951-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03951-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03951-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03951-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03951-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="03951-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03951-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03951-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03951-116">Not supported.</span></span>|
|<span data-ttu-id="03951-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03951-117">Application</span></span>|<span data-ttu-id="03951-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03951-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03951-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03951-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="03951-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03951-120">Request headers</span></span>
|<span data-ttu-id="03951-121">标头</span><span class="sxs-lookup"><span data-stu-id="03951-121">Header</span></span>|<span data-ttu-id="03951-122">值</span><span class="sxs-lookup"><span data-stu-id="03951-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03951-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03951-123">Authorization</span></span>|<span data-ttu-id="03951-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03951-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03951-125">接受</span><span class="sxs-lookup"><span data-stu-id="03951-125">Accept</span></span>|<span data-ttu-id="03951-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03951-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03951-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03951-127">Request body</span></span>
<span data-ttu-id="03951-128">在请求正文中，提供 [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03951-128">In the request body, supply a JSON representation for the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="03951-129">下表显示创建 [windows10XTrustedRootCertificate 时所需的属性](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="03951-129">The following table shows the properties that are required when you create the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span></span>

|<span data-ttu-id="03951-130">属性</span><span class="sxs-lookup"><span data-stu-id="03951-130">Property</span></span>|<span data-ttu-id="03951-131">类型</span><span class="sxs-lookup"><span data-stu-id="03951-131">Type</span></span>|<span data-ttu-id="03951-132">说明</span><span class="sxs-lookup"><span data-stu-id="03951-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03951-133">id</span><span class="sxs-lookup"><span data-stu-id="03951-133">id</span></span>|<span data-ttu-id="03951-134">String</span><span class="sxs-lookup"><span data-stu-id="03951-134">String</span></span>|<span data-ttu-id="03951-135">配置文件标识符 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03951-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="03951-136">version</span><span class="sxs-lookup"><span data-stu-id="03951-136">version</span></span>|<span data-ttu-id="03951-137">Int32</span><span class="sxs-lookup"><span data-stu-id="03951-137">Int32</span></span>|<span data-ttu-id="03951-138">配置文件的版本 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03951-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="03951-139">displayName</span><span class="sxs-lookup"><span data-stu-id="03951-139">displayName</span></span>|<span data-ttu-id="03951-140">String</span><span class="sxs-lookup"><span data-stu-id="03951-140">String</span></span>|<span data-ttu-id="03951-141">配置文件显示名称继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03951-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="03951-142">说明</span><span class="sxs-lookup"><span data-stu-id="03951-142">description</span></span>|<span data-ttu-id="03951-143">String</span><span class="sxs-lookup"><span data-stu-id="03951-143">String</span></span>|<span data-ttu-id="03951-144">配置文件说明 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03951-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="03951-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="03951-145">creationDateTime</span></span>|<span data-ttu-id="03951-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03951-146">DateTimeOffset</span></span>|<span data-ttu-id="03951-147">DateTime 配置文件已创建 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03951-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="03951-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03951-148">lastModifiedDateTime</span></span>|<span data-ttu-id="03951-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03951-149">DateTimeOffset</span></span>|<span data-ttu-id="03951-150">DateTime 配置文件上次修改时间 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03951-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="03951-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03951-151">roleScopeTagIds</span></span>|<span data-ttu-id="03951-152">String collection</span><span class="sxs-lookup"><span data-stu-id="03951-152">String collection</span></span>|<span data-ttu-id="03951-153">范围标记 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03951-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="03951-154">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="03951-154">trustedRootCertificate</span></span>|<span data-ttu-id="03951-155">Binary</span><span class="sxs-lookup"><span data-stu-id="03951-155">Binary</span></span>|<span data-ttu-id="03951-156">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="03951-156">Trusted Root Certificate</span></span>|
|<span data-ttu-id="03951-157">certFileName</span><span class="sxs-lookup"><span data-stu-id="03951-157">certFileName</span></span>|<span data-ttu-id="03951-158">String</span><span class="sxs-lookup"><span data-stu-id="03951-158">String</span></span>|<span data-ttu-id="03951-159">要显示在 UI 中的文件名。</span><span class="sxs-lookup"><span data-stu-id="03951-159">File name to display in UI.</span></span>|
|<span data-ttu-id="03951-160">destinationStore</span><span class="sxs-lookup"><span data-stu-id="03951-160">destinationStore</span></span>|[<span data-ttu-id="03951-161">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="03951-161">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="03951-162">受信任根证书的目标存储位置。</span><span class="sxs-lookup"><span data-stu-id="03951-162">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="03951-163">可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。</span><span class="sxs-lookup"><span data-stu-id="03951-163">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="03951-164">响应</span><span class="sxs-lookup"><span data-stu-id="03951-164">Response</span></span>
<span data-ttu-id="03951-165">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03951-165">If successful, this method returns a `200 OK` response code and an updated [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03951-166">示例</span><span class="sxs-lookup"><span data-stu-id="03951-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="03951-167">请求</span><span class="sxs-lookup"><span data-stu-id="03951-167">Request</span></span>
<span data-ttu-id="03951-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03951-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03951-169">响应</span><span class="sxs-lookup"><span data-stu-id="03951-169">Response</span></span>
<span data-ttu-id="03951-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03951-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




