---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d46e446aab9806ad856f71cb8ac57c2f75f1b55
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865794"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="864d0-103">deviceEnrollmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="864d0-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="864d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="864d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="864d0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="864d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="864d0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="864d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="864d0-107">设备注册配置的基类</span><span class="sxs-lookup"><span data-stu-id="864d0-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="864d0-108">方法</span><span class="sxs-lookup"><span data-stu-id="864d0-108">Methods</span></span>
|<span data-ttu-id="864d0-109">方法</span><span class="sxs-lookup"><span data-stu-id="864d0-109">Method</span></span>|<span data-ttu-id="864d0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="864d0-110">Return Type</span></span>|<span data-ttu-id="864d0-111">说明</span><span class="sxs-lookup"><span data-stu-id="864d0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="864d0-112">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="864d0-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="864d0-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="864d0-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="864d0-114">列出 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="864d0-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="864d0-115">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="864d0-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="864d0-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="864d0-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="864d0-117">读取 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="864d0-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="864d0-118">**载入**</span><span class="sxs-lookup"><span data-stu-id="864d0-118">**Onboarding**</span></span>|
|[<span data-ttu-id="864d0-119">setPriority action</span><span class="sxs-lookup"><span data-stu-id="864d0-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="864d0-120">无</span><span class="sxs-lookup"><span data-stu-id="864d0-120">None</span></span>|<span data-ttu-id="864d0-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="864d0-121">Not yet documented</span></span>|
|[<span data-ttu-id="864d0-122">分配操作</span><span class="sxs-lookup"><span data-stu-id="864d0-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="864d0-123">无</span><span class="sxs-lookup"><span data-stu-id="864d0-123">None</span></span>|<span data-ttu-id="864d0-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="864d0-124">Not yet documented</span></span>|
|<span data-ttu-id="864d0-125">**策略集**</span><span class="sxs-lookup"><span data-stu-id="864d0-125">**Policy Set**</span></span>|
|[<span data-ttu-id="864d0-126">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="864d0-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="864d0-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="864d0-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="864d0-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="864d0-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="864d0-129">属性</span><span class="sxs-lookup"><span data-stu-id="864d0-129">Properties</span></span>
|<span data-ttu-id="864d0-130">属性</span><span class="sxs-lookup"><span data-stu-id="864d0-130">Property</span></span>|<span data-ttu-id="864d0-131">类型</span><span class="sxs-lookup"><span data-stu-id="864d0-131">Type</span></span>|<span data-ttu-id="864d0-132">说明</span><span class="sxs-lookup"><span data-stu-id="864d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="864d0-133">id</span><span class="sxs-lookup"><span data-stu-id="864d0-133">id</span></span>|<span data-ttu-id="864d0-134">String</span><span class="sxs-lookup"><span data-stu-id="864d0-134">String</span></span>|<span data-ttu-id="864d0-135">帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="864d0-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="864d0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="864d0-136">displayName</span></span>|<span data-ttu-id="864d0-137">String</span><span class="sxs-lookup"><span data-stu-id="864d0-137">String</span></span>|<span data-ttu-id="864d0-138">设备显示名称配置</span><span class="sxs-lookup"><span data-stu-id="864d0-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="864d0-139">说明</span><span class="sxs-lookup"><span data-stu-id="864d0-139">description</span></span>|<span data-ttu-id="864d0-140">String</span><span class="sxs-lookup"><span data-stu-id="864d0-140">String</span></span>|<span data-ttu-id="864d0-141">设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="864d0-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="864d0-142">priority</span><span class="sxs-lookup"><span data-stu-id="864d0-142">priority</span></span>|<span data-ttu-id="864d0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="864d0-143">Int32</span></span>|<span data-ttu-id="864d0-144">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="864d0-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="864d0-145">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="864d0-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="864d0-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="864d0-146">createdDateTime</span></span>|<span data-ttu-id="864d0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="864d0-147">DateTimeOffset</span></span>|<span data-ttu-id="864d0-148">设备注册配置的创建日期时间（UTC）</span><span class="sxs-lookup"><span data-stu-id="864d0-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="864d0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="864d0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="864d0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="864d0-150">DateTimeOffset</span></span>|<span data-ttu-id="864d0-151">设备注册配置的上次修改日期时间（UTC）</span><span class="sxs-lookup"><span data-stu-id="864d0-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="864d0-152">version</span><span class="sxs-lookup"><span data-stu-id="864d0-152">version</span></span>|<span data-ttu-id="864d0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="864d0-153">Int32</span></span>|<span data-ttu-id="864d0-154">设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="864d0-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="864d0-155">关系</span><span class="sxs-lookup"><span data-stu-id="864d0-155">Relationships</span></span>
|<span data-ttu-id="864d0-156">关系</span><span class="sxs-lookup"><span data-stu-id="864d0-156">Relationship</span></span>|<span data-ttu-id="864d0-157">类型</span><span class="sxs-lookup"><span data-stu-id="864d0-157">Type</span></span>|<span data-ttu-id="864d0-158">说明</span><span class="sxs-lookup"><span data-stu-id="864d0-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="864d0-159">**载入**</span><span class="sxs-lookup"><span data-stu-id="864d0-159">**Onboarding**</span></span>|
|<span data-ttu-id="864d0-160">assignments</span><span class="sxs-lookup"><span data-stu-id="864d0-160">assignments</span></span>|<span data-ttu-id="864d0-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="864d0-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="864d0-162">设备配置文件的组分配列表</span><span class="sxs-lookup"><span data-stu-id="864d0-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="864d0-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="864d0-163">JSON Representation</span></span>
<span data-ttu-id="864d0-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="864d0-164">Here is a JSON representation of the resource.</span></span>
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




