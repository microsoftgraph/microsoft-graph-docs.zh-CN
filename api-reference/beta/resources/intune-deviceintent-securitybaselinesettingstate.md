---
title: securityBaselineSettingState 资源类型
description: 设备设置的安全基准合规性状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562277"
---
# <a name="securitybaselinesettingstate-resource-type"></a><span data-ttu-id="21d52-103">securityBaselineSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="21d52-103">securityBaselineSettingState resource type</span></span>

> <span data-ttu-id="21d52-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21d52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21d52-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21d52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d52-106">设备设置的安全基准合规性状态</span><span class="sxs-lookup"><span data-stu-id="21d52-106">The security baseline compliance state of a setting for a device</span></span>

## <a name="methods"></a><span data-ttu-id="21d52-107">方法</span><span class="sxs-lookup"><span data-stu-id="21d52-107">Methods</span></span>
|<span data-ttu-id="21d52-108">方法</span><span class="sxs-lookup"><span data-stu-id="21d52-108">Method</span></span>|<span data-ttu-id="21d52-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="21d52-109">Return Type</span></span>|<span data-ttu-id="21d52-110">说明</span><span class="sxs-lookup"><span data-stu-id="21d52-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21d52-111">列出 securityBaselineSettingStates</span><span class="sxs-lookup"><span data-stu-id="21d52-111">List securityBaselineSettingStates</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|<span data-ttu-id="21d52-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="21d52-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) collection</span></span>|<span data-ttu-id="21d52-113">列出[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21d52-113">List properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="21d52-114">获取 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="21d52-114">Get securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[<span data-ttu-id="21d52-115">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="21d52-115">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="21d52-116">读取[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21d52-116">Read properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="21d52-117">创建 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="21d52-117">Create securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[<span data-ttu-id="21d52-118">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="21d52-118">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="21d52-119">创建新的[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="21d52-119">Create a new [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="21d52-120">删除 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="21d52-120">Delete securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|<span data-ttu-id="21d52-121">无</span><span class="sxs-lookup"><span data-stu-id="21d52-121">None</span></span>|<span data-ttu-id="21d52-122">删除[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="21d52-122">Deletes a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>|
|[<span data-ttu-id="21d52-123">更新 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="21d52-123">Update securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[<span data-ttu-id="21d52-124">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="21d52-124">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="21d52-125">更新[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="21d52-125">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21d52-126">属性</span><span class="sxs-lookup"><span data-stu-id="21d52-126">Properties</span></span>
|<span data-ttu-id="21d52-127">属性</span><span class="sxs-lookup"><span data-stu-id="21d52-127">Property</span></span>|<span data-ttu-id="21d52-128">类型</span><span class="sxs-lookup"><span data-stu-id="21d52-128">Type</span></span>|<span data-ttu-id="21d52-129">说明</span><span class="sxs-lookup"><span data-stu-id="21d52-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d52-130">id</span><span class="sxs-lookup"><span data-stu-id="21d52-130">id</span></span>|<span data-ttu-id="21d52-131">String</span><span class="sxs-lookup"><span data-stu-id="21d52-131">String</span></span>|<span data-ttu-id="21d52-132">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="21d52-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="21d52-133">settingName</span><span class="sxs-lookup"><span data-stu-id="21d52-133">settingName</span></span>|<span data-ttu-id="21d52-134">String</span><span class="sxs-lookup"><span data-stu-id="21d52-134">String</span></span>|<span data-ttu-id="21d52-135">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="21d52-135">The setting name that is being reported</span></span>|
|<span data-ttu-id="21d52-136">状态</span><span class="sxs-lookup"><span data-stu-id="21d52-136">state</span></span>|[<span data-ttu-id="21d52-137">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="21d52-137">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="21d52-138">安全基准设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="21d52-138">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="21d52-139">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="21d52-139">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="21d52-140">settingCategoryId</span><span class="sxs-lookup"><span data-stu-id="21d52-140">settingCategoryId</span></span>|<span data-ttu-id="21d52-141">String</span><span class="sxs-lookup"><span data-stu-id="21d52-141">String</span></span>|<span data-ttu-id="21d52-142">此设置所属的设置类别 id</span><span class="sxs-lookup"><span data-stu-id="21d52-142">The setting category id which this setting belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="21d52-143">关系</span><span class="sxs-lookup"><span data-stu-id="21d52-143">Relationships</span></span>
<span data-ttu-id="21d52-144">无</span><span class="sxs-lookup"><span data-stu-id="21d52-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21d52-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21d52-145">JSON Representation</span></span>
<span data-ttu-id="21d52-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21d52-146">Here is a JSON representation of the resource.</span></span>
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



