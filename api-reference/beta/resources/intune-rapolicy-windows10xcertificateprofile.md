---
title: windows10XCertificateProfile 资源类型
description: " (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 840b898599ec6fc97e6d1c6eba2d1f94cd84329f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301494"
---
# <a name="windows10xcertificateprofile-resource-type"></a><span data-ttu-id="bac64-103">windows10XCertificateProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="bac64-103">windows10XCertificateProfile resource type</span></span>

<span data-ttu-id="bac64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bac64-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bac64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bac64-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bac64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac64-107"> (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型</span><span class="sxs-lookup"><span data-stu-id="bac64-107">Base Profile Type for Authentication Certificates (SCEP or PFX Create)</span></span>


<span data-ttu-id="bac64-108">继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bac64-108">Inherits from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bac64-109">方法</span><span class="sxs-lookup"><span data-stu-id="bac64-109">Methods</span></span>
|<span data-ttu-id="bac64-110">方法</span><span class="sxs-lookup"><span data-stu-id="bac64-110">Method</span></span>|<span data-ttu-id="bac64-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="bac64-111">Return Type</span></span>|<span data-ttu-id="bac64-112">说明</span><span class="sxs-lookup"><span data-stu-id="bac64-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bac64-113">列出 windows10XCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="bac64-113">List windows10XCertificateProfiles</span></span>](../api/intune-rapolicy-windows10xcertificateprofile-list.md)|<span data-ttu-id="bac64-114">[windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bac64-114">[windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) collection</span></span>|<span data-ttu-id="bac64-115">列出 [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bac64-115">List properties and relationships of the [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) objects.</span></span>|
|[<span data-ttu-id="bac64-116">获取 windows10XCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="bac64-116">Get windows10XCertificateProfile</span></span>](../api/intune-rapolicy-windows10xcertificateprofile-get.md)|[<span data-ttu-id="bac64-117">windows10XCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="bac64-117">windows10XCertificateProfile</span></span>](../resources/intune-rapolicy-windows10xcertificateprofile.md)|<span data-ttu-id="bac64-118">读取 [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bac64-118">Read properties and relationships of the [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bac64-119">属性</span><span class="sxs-lookup"><span data-stu-id="bac64-119">Properties</span></span>
|<span data-ttu-id="bac64-120">属性</span><span class="sxs-lookup"><span data-stu-id="bac64-120">Property</span></span>|<span data-ttu-id="bac64-121">类型</span><span class="sxs-lookup"><span data-stu-id="bac64-121">Type</span></span>|<span data-ttu-id="bac64-122">说明</span><span class="sxs-lookup"><span data-stu-id="bac64-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac64-123">id</span><span class="sxs-lookup"><span data-stu-id="bac64-123">id</span></span>|<span data-ttu-id="bac64-124">String</span><span class="sxs-lookup"><span data-stu-id="bac64-124">String</span></span>|<span data-ttu-id="bac64-125">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件标识符</span><span class="sxs-lookup"><span data-stu-id="bac64-125">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="bac64-126">version</span><span class="sxs-lookup"><span data-stu-id="bac64-126">version</span></span>|<span data-ttu-id="bac64-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bac64-127">Int32</span></span>|<span data-ttu-id="bac64-128">继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的配置文件的版本</span><span class="sxs-lookup"><span data-stu-id="bac64-128">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="bac64-129">displayName</span><span class="sxs-lookup"><span data-stu-id="bac64-129">displayName</span></span>|<span data-ttu-id="bac64-130">String</span><span class="sxs-lookup"><span data-stu-id="bac64-130">String</span></span>|<span data-ttu-id="bac64-131">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件显示名称</span><span class="sxs-lookup"><span data-stu-id="bac64-131">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="bac64-132">description</span><span class="sxs-lookup"><span data-stu-id="bac64-132">description</span></span>|<span data-ttu-id="bac64-133">String</span><span class="sxs-lookup"><span data-stu-id="bac64-133">String</span></span>|<span data-ttu-id="bac64-134">从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件说明</span><span class="sxs-lookup"><span data-stu-id="bac64-134">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="bac64-135">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="bac64-135">creationDateTime</span></span>|<span data-ttu-id="bac64-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac64-136">DateTimeOffset</span></span>|<span data-ttu-id="bac64-137">已创建从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的 DateTime 配置文件</span><span class="sxs-lookup"><span data-stu-id="bac64-137">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="bac64-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bac64-138">lastModifiedDateTime</span></span>|<span data-ttu-id="bac64-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac64-139">DateTimeOffset</span></span>|<span data-ttu-id="bac64-140">上次修改的日期时间配置文件继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bac64-140">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="bac64-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bac64-141">roleScopeTagIds</span></span>|<span data-ttu-id="bac64-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="bac64-142">String collection</span></span>|<span data-ttu-id="bac64-143">继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的范围标记</span><span class="sxs-lookup"><span data-stu-id="bac64-143">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bac64-144">关系</span><span class="sxs-lookup"><span data-stu-id="bac64-144">Relationships</span></span>
|<span data-ttu-id="bac64-145">关系</span><span class="sxs-lookup"><span data-stu-id="bac64-145">Relationship</span></span>|<span data-ttu-id="bac64-146">类型</span><span class="sxs-lookup"><span data-stu-id="bac64-146">Type</span></span>|<span data-ttu-id="bac64-147">描述</span><span class="sxs-lookup"><span data-stu-id="bac64-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac64-148">assignments</span><span class="sxs-lookup"><span data-stu-id="bac64-148">assignments</span></span>|<span data-ttu-id="bac64-149">[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bac64-149">[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection</span></span>|<span data-ttu-id="bac64-150">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="bac64-150">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="bac64-151">继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bac64-151">Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bac64-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bac64-152">JSON Representation</span></span>
<span data-ttu-id="bac64-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bac64-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCertificateProfile",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




