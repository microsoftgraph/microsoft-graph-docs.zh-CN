---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79941f498efae8167e6d9abcd9bcdf78b9557677
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199939"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="d4628-103">deviceEnrollmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4628-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="d4628-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4628-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4628-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4628-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4628-106">设备注册配置的基类</span><span class="sxs-lookup"><span data-stu-id="d4628-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="d4628-107">方法</span><span class="sxs-lookup"><span data-stu-id="d4628-107">Methods</span></span>
|<span data-ttu-id="d4628-108">方法</span><span class="sxs-lookup"><span data-stu-id="d4628-108">Method</span></span>|<span data-ttu-id="d4628-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4628-109">Return Type</span></span>|<span data-ttu-id="d4628-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4628-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4628-111">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="d4628-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="d4628-112">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4628-112">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="d4628-113">列出 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4628-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d4628-114">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4628-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="d4628-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4628-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="d4628-116">读取 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4628-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="d4628-117">**载入**</span><span class="sxs-lookup"><span data-stu-id="d4628-117">**Onboarding**</span></span>|
|[<span data-ttu-id="d4628-118">setPriority action</span><span class="sxs-lookup"><span data-stu-id="d4628-118">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="d4628-119">无</span><span class="sxs-lookup"><span data-stu-id="d4628-119">None</span></span>|<span data-ttu-id="d4628-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4628-120">Not yet documented</span></span>|
|[<span data-ttu-id="d4628-121">分配操作</span><span class="sxs-lookup"><span data-stu-id="d4628-121">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="d4628-122">无</span><span class="sxs-lookup"><span data-stu-id="d4628-122">None</span></span>|<span data-ttu-id="d4628-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4628-123">Not yet documented</span></span>|
|<span data-ttu-id="d4628-124">**策略集**</span><span class="sxs-lookup"><span data-stu-id="d4628-124">**Policy Set**</span></span>|
|[<span data-ttu-id="d4628-125">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="d4628-125">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="d4628-126">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="d4628-126">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="d4628-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4628-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d4628-128">属性</span><span class="sxs-lookup"><span data-stu-id="d4628-128">Properties</span></span>
|<span data-ttu-id="d4628-129">属性</span><span class="sxs-lookup"><span data-stu-id="d4628-129">Property</span></span>|<span data-ttu-id="d4628-130">类型</span><span class="sxs-lookup"><span data-stu-id="d4628-130">Type</span></span>|<span data-ttu-id="d4628-131">说明</span><span class="sxs-lookup"><span data-stu-id="d4628-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4628-132">id</span><span class="sxs-lookup"><span data-stu-id="d4628-132">id</span></span>|<span data-ttu-id="d4628-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d4628-133">String</span></span>|<span data-ttu-id="d4628-134">帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d4628-134">Unique Identifier for the account</span></span>|
|<span data-ttu-id="d4628-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d4628-135">displayName</span></span>|<span data-ttu-id="d4628-136">String</span><span class="sxs-lookup"><span data-stu-id="d4628-136">String</span></span>|<span data-ttu-id="d4628-137">设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="d4628-137">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="d4628-138">说明</span><span class="sxs-lookup"><span data-stu-id="d4628-138">description</span></span>|<span data-ttu-id="d4628-139">String</span><span class="sxs-lookup"><span data-stu-id="d4628-139">String</span></span>|<span data-ttu-id="d4628-140">设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="d4628-140">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="d4628-141">priority</span><span class="sxs-lookup"><span data-stu-id="d4628-141">priority</span></span>|<span data-ttu-id="d4628-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d4628-142">Int32</span></span>|<span data-ttu-id="d4628-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="d4628-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d4628-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="d4628-144">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="d4628-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4628-145">createdDateTime</span></span>|<span data-ttu-id="d4628-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4628-146">DateTimeOffset</span></span>|<span data-ttu-id="d4628-147">设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="d4628-147">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="d4628-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4628-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d4628-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4628-149">DateTimeOffset</span></span>|<span data-ttu-id="d4628-150">设备注册配置的上次修改日期时间（UTC）</span><span class="sxs-lookup"><span data-stu-id="d4628-150">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="d4628-151">version</span><span class="sxs-lookup"><span data-stu-id="d4628-151">version</span></span>|<span data-ttu-id="d4628-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d4628-152">Int32</span></span>|<span data-ttu-id="d4628-153">设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="d4628-153">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4628-154">关系</span><span class="sxs-lookup"><span data-stu-id="d4628-154">Relationships</span></span>
|<span data-ttu-id="d4628-155">关系</span><span class="sxs-lookup"><span data-stu-id="d4628-155">Relationship</span></span>|<span data-ttu-id="d4628-156">类型</span><span class="sxs-lookup"><span data-stu-id="d4628-156">Type</span></span>|<span data-ttu-id="d4628-157">说明</span><span class="sxs-lookup"><span data-stu-id="d4628-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4628-158">**载入**</span><span class="sxs-lookup"><span data-stu-id="d4628-158">**Onboarding**</span></span>|
|<span data-ttu-id="d4628-159">assignments</span><span class="sxs-lookup"><span data-stu-id="d4628-159">assignments</span></span>|<span data-ttu-id="d4628-160">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4628-160">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d4628-161">设备配置文件的组分配列表</span><span class="sxs-lookup"><span data-stu-id="d4628-161">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4628-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4628-162">JSON Representation</span></span>
<span data-ttu-id="d4628-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4628-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```



