---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d05914e1b25ac3712ac60274facf0904c91d4224
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940454"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="68a0b-103">deviceEnrollmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="68a0b-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="68a0b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68a0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68a0b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68a0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68a0b-106">设备注册配置的基类</span><span class="sxs-lookup"><span data-stu-id="68a0b-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="68a0b-107">方法</span><span class="sxs-lookup"><span data-stu-id="68a0b-107">Methods</span></span>
|<span data-ttu-id="68a0b-108">方法</span><span class="sxs-lookup"><span data-stu-id="68a0b-108">Method</span></span>|<span data-ttu-id="68a0b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="68a0b-109">Return Type</span></span>|<span data-ttu-id="68a0b-110">说明</span><span class="sxs-lookup"><span data-stu-id="68a0b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68a0b-111">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="68a0b-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="68a0b-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68a0b-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="68a0b-113">列出 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="68a0b-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="68a0b-114">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="68a0b-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="68a0b-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="68a0b-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|<span data-ttu-id="68a0b-116">读取 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="68a0b-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>|
|[<span data-ttu-id="68a0b-117">setPriority action</span><span class="sxs-lookup"><span data-stu-id="68a0b-117">setPriority action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="68a0b-118">无</span><span class="sxs-lookup"><span data-stu-id="68a0b-118">None</span></span>|<span data-ttu-id="68a0b-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="68a0b-119">Not yet documented</span></span>|
|[<span data-ttu-id="68a0b-120">分配操作</span><span class="sxs-lookup"><span data-stu-id="68a0b-120">assign action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="68a0b-121">无</span><span class="sxs-lookup"><span data-stu-id="68a0b-121">None</span></span>|<span data-ttu-id="68a0b-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="68a0b-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="68a0b-123">属性</span><span class="sxs-lookup"><span data-stu-id="68a0b-123">Properties</span></span>
|<span data-ttu-id="68a0b-124">属性</span><span class="sxs-lookup"><span data-stu-id="68a0b-124">Property</span></span>|<span data-ttu-id="68a0b-125">类型</span><span class="sxs-lookup"><span data-stu-id="68a0b-125">Type</span></span>|<span data-ttu-id="68a0b-126">说明</span><span class="sxs-lookup"><span data-stu-id="68a0b-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68a0b-127">id</span><span class="sxs-lookup"><span data-stu-id="68a0b-127">id</span></span>|<span data-ttu-id="68a0b-128">字符串</span><span class="sxs-lookup"><span data-stu-id="68a0b-128">String</span></span>|<span data-ttu-id="68a0b-129">帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="68a0b-129">Unique Identifier for the account</span></span>|
|<span data-ttu-id="68a0b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="68a0b-130">displayName</span></span>|<span data-ttu-id="68a0b-131">String</span><span class="sxs-lookup"><span data-stu-id="68a0b-131">String</span></span>|<span data-ttu-id="68a0b-132">设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="68a0b-132">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="68a0b-133">说明</span><span class="sxs-lookup"><span data-stu-id="68a0b-133">description</span></span>|<span data-ttu-id="68a0b-134">String</span><span class="sxs-lookup"><span data-stu-id="68a0b-134">String</span></span>|<span data-ttu-id="68a0b-135">设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="68a0b-135">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="68a0b-136">priority</span><span class="sxs-lookup"><span data-stu-id="68a0b-136">priority</span></span>|<span data-ttu-id="68a0b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="68a0b-137">Int32</span></span>|<span data-ttu-id="68a0b-138">当用户存在于分配有注册配置的多个组中时, 将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="68a0b-138">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="68a0b-139">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="68a0b-139">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="68a0b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68a0b-140">createdDateTime</span></span>|<span data-ttu-id="68a0b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68a0b-141">DateTimeOffset</span></span>|<span data-ttu-id="68a0b-142">设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="68a0b-142">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="68a0b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68a0b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="68a0b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68a0b-144">DateTimeOffset</span></span>|<span data-ttu-id="68a0b-145">设备注册配置的上次修改日期时间 (UTC)</span><span class="sxs-lookup"><span data-stu-id="68a0b-145">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="68a0b-146">version</span><span class="sxs-lookup"><span data-stu-id="68a0b-146">version</span></span>|<span data-ttu-id="68a0b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="68a0b-147">Int32</span></span>|<span data-ttu-id="68a0b-148">设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="68a0b-148">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="68a0b-149">关系</span><span class="sxs-lookup"><span data-stu-id="68a0b-149">Relationships</span></span>
|<span data-ttu-id="68a0b-150">关系</span><span class="sxs-lookup"><span data-stu-id="68a0b-150">Relationship</span></span>|<span data-ttu-id="68a0b-151">类型</span><span class="sxs-lookup"><span data-stu-id="68a0b-151">Type</span></span>|<span data-ttu-id="68a0b-152">说明</span><span class="sxs-lookup"><span data-stu-id="68a0b-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68a0b-153">assignments</span><span class="sxs-lookup"><span data-stu-id="68a0b-153">assignments</span></span>|<span data-ttu-id="68a0b-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68a0b-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="68a0b-155">设备配置文件的组分配列表</span><span class="sxs-lookup"><span data-stu-id="68a0b-155">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68a0b-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68a0b-156">JSON Representation</span></span>
<span data-ttu-id="68a0b-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68a0b-157">Here is a JSON representation of the resource.</span></span>
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




