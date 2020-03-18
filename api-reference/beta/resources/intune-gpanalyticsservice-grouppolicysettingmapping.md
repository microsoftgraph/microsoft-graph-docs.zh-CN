---
title: groupPolicySettingMapping 资源类型
description: MDM/Intune 映射的组策略设置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83c3f827bcd7ed9bf5a0fa7fcf863c1d585e4342
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783156"
---
# <a name="grouppolicysettingmapping-resource-type"></a><span data-ttu-id="17549-103">groupPolicySettingMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="17549-103">groupPolicySettingMapping resource type</span></span>

> <span data-ttu-id="17549-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17549-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17549-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17549-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17549-106">MDM/Intune 映射的组策略设置。</span><span class="sxs-lookup"><span data-stu-id="17549-106">The Group Policy setting to MDM/Intune mapping.</span></span>

## <a name="methods"></a><span data-ttu-id="17549-107">方法</span><span class="sxs-lookup"><span data-stu-id="17549-107">Methods</span></span>
|<span data-ttu-id="17549-108">方法</span><span class="sxs-lookup"><span data-stu-id="17549-108">Method</span></span>|<span data-ttu-id="17549-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="17549-109">Return Type</span></span>|<span data-ttu-id="17549-110">说明</span><span class="sxs-lookup"><span data-stu-id="17549-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17549-111">列出 groupPolicySettingMappings</span><span class="sxs-lookup"><span data-stu-id="17549-111">List groupPolicySettingMappings</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|<span data-ttu-id="17549-112">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)集合</span><span class="sxs-lookup"><span data-stu-id="17549-112">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) collection</span></span>|<span data-ttu-id="17549-113">列出[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17549-113">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>|
|[<span data-ttu-id="17549-114">获取 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="17549-114">Get groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[<span data-ttu-id="17549-115">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="17549-115">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="17549-116">读取[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17549-116">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="17549-117">创建 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="17549-117">Create groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[<span data-ttu-id="17549-118">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="17549-118">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="17549-119">创建新的[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17549-119">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="17549-120">删除 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="17549-120">Delete groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|<span data-ttu-id="17549-121">None</span><span class="sxs-lookup"><span data-stu-id="17549-121">None</span></span>|<span data-ttu-id="17549-122">删除[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。</span><span class="sxs-lookup"><span data-stu-id="17549-122">Deletes a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>|
|[<span data-ttu-id="17549-123">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="17549-123">Update groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[<span data-ttu-id="17549-124">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="17549-124">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="17549-125">更新[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17549-125">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="17549-126">属性</span><span class="sxs-lookup"><span data-stu-id="17549-126">Properties</span></span>
|<span data-ttu-id="17549-127">属性</span><span class="sxs-lookup"><span data-stu-id="17549-127">Property</span></span>|<span data-ttu-id="17549-128">类型</span><span class="sxs-lookup"><span data-stu-id="17549-128">Type</span></span>|<span data-ttu-id="17549-129">说明</span><span class="sxs-lookup"><span data-stu-id="17549-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17549-130">id</span><span class="sxs-lookup"><span data-stu-id="17549-130">id</span></span>|<span data-ttu-id="17549-131">String</span><span class="sxs-lookup"><span data-stu-id="17549-131">String</span></span>|<span data-ttu-id="17549-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="17549-132">Not yet documented</span></span>|
|<span data-ttu-id="17549-133">parentId</span><span class="sxs-lookup"><span data-stu-id="17549-133">parentId</span></span>|<span data-ttu-id="17549-134">String</span><span class="sxs-lookup"><span data-stu-id="17549-134">String</span></span>|<span data-ttu-id="17549-135">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="17549-135">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="17549-136">childIdList</span><span class="sxs-lookup"><span data-stu-id="17549-136">childIdList</span></span>|<span data-ttu-id="17549-137">String collection</span><span class="sxs-lookup"><span data-stu-id="17549-137">String collection</span></span>|<span data-ttu-id="17549-138">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="17549-138">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="17549-139">settingName</span><span class="sxs-lookup"><span data-stu-id="17549-139">settingName</span></span>|<span data-ttu-id="17549-140">String</span><span class="sxs-lookup"><span data-stu-id="17549-140">String</span></span>|<span data-ttu-id="17549-141">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="17549-141">The name of this group policy setting.</span></span>|
|<span data-ttu-id="17549-142">settingValue</span><span class="sxs-lookup"><span data-stu-id="17549-142">settingValue</span></span>|<span data-ttu-id="17549-143">String</span><span class="sxs-lookup"><span data-stu-id="17549-143">String</span></span>|<span data-ttu-id="17549-144">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="17549-144">The value of this group policy setting.</span></span>|
|<span data-ttu-id="17549-145">settingValueType</span><span class="sxs-lookup"><span data-stu-id="17549-145">settingValueType</span></span>|<span data-ttu-id="17549-146">String</span><span class="sxs-lookup"><span data-stu-id="17549-146">String</span></span>|<span data-ttu-id="17549-147">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="17549-147">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="17549-148">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="17549-148">settingDisplayName</span></span>|<span data-ttu-id="17549-149">String</span><span class="sxs-lookup"><span data-stu-id="17549-149">String</span></span>|<span data-ttu-id="17549-150">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="17549-150">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="17549-151">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="17549-151">settingDisplayValue</span></span>|<span data-ttu-id="17549-152">String</span><span class="sxs-lookup"><span data-stu-id="17549-152">String</span></span>|<span data-ttu-id="17549-153">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="17549-153">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="17549-154">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="17549-154">settingDisplayValueType</span></span>|<span data-ttu-id="17549-155">String</span><span class="sxs-lookup"><span data-stu-id="17549-155">String</span></span>|<span data-ttu-id="17549-156">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="17549-156">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="17549-157">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="17549-157">settingValueDisplayUnits</span></span>|<span data-ttu-id="17549-158">String</span><span class="sxs-lookup"><span data-stu-id="17549-158">String</span></span>|<span data-ttu-id="17549-159">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="17549-159">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="17549-160">settingCategory</span><span class="sxs-lookup"><span data-stu-id="17549-160">settingCategory</span></span>|<span data-ttu-id="17549-161">String</span><span class="sxs-lookup"><span data-stu-id="17549-161">String</span></span>|<span data-ttu-id="17549-162">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="17549-162">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="17549-163">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="17549-163">mdmCspName</span></span>|<span data-ttu-id="17549-164">String</span><span class="sxs-lookup"><span data-stu-id="17549-164">String</span></span>|<span data-ttu-id="17549-165">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="17549-165">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="17549-166">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="17549-166">mdmSettingUri</span></span>|<span data-ttu-id="17549-167">String</span><span class="sxs-lookup"><span data-stu-id="17549-167">String</span></span>|<span data-ttu-id="17549-168">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="17549-168">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="17549-169">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="17549-169">mdmMinimumOSVersion</span></span>|<span data-ttu-id="17549-170">Int32</span><span class="sxs-lookup"><span data-stu-id="17549-170">Int32</span></span>|<span data-ttu-id="17549-171">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="17549-171">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="17549-172">settingType</span><span class="sxs-lookup"><span data-stu-id="17549-172">settingType</span></span>|[<span data-ttu-id="17549-173">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="17549-173">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="17549-174">组策略的设置类型（安全性或 admx）。</span><span class="sxs-lookup"><span data-stu-id="17549-174">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="17549-175">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="17549-175">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="17549-176">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="17549-176">isMdmSupported</span></span>|<span data-ttu-id="17549-177">布尔值</span><span class="sxs-lookup"><span data-stu-id="17549-177">Boolean</span></span>|<span data-ttu-id="17549-178">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="17549-178">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="17549-179">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="17549-179">mdmSupportedState</span></span>|[<span data-ttu-id="17549-180">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="17549-180">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="17549-181">指示是否支持 Mdm 中的设置。</span><span class="sxs-lookup"><span data-stu-id="17549-181">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="17549-182">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="17549-182">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="17549-183">settingScope</span><span class="sxs-lookup"><span data-stu-id="17549-183">settingScope</span></span>|[<span data-ttu-id="17549-184">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="17549-184">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="17549-185">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="17549-185">The scope of the setting.</span></span> <span data-ttu-id="17549-186">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="17549-186">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="17549-187">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="17549-187">intuneSettingUriList</span></span>|<span data-ttu-id="17549-188">String collection</span><span class="sxs-lookup"><span data-stu-id="17549-188">String collection</span></span>|<span data-ttu-id="17549-189">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="17549-189">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="17549-190">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="17549-190">intuneSettingDefinitionId</span></span>|<span data-ttu-id="17549-191">String</span><span class="sxs-lookup"><span data-stu-id="17549-191">String</span></span>|<span data-ttu-id="17549-192">Intune 设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="17549-192">The Intune Setting Definition Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="17549-193">关系</span><span class="sxs-lookup"><span data-stu-id="17549-193">Relationships</span></span>
<span data-ttu-id="17549-194">无</span><span class="sxs-lookup"><span data-stu-id="17549-194">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17549-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17549-195">JSON Representation</span></span>
<span data-ttu-id="17549-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17549-196">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicySettingMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "String (identifier)",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": 1024,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String"
}
```



