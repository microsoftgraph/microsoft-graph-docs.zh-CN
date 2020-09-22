---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7e5c2a1eef152ba613be8909ca80f6040305720
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055323"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="49359-103">deviceEnrollmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="49359-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="49359-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49359-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49359-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49359-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49359-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49359-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49359-107">设备注册配置的基类</span><span class="sxs-lookup"><span data-stu-id="49359-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="49359-108">方法</span><span class="sxs-lookup"><span data-stu-id="49359-108">Methods</span></span>
|<span data-ttu-id="49359-109">方法</span><span class="sxs-lookup"><span data-stu-id="49359-109">Method</span></span>|<span data-ttu-id="49359-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="49359-110">Return Type</span></span>|<span data-ttu-id="49359-111">说明</span><span class="sxs-lookup"><span data-stu-id="49359-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49359-112">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="49359-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="49359-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="49359-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="49359-114">列出 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49359-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="49359-115">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="49359-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="49359-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="49359-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="49359-117">读取 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49359-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="49359-118">**载入**</span><span class="sxs-lookup"><span data-stu-id="49359-118">**Onboarding**</span></span>|
|[<span data-ttu-id="49359-119">setPriority action</span><span class="sxs-lookup"><span data-stu-id="49359-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="49359-120">无</span><span class="sxs-lookup"><span data-stu-id="49359-120">None</span></span>|<span data-ttu-id="49359-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49359-121">Not yet documented</span></span>|
|[<span data-ttu-id="49359-122">分配操作</span><span class="sxs-lookup"><span data-stu-id="49359-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="49359-123">无</span><span class="sxs-lookup"><span data-stu-id="49359-123">None</span></span>|<span data-ttu-id="49359-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49359-124">Not yet documented</span></span>|
|<span data-ttu-id="49359-125">**策略集**</span><span class="sxs-lookup"><span data-stu-id="49359-125">**Policy Set**</span></span>|
|[<span data-ttu-id="49359-126">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="49359-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="49359-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="49359-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="49359-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49359-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="49359-129">属性</span><span class="sxs-lookup"><span data-stu-id="49359-129">Properties</span></span>
|<span data-ttu-id="49359-130">属性</span><span class="sxs-lookup"><span data-stu-id="49359-130">Property</span></span>|<span data-ttu-id="49359-131">类型</span><span class="sxs-lookup"><span data-stu-id="49359-131">Type</span></span>|<span data-ttu-id="49359-132">说明</span><span class="sxs-lookup"><span data-stu-id="49359-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49359-133">id</span><span class="sxs-lookup"><span data-stu-id="49359-133">id</span></span>|<span data-ttu-id="49359-134">String</span><span class="sxs-lookup"><span data-stu-id="49359-134">String</span></span>|<span data-ttu-id="49359-135">帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="49359-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="49359-136">displayName</span><span class="sxs-lookup"><span data-stu-id="49359-136">displayName</span></span>|<span data-ttu-id="49359-137">String</span><span class="sxs-lookup"><span data-stu-id="49359-137">String</span></span>|<span data-ttu-id="49359-138">设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="49359-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="49359-139">说明</span><span class="sxs-lookup"><span data-stu-id="49359-139">description</span></span>|<span data-ttu-id="49359-140">String</span><span class="sxs-lookup"><span data-stu-id="49359-140">String</span></span>|<span data-ttu-id="49359-141">设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="49359-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="49359-142">priority</span><span class="sxs-lookup"><span data-stu-id="49359-142">priority</span></span>|<span data-ttu-id="49359-143">Int32</span><span class="sxs-lookup"><span data-stu-id="49359-143">Int32</span></span>|<span data-ttu-id="49359-144">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="49359-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="49359-145">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="49359-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="49359-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49359-146">createdDateTime</span></span>|<span data-ttu-id="49359-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49359-147">DateTimeOffset</span></span>|<span data-ttu-id="49359-148">设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="49359-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="49359-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49359-149">lastModifiedDateTime</span></span>|<span data-ttu-id="49359-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49359-150">DateTimeOffset</span></span>|<span data-ttu-id="49359-151">设备注册配置的上次修改日期时间（UTC）</span><span class="sxs-lookup"><span data-stu-id="49359-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="49359-152">version</span><span class="sxs-lookup"><span data-stu-id="49359-152">version</span></span>|<span data-ttu-id="49359-153">Int32</span><span class="sxs-lookup"><span data-stu-id="49359-153">Int32</span></span>|<span data-ttu-id="49359-154">设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="49359-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="49359-155">关系</span><span class="sxs-lookup"><span data-stu-id="49359-155">Relationships</span></span>
|<span data-ttu-id="49359-156">关系</span><span class="sxs-lookup"><span data-stu-id="49359-156">Relationship</span></span>|<span data-ttu-id="49359-157">类型</span><span class="sxs-lookup"><span data-stu-id="49359-157">Type</span></span>|<span data-ttu-id="49359-158">说明</span><span class="sxs-lookup"><span data-stu-id="49359-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49359-159">**载入**</span><span class="sxs-lookup"><span data-stu-id="49359-159">**Onboarding**</span></span>|
|<span data-ttu-id="49359-160">assignments</span><span class="sxs-lookup"><span data-stu-id="49359-160">assignments</span></span>|<span data-ttu-id="49359-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="49359-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="49359-162">设备配置文件的组分配列表</span><span class="sxs-lookup"><span data-stu-id="49359-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49359-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49359-163">JSON Representation</span></span>
<span data-ttu-id="49359-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49359-164">Here is a JSON representation of the resource.</span></span>
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






