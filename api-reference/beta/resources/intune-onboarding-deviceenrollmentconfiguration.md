---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34b62ec6a00e47ed307951a881e247e0914b5c0b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998287"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="d2d66-103">deviceEnrollmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2d66-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="d2d66-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2d66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2d66-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2d66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d66-106">设备注册配置的基类</span><span class="sxs-lookup"><span data-stu-id="d2d66-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="d2d66-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2d66-107">Methods</span></span>
|<span data-ttu-id="d2d66-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2d66-108">Method</span></span>|<span data-ttu-id="d2d66-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2d66-109">Return Type</span></span>|<span data-ttu-id="d2d66-110">说明</span><span class="sxs-lookup"><span data-stu-id="d2d66-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2d66-111">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="d2d66-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="d2d66-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2d66-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="d2d66-113">列出 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2d66-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d2d66-114">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2d66-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="d2d66-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2d66-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|<span data-ttu-id="d2d66-116">读取 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2d66-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d2d66-117">setPriority action</span><span class="sxs-lookup"><span data-stu-id="d2d66-117">setPriority action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="d2d66-118">无</span><span class="sxs-lookup"><span data-stu-id="d2d66-118">None</span></span>|<span data-ttu-id="d2d66-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2d66-119">Not yet documented</span></span>|
|[<span data-ttu-id="d2d66-120">分配操作</span><span class="sxs-lookup"><span data-stu-id="d2d66-120">assign action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="d2d66-121">无</span><span class="sxs-lookup"><span data-stu-id="d2d66-121">None</span></span>|<span data-ttu-id="d2d66-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2d66-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d2d66-123">属性</span><span class="sxs-lookup"><span data-stu-id="d2d66-123">Properties</span></span>
|<span data-ttu-id="d2d66-124">属性</span><span class="sxs-lookup"><span data-stu-id="d2d66-124">Property</span></span>|<span data-ttu-id="d2d66-125">类型</span><span class="sxs-lookup"><span data-stu-id="d2d66-125">Type</span></span>|<span data-ttu-id="d2d66-126">说明</span><span class="sxs-lookup"><span data-stu-id="d2d66-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d66-127">id</span><span class="sxs-lookup"><span data-stu-id="d2d66-127">id</span></span>|<span data-ttu-id="d2d66-128">字符串</span><span class="sxs-lookup"><span data-stu-id="d2d66-128">String</span></span>|<span data-ttu-id="d2d66-129">帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d2d66-129">Unique Identifier for the account</span></span>|
|<span data-ttu-id="d2d66-130">displayName</span><span class="sxs-lookup"><span data-stu-id="d2d66-130">displayName</span></span>|<span data-ttu-id="d2d66-131">String</span><span class="sxs-lookup"><span data-stu-id="d2d66-131">String</span></span>|<span data-ttu-id="d2d66-132">设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="d2d66-132">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="d2d66-133">说明</span><span class="sxs-lookup"><span data-stu-id="d2d66-133">description</span></span>|<span data-ttu-id="d2d66-134">String</span><span class="sxs-lookup"><span data-stu-id="d2d66-134">String</span></span>|<span data-ttu-id="d2d66-135">设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="d2d66-135">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="d2d66-136">priority</span><span class="sxs-lookup"><span data-stu-id="d2d66-136">priority</span></span>|<span data-ttu-id="d2d66-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d66-137">Int32</span></span>|<span data-ttu-id="d2d66-138">当用户存在于分配有注册配置的多个组中时, 将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="d2d66-138">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d2d66-139">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="d2d66-139">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="d2d66-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d66-140">createdDateTime</span></span>|<span data-ttu-id="d2d66-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d66-141">DateTimeOffset</span></span>|<span data-ttu-id="d2d66-142">设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="d2d66-142">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="d2d66-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d66-143">lastModifiedDateTime</span></span>|<span data-ttu-id="d2d66-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d66-144">DateTimeOffset</span></span>|<span data-ttu-id="d2d66-145">设备注册配置的上次修改日期时间 (UTC)</span><span class="sxs-lookup"><span data-stu-id="d2d66-145">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="d2d66-146">version</span><span class="sxs-lookup"><span data-stu-id="d2d66-146">version</span></span>|<span data-ttu-id="d2d66-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d2d66-147">Int32</span></span>|<span data-ttu-id="d2d66-148">设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="d2d66-148">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2d66-149">关系</span><span class="sxs-lookup"><span data-stu-id="d2d66-149">Relationships</span></span>
|<span data-ttu-id="d2d66-150">关系</span><span class="sxs-lookup"><span data-stu-id="d2d66-150">Relationship</span></span>|<span data-ttu-id="d2d66-151">类型</span><span class="sxs-lookup"><span data-stu-id="d2d66-151">Type</span></span>|<span data-ttu-id="d2d66-152">说明</span><span class="sxs-lookup"><span data-stu-id="d2d66-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d66-153">assignments</span><span class="sxs-lookup"><span data-stu-id="d2d66-153">assignments</span></span>|<span data-ttu-id="d2d66-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2d66-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d2d66-155">设备配置文件的组分配列表</span><span class="sxs-lookup"><span data-stu-id="d2d66-155">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2d66-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2d66-156">JSON Representation</span></span>
<span data-ttu-id="d2d66-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2d66-157">Here is a JSON representation of the resource.</span></span>
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





