---
title: deviceManagementStringSettingInstance 资源类型
description: 一个代表字符串值的设置实例
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ea58c6fdb4a8ad3a2a68ead7044943093c22bb1
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522543"
---
# <a name="devicemanagementstringsettinginstance-resource-type"></a><span data-ttu-id="1f538-103">deviceManagementStringSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f538-103">deviceManagementStringSettingInstance resource type</span></span>

> <span data-ttu-id="1f538-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f538-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f538-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f538-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f538-106">一个代表字符串值的设置实例</span><span class="sxs-lookup"><span data-stu-id="1f538-106">A setting instance representing a string value</span></span>


<span data-ttu-id="1f538-107">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1f538-107">Inherits from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1f538-108">方法</span><span class="sxs-lookup"><span data-stu-id="1f538-108">Methods</span></span>
|<span data-ttu-id="1f538-109">方法</span><span class="sxs-lookup"><span data-stu-id="1f538-109">Method</span></span>|<span data-ttu-id="1f538-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1f538-110">Return Type</span></span>|<span data-ttu-id="1f538-111">说明</span><span class="sxs-lookup"><span data-stu-id="1f538-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f538-112">列出 deviceManagementStringSettingInstances</span><span class="sxs-lookup"><span data-stu-id="1f538-112">List deviceManagementStringSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-list.md)|<span data-ttu-id="1f538-113">[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="1f538-113">[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) collection</span></span>|<span data-ttu-id="1f538-114">列出[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f538-114">List properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="1f538-115">获取 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f538-115">Get deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-get.md)|[<span data-ttu-id="1f538-116">deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f538-116">deviceManagementStringSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|<span data-ttu-id="1f538-117">读取[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f538-117">Read properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>|
|[<span data-ttu-id="1f538-118">创建 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f538-118">Create deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-create.md)|[<span data-ttu-id="1f538-119">deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f538-119">deviceManagementStringSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|<span data-ttu-id="1f538-120">创建新的[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1f538-120">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>|
|[<span data-ttu-id="1f538-121">删除 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f538-121">Delete deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-delete.md)|<span data-ttu-id="1f538-122">无</span><span class="sxs-lookup"><span data-stu-id="1f538-122">None</span></span>|<span data-ttu-id="1f538-123">删除[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)。</span><span class="sxs-lookup"><span data-stu-id="1f538-123">Deletes a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>|
|[<span data-ttu-id="1f538-124">更新 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f538-124">Update deviceManagementStringSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementstringsettinginstance-update.md)|[<span data-ttu-id="1f538-125">deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f538-125">deviceManagementStringSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|<span data-ttu-id="1f538-126">更新[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f538-126">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f538-127">属性</span><span class="sxs-lookup"><span data-stu-id="1f538-127">Properties</span></span>
|<span data-ttu-id="1f538-128">属性</span><span class="sxs-lookup"><span data-stu-id="1f538-128">Property</span></span>|<span data-ttu-id="1f538-129">类型</span><span class="sxs-lookup"><span data-stu-id="1f538-129">Type</span></span>|<span data-ttu-id="1f538-130">说明</span><span class="sxs-lookup"><span data-stu-id="1f538-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f538-131">id</span><span class="sxs-lookup"><span data-stu-id="1f538-131">id</span></span>|<span data-ttu-id="1f538-132">String</span><span class="sxs-lookup"><span data-stu-id="1f538-132">String</span></span>|<span data-ttu-id="1f538-133">从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="1f538-133">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f538-134">definitionId</span><span class="sxs-lookup"><span data-stu-id="1f538-134">definitionId</span></span>|<span data-ttu-id="1f538-135">String</span><span class="sxs-lookup"><span data-stu-id="1f538-135">String</span></span>|<span data-ttu-id="1f538-136">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="1f538-136">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f538-137">valueJson</span><span class="sxs-lookup"><span data-stu-id="1f538-137">valueJson</span></span>|<span data-ttu-id="1f538-138">String</span><span class="sxs-lookup"><span data-stu-id="1f538-138">String</span></span>|<span data-ttu-id="1f538-139">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f538-139">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f538-140">value</span><span class="sxs-lookup"><span data-stu-id="1f538-140">value</span></span>|<span data-ttu-id="1f538-141">String</span><span class="sxs-lookup"><span data-stu-id="1f538-141">String</span></span>|<span data-ttu-id="1f538-142">字符串值</span><span class="sxs-lookup"><span data-stu-id="1f538-142">The string value</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f538-143">关系</span><span class="sxs-lookup"><span data-stu-id="1f538-143">Relationships</span></span>
<span data-ttu-id="1f538-144">无</span><span class="sxs-lookup"><span data-stu-id="1f538-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f538-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f538-145">JSON Representation</span></span>
<span data-ttu-id="1f538-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f538-146">Here is a JSON representation of the resource.</span></span>
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







