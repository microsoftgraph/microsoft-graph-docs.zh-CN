---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad0543a521d66ed6e515afe806b583e247a75a07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771178"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="a7c43-103">deviceEnrollmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7c43-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="a7c43-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7c43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7c43-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7c43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7c43-106">设备注册配置的基类</span><span class="sxs-lookup"><span data-stu-id="a7c43-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="a7c43-107">方法</span><span class="sxs-lookup"><span data-stu-id="a7c43-107">Methods</span></span>
|<span data-ttu-id="a7c43-108">方法</span><span class="sxs-lookup"><span data-stu-id="a7c43-108">Method</span></span>|<span data-ttu-id="a7c43-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7c43-109">Return Type</span></span>|<span data-ttu-id="a7c43-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7c43-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7c43-111">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="a7c43-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="a7c43-112">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7c43-112">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="a7c43-113">列出 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7c43-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a7c43-114">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7c43-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="a7c43-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7c43-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="a7c43-116">读取 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7c43-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="a7c43-117">**载入**</span><span class="sxs-lookup"><span data-stu-id="a7c43-117">**Onboarding**</span></span>|
|[<span data-ttu-id="a7c43-118">setPriority action</span><span class="sxs-lookup"><span data-stu-id="a7c43-118">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="a7c43-119">无</span><span class="sxs-lookup"><span data-stu-id="a7c43-119">None</span></span>|<span data-ttu-id="a7c43-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a7c43-120">Not yet documented</span></span>|
|[<span data-ttu-id="a7c43-121">分配操作</span><span class="sxs-lookup"><span data-stu-id="a7c43-121">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="a7c43-122">无</span><span class="sxs-lookup"><span data-stu-id="a7c43-122">None</span></span>|<span data-ttu-id="a7c43-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a7c43-123">Not yet documented</span></span>|
|<span data-ttu-id="a7c43-124">**策略集**</span><span class="sxs-lookup"><span data-stu-id="a7c43-124">**Policy Set**</span></span>|
|[<span data-ttu-id="a7c43-125">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="a7c43-125">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="a7c43-126">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="a7c43-126">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="a7c43-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a7c43-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a7c43-128">属性</span><span class="sxs-lookup"><span data-stu-id="a7c43-128">Properties</span></span>
|<span data-ttu-id="a7c43-129">属性</span><span class="sxs-lookup"><span data-stu-id="a7c43-129">Property</span></span>|<span data-ttu-id="a7c43-130">类型</span><span class="sxs-lookup"><span data-stu-id="a7c43-130">Type</span></span>|<span data-ttu-id="a7c43-131">说明</span><span class="sxs-lookup"><span data-stu-id="a7c43-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c43-132">id</span><span class="sxs-lookup"><span data-stu-id="a7c43-132">id</span></span>|<span data-ttu-id="a7c43-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a7c43-133">String</span></span>|<span data-ttu-id="a7c43-134">帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="a7c43-134">Unique Identifier for the account</span></span>|
|<span data-ttu-id="a7c43-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a7c43-135">displayName</span></span>|<span data-ttu-id="a7c43-136">String</span><span class="sxs-lookup"><span data-stu-id="a7c43-136">String</span></span>|<span data-ttu-id="a7c43-137">设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="a7c43-137">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="a7c43-138">说明</span><span class="sxs-lookup"><span data-stu-id="a7c43-138">description</span></span>|<span data-ttu-id="a7c43-139">String</span><span class="sxs-lookup"><span data-stu-id="a7c43-139">String</span></span>|<span data-ttu-id="a7c43-140">设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="a7c43-140">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="a7c43-141">priority</span><span class="sxs-lookup"><span data-stu-id="a7c43-141">priority</span></span>|<span data-ttu-id="a7c43-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a7c43-142">Int32</span></span>|<span data-ttu-id="a7c43-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="a7c43-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="a7c43-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="a7c43-144">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="a7c43-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c43-145">createdDateTime</span></span>|<span data-ttu-id="a7c43-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c43-146">DateTimeOffset</span></span>|<span data-ttu-id="a7c43-147">设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="a7c43-147">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="a7c43-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c43-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a7c43-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c43-149">DateTimeOffset</span></span>|<span data-ttu-id="a7c43-150">设备注册配置的上次修改日期时间（UTC）</span><span class="sxs-lookup"><span data-stu-id="a7c43-150">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="a7c43-151">version</span><span class="sxs-lookup"><span data-stu-id="a7c43-151">version</span></span>|<span data-ttu-id="a7c43-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a7c43-152">Int32</span></span>|<span data-ttu-id="a7c43-153">设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="a7c43-153">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c43-154">关系</span><span class="sxs-lookup"><span data-stu-id="a7c43-154">Relationships</span></span>
|<span data-ttu-id="a7c43-155">关系</span><span class="sxs-lookup"><span data-stu-id="a7c43-155">Relationship</span></span>|<span data-ttu-id="a7c43-156">类型</span><span class="sxs-lookup"><span data-stu-id="a7c43-156">Type</span></span>|<span data-ttu-id="a7c43-157">说明</span><span class="sxs-lookup"><span data-stu-id="a7c43-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c43-158">**载入**</span><span class="sxs-lookup"><span data-stu-id="a7c43-158">**Onboarding**</span></span>|
|<span data-ttu-id="a7c43-159">assignments</span><span class="sxs-lookup"><span data-stu-id="a7c43-159">assignments</span></span>|<span data-ttu-id="a7c43-160">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7c43-160">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a7c43-161">设备配置文件的组分配列表</span><span class="sxs-lookup"><span data-stu-id="a7c43-161">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7c43-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7c43-162">JSON Representation</span></span>
<span data-ttu-id="a7c43-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7c43-163">Here is a JSON representation of the resource.</span></span>
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



