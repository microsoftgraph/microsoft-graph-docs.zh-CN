---
title: securityBaselineState 资源类型
description: 设备的安全基准状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c81a3d351c7c1e854c26e05e32f8426ffdc0631
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524559"
---
# <a name="securitybaselinestate-resource-type"></a><span data-ttu-id="e45dd-103">securityBaselineState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e45dd-103">securityBaselineState resource type</span></span>

> <span data-ttu-id="e45dd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e45dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e45dd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e45dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45dd-106">设备的安全基准状态。</span><span class="sxs-lookup"><span data-stu-id="e45dd-106">Security baseline state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="e45dd-107">方法</span><span class="sxs-lookup"><span data-stu-id="e45dd-107">Methods</span></span>
|<span data-ttu-id="e45dd-108">方法</span><span class="sxs-lookup"><span data-stu-id="e45dd-108">Method</span></span>|<span data-ttu-id="e45dd-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e45dd-109">Return Type</span></span>|<span data-ttu-id="e45dd-110">说明</span><span class="sxs-lookup"><span data-stu-id="e45dd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e45dd-111">列出 securityBaselineStates</span><span class="sxs-lookup"><span data-stu-id="e45dd-111">List securityBaselineStates</span></span>](../api/intune-deviceintent-securitybaselinestate-list.md)|<span data-ttu-id="e45dd-112">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e45dd-112">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) collection</span></span>|<span data-ttu-id="e45dd-113">列出[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e45dd-113">List properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects.</span></span>|
|[<span data-ttu-id="e45dd-114">获取 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e45dd-114">Get securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-get.md)|[<span data-ttu-id="e45dd-115">securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e45dd-115">securityBaselineState</span></span>](../resources/intune-deviceintent-securitybaselinestate.md)|<span data-ttu-id="e45dd-116">读取[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e45dd-116">Read properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>|
|[<span data-ttu-id="e45dd-117">创建 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e45dd-117">Create securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-create.md)|[<span data-ttu-id="e45dd-118">securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e45dd-118">securityBaselineState</span></span>](../resources/intune-deviceintent-securitybaselinestate.md)|<span data-ttu-id="e45dd-119">创建新的[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e45dd-119">Create a new [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>|
|[<span data-ttu-id="e45dd-120">删除 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e45dd-120">Delete securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-delete.md)|<span data-ttu-id="e45dd-121">无</span><span class="sxs-lookup"><span data-stu-id="e45dd-121">None</span></span>|<span data-ttu-id="e45dd-122">删除[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)。</span><span class="sxs-lookup"><span data-stu-id="e45dd-122">Deletes a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>|
|[<span data-ttu-id="e45dd-123">更新 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e45dd-123">Update securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-update.md)|[<span data-ttu-id="e45dd-124">securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e45dd-124">securityBaselineState</span></span>](../resources/intune-deviceintent-securitybaselinestate.md)|<span data-ttu-id="e45dd-125">更新[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e45dd-125">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e45dd-126">属性</span><span class="sxs-lookup"><span data-stu-id="e45dd-126">Properties</span></span>
|<span data-ttu-id="e45dd-127">属性</span><span class="sxs-lookup"><span data-stu-id="e45dd-127">Property</span></span>|<span data-ttu-id="e45dd-128">类型</span><span class="sxs-lookup"><span data-stu-id="e45dd-128">Type</span></span>|<span data-ttu-id="e45dd-129">说明</span><span class="sxs-lookup"><span data-stu-id="e45dd-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45dd-130">id</span><span class="sxs-lookup"><span data-stu-id="e45dd-130">id</span></span>|<span data-ttu-id="e45dd-131">String</span><span class="sxs-lookup"><span data-stu-id="e45dd-131">String</span></span>|<span data-ttu-id="e45dd-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e45dd-132">Key of the entity.</span></span>|
|<span data-ttu-id="e45dd-133">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="e45dd-133">securityBaselineTemplateId</span></span>|<span data-ttu-id="e45dd-134">String</span><span class="sxs-lookup"><span data-stu-id="e45dd-134">String</span></span>|<span data-ttu-id="e45dd-135">安全基准模板 id</span><span class="sxs-lookup"><span data-stu-id="e45dd-135">The security baseline template id</span></span>|
|<span data-ttu-id="e45dd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e45dd-136">displayName</span></span>|<span data-ttu-id="e45dd-137">String</span><span class="sxs-lookup"><span data-stu-id="e45dd-137">String</span></span>|<span data-ttu-id="e45dd-138">安全基准的显示名称</span><span class="sxs-lookup"><span data-stu-id="e45dd-138">The display name of the security baseline</span></span>|

## <a name="relationships"></a><span data-ttu-id="e45dd-139">关系</span><span class="sxs-lookup"><span data-stu-id="e45dd-139">Relationships</span></span>
|<span data-ttu-id="e45dd-140">关系</span><span class="sxs-lookup"><span data-stu-id="e45dd-140">Relationship</span></span>|<span data-ttu-id="e45dd-141">类型</span><span class="sxs-lookup"><span data-stu-id="e45dd-141">Type</span></span>|<span data-ttu-id="e45dd-142">说明</span><span class="sxs-lookup"><span data-stu-id="e45dd-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45dd-143">settingStates</span><span class="sxs-lookup"><span data-stu-id="e45dd-143">settingStates</span></span>|<span data-ttu-id="e45dd-144">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e45dd-144">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) collection</span></span>|<span data-ttu-id="e45dd-145">设备的不同设置的安全基准状态</span><span class="sxs-lookup"><span data-stu-id="e45dd-145">The security baseline state for different settings for a device</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e45dd-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e45dd-146">JSON Representation</span></span>
<span data-ttu-id="e45dd-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e45dd-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "String (identifier)",
  "securityBaselineTemplateId": "String",
  "displayName": "String"
}
```



