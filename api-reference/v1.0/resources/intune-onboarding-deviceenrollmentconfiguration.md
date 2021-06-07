---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03787eed949221af2b4cbee5ca08d107aa60c229
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752754"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="9081a-103">deviceEnrollmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="9081a-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="9081a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9081a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9081a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9081a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9081a-106">设备注册配置的基类</span><span class="sxs-lookup"><span data-stu-id="9081a-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="9081a-107">Methods</span><span class="sxs-lookup"><span data-stu-id="9081a-107">Methods</span></span>
|<span data-ttu-id="9081a-108">方法</span><span class="sxs-lookup"><span data-stu-id="9081a-108">Method</span></span>|<span data-ttu-id="9081a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9081a-109">Return Type</span></span>|<span data-ttu-id="9081a-110">Description</span><span class="sxs-lookup"><span data-stu-id="9081a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9081a-111">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="9081a-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="9081a-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9081a-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="9081a-113">列出 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9081a-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="9081a-114">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="9081a-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="9081a-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="9081a-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|<span data-ttu-id="9081a-116">读取 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9081a-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9081a-117">setPriority action</span><span class="sxs-lookup"><span data-stu-id="9081a-117">setPriority action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="9081a-118">无</span><span class="sxs-lookup"><span data-stu-id="9081a-118">None</span></span>|<span data-ttu-id="9081a-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9081a-119">Not yet documented</span></span>|
|[<span data-ttu-id="9081a-120">分配操作</span><span class="sxs-lookup"><span data-stu-id="9081a-120">assign action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="9081a-121">无</span><span class="sxs-lookup"><span data-stu-id="9081a-121">None</span></span>|<span data-ttu-id="9081a-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9081a-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9081a-123">属性</span><span class="sxs-lookup"><span data-stu-id="9081a-123">Properties</span></span>
|<span data-ttu-id="9081a-124">属性</span><span class="sxs-lookup"><span data-stu-id="9081a-124">Property</span></span>|<span data-ttu-id="9081a-125">类型</span><span class="sxs-lookup"><span data-stu-id="9081a-125">Type</span></span>|<span data-ttu-id="9081a-126">说明</span><span class="sxs-lookup"><span data-stu-id="9081a-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9081a-127">id</span><span class="sxs-lookup"><span data-stu-id="9081a-127">id</span></span>|<span data-ttu-id="9081a-128">String</span><span class="sxs-lookup"><span data-stu-id="9081a-128">String</span></span>|<span data-ttu-id="9081a-129">帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="9081a-129">Unique Identifier for the account</span></span>|
|<span data-ttu-id="9081a-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9081a-130">displayName</span></span>|<span data-ttu-id="9081a-131">String</span><span class="sxs-lookup"><span data-stu-id="9081a-131">String</span></span>|<span data-ttu-id="9081a-132">设备显示名称配置</span><span class="sxs-lookup"><span data-stu-id="9081a-132">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="9081a-133">说明</span><span class="sxs-lookup"><span data-stu-id="9081a-133">description</span></span>|<span data-ttu-id="9081a-134">String</span><span class="sxs-lookup"><span data-stu-id="9081a-134">String</span></span>|<span data-ttu-id="9081a-135">设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="9081a-135">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="9081a-136">priority</span><span class="sxs-lookup"><span data-stu-id="9081a-136">priority</span></span>|<span data-ttu-id="9081a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9081a-137">Int32</span></span>|<span data-ttu-id="9081a-138">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="9081a-138">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="9081a-139">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="9081a-139">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="9081a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9081a-140">createdDateTime</span></span>|<span data-ttu-id="9081a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9081a-141">DateTimeOffset</span></span>|<span data-ttu-id="9081a-142">设备注册配置的创建日期时间（UTC）</span><span class="sxs-lookup"><span data-stu-id="9081a-142">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="9081a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9081a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9081a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9081a-144">DateTimeOffset</span></span>|<span data-ttu-id="9081a-145">设备注册配置的上次修改日期时间（UTC）</span><span class="sxs-lookup"><span data-stu-id="9081a-145">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="9081a-146">version</span><span class="sxs-lookup"><span data-stu-id="9081a-146">version</span></span>|<span data-ttu-id="9081a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9081a-147">Int32</span></span>|<span data-ttu-id="9081a-148">设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="9081a-148">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="9081a-149">关系</span><span class="sxs-lookup"><span data-stu-id="9081a-149">Relationships</span></span>
|<span data-ttu-id="9081a-150">关系</span><span class="sxs-lookup"><span data-stu-id="9081a-150">Relationship</span></span>|<span data-ttu-id="9081a-151">类型</span><span class="sxs-lookup"><span data-stu-id="9081a-151">Type</span></span>|<span data-ttu-id="9081a-152">Description</span><span class="sxs-lookup"><span data-stu-id="9081a-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9081a-153">assignments</span><span class="sxs-lookup"><span data-stu-id="9081a-153">assignments</span></span>|<span data-ttu-id="9081a-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9081a-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9081a-155">设备配置文件的组分配列表</span><span class="sxs-lookup"><span data-stu-id="9081a-155">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9081a-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9081a-156">JSON Representation</span></span>
<span data-ttu-id="9081a-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9081a-157">Here is a JSON representation of the resource.</span></span>
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




