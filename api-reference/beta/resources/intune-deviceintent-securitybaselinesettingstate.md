---
title: securityBaselineSettingState 资源类型
description: 设备设置的安全基准合规性状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522578"
---
# <a name="securitybaselinesettingstate-resource-type"></a><span data-ttu-id="b427b-103">securityBaselineSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b427b-103">securityBaselineSettingState resource type</span></span>

> <span data-ttu-id="b427b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b427b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b427b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b427b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b427b-106">设备设置的安全基准合规性状态</span><span class="sxs-lookup"><span data-stu-id="b427b-106">The security baseline compliance state of a setting for a device</span></span>

## <a name="methods"></a><span data-ttu-id="b427b-107">方法</span><span class="sxs-lookup"><span data-stu-id="b427b-107">Methods</span></span>
|<span data-ttu-id="b427b-108">方法</span><span class="sxs-lookup"><span data-stu-id="b427b-108">Method</span></span>|<span data-ttu-id="b427b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b427b-109">Return Type</span></span>|<span data-ttu-id="b427b-110">说明</span><span class="sxs-lookup"><span data-stu-id="b427b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b427b-111">列出 securityBaselineSettingStates</span><span class="sxs-lookup"><span data-stu-id="b427b-111">List securityBaselineSettingStates</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|<span data-ttu-id="b427b-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="b427b-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) collection</span></span>|<span data-ttu-id="b427b-113">列出[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b427b-113">List properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="b427b-114">获取 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="b427b-114">Get securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[<span data-ttu-id="b427b-115">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="b427b-115">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="b427b-116">读取[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b427b-116">Read properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="b427b-117">创建 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="b427b-117">Create securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[<span data-ttu-id="b427b-118">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="b427b-118">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="b427b-119">创建新的[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b427b-119">Create a new [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="b427b-120">删除 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="b427b-120">Delete securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|<span data-ttu-id="b427b-121">无</span><span class="sxs-lookup"><span data-stu-id="b427b-121">None</span></span>|<span data-ttu-id="b427b-122">删除[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="b427b-122">Deletes a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>|
|[<span data-ttu-id="b427b-123">更新 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="b427b-123">Update securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[<span data-ttu-id="b427b-124">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="b427b-124">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="b427b-125">更新[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b427b-125">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b427b-126">属性</span><span class="sxs-lookup"><span data-stu-id="b427b-126">Properties</span></span>
|<span data-ttu-id="b427b-127">属性</span><span class="sxs-lookup"><span data-stu-id="b427b-127">Property</span></span>|<span data-ttu-id="b427b-128">类型</span><span class="sxs-lookup"><span data-stu-id="b427b-128">Type</span></span>|<span data-ttu-id="b427b-129">说明</span><span class="sxs-lookup"><span data-stu-id="b427b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b427b-130">id</span><span class="sxs-lookup"><span data-stu-id="b427b-130">id</span></span>|<span data-ttu-id="b427b-131">String</span><span class="sxs-lookup"><span data-stu-id="b427b-131">String</span></span>|<span data-ttu-id="b427b-132">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b427b-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="b427b-133">settingName</span><span class="sxs-lookup"><span data-stu-id="b427b-133">settingName</span></span>|<span data-ttu-id="b427b-134">String</span><span class="sxs-lookup"><span data-stu-id="b427b-134">String</span></span>|<span data-ttu-id="b427b-135">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="b427b-135">The setting name that is being reported</span></span>|
|<span data-ttu-id="b427b-136">state</span><span class="sxs-lookup"><span data-stu-id="b427b-136">state</span></span>|[<span data-ttu-id="b427b-137">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="b427b-137">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="b427b-138">安全基准设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="b427b-138">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="b427b-139">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="b427b-139">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="b427b-140">settingCategoryId</span><span class="sxs-lookup"><span data-stu-id="b427b-140">settingCategoryId</span></span>|<span data-ttu-id="b427b-141">String</span><span class="sxs-lookup"><span data-stu-id="b427b-141">String</span></span>|<span data-ttu-id="b427b-142">此设置所属的设置类别 id</span><span class="sxs-lookup"><span data-stu-id="b427b-142">The setting category id which this setting belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="b427b-143">关系</span><span class="sxs-lookup"><span data-stu-id="b427b-143">Relationships</span></span>
<span data-ttu-id="b427b-144">无</span><span class="sxs-lookup"><span data-stu-id="b427b-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b427b-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b427b-145">JSON Representation</span></span>
<span data-ttu-id="b427b-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b427b-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```



