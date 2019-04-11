---
title: deviceManagementStringSettingInstance 资源类型
description: 一个代表字符串值的设置实例
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3297085a905934792de2d371f295b467ad9a8e44
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794944"
---
# <a name="devicemanagementstringsettinginstance-resource-type"></a><span data-ttu-id="56a75-103">deviceManagementStringSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="56a75-103">deviceManagementStringSettingInstance resource type</span></span>

> <span data-ttu-id="56a75-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56a75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56a75-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56a75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56a75-106">一个代表字符串值的设置实例</span><span class="sxs-lookup"><span data-stu-id="56a75-106">A setting instance representing a string value</span></span>


<span data-ttu-id="56a75-107">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="56a75-107">Inherits from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>

## <a name="methods"></a><span data-ttu-id="56a75-108">方法</span><span class="sxs-lookup"><span data-stu-id="56a75-108">Methods</span></span>
|<span data-ttu-id="56a75-109">方法</span><span class="sxs-lookup"><span data-stu-id="56a75-109">Method</span></span>|<span data-ttu-id="56a75-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="56a75-110">Return Type</span></span>|<span data-ttu-id="56a75-111">说明</span><span class="sxs-lookup"><span data-stu-id="56a75-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56a75-112">列出 deviceManagementStringSettingInstances</span><span class="sxs-lookup"><span data-stu-id="56a75-112">List deviceManagementStringSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-list.md)|<span data-ttu-id="56a75-113">[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="56a75-113">[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) collection</span></span>|<span data-ttu-id="56a75-114">列出[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56a75-114">List properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="56a75-115">获取 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="56a75-115">Get deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-get.md)|[<span data-ttu-id="56a75-116">deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="56a75-116">deviceManagementStringSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|<span data-ttu-id="56a75-117">读取[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56a75-117">Read properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>|
|[<span data-ttu-id="56a75-118">创建 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="56a75-118">Create deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-create.md)|[<span data-ttu-id="56a75-119">deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="56a75-119">deviceManagementStringSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|<span data-ttu-id="56a75-120">创建新的[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="56a75-120">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>|
|[<span data-ttu-id="56a75-121">删除 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="56a75-121">Delete deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-delete.md)|<span data-ttu-id="56a75-122">无</span><span class="sxs-lookup"><span data-stu-id="56a75-122">None</span></span>|<span data-ttu-id="56a75-123">删除[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)。</span><span class="sxs-lookup"><span data-stu-id="56a75-123">Deletes a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>|
|[<span data-ttu-id="56a75-124">更新 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="56a75-124">Update deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-update.md)|[<span data-ttu-id="56a75-125">deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="56a75-125">deviceManagementStringSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|<span data-ttu-id="56a75-126">更新[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56a75-126">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56a75-127">属性</span><span class="sxs-lookup"><span data-stu-id="56a75-127">Properties</span></span>
|<span data-ttu-id="56a75-128">属性</span><span class="sxs-lookup"><span data-stu-id="56a75-128">Property</span></span>|<span data-ttu-id="56a75-129">类型</span><span class="sxs-lookup"><span data-stu-id="56a75-129">Type</span></span>|<span data-ttu-id="56a75-130">说明</span><span class="sxs-lookup"><span data-stu-id="56a75-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a75-131">id</span><span class="sxs-lookup"><span data-stu-id="56a75-131">id</span></span>|<span data-ttu-id="56a75-132">String</span><span class="sxs-lookup"><span data-stu-id="56a75-132">String</span></span>|<span data-ttu-id="56a75-133">从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="56a75-133">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="56a75-134">definitionId</span><span class="sxs-lookup"><span data-stu-id="56a75-134">definitionId</span></span>|<span data-ttu-id="56a75-135">String</span><span class="sxs-lookup"><span data-stu-id="56a75-135">String</span></span>|<span data-ttu-id="56a75-136">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="56a75-136">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="56a75-137">valueJson</span><span class="sxs-lookup"><span data-stu-id="56a75-137">valueJson</span></span>|<span data-ttu-id="56a75-138">String</span><span class="sxs-lookup"><span data-stu-id="56a75-138">String</span></span>|<span data-ttu-id="56a75-139">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56a75-139">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="56a75-140">value</span><span class="sxs-lookup"><span data-stu-id="56a75-140">value</span></span>|<span data-ttu-id="56a75-141">String</span><span class="sxs-lookup"><span data-stu-id="56a75-141">String</span></span>|<span data-ttu-id="56a75-142">字符串值</span><span class="sxs-lookup"><span data-stu-id="56a75-142">The string value</span></span>|

## <a name="relationships"></a><span data-ttu-id="56a75-143">关系</span><span class="sxs-lookup"><span data-stu-id="56a75-143">Relationships</span></span>
<span data-ttu-id="56a75-144">无</span><span class="sxs-lookup"><span data-stu-id="56a75-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56a75-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56a75-145">JSON Representation</span></span>
<span data-ttu-id="56a75-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56a75-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementStringSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": "String"
}
```





