---
title: groupPolicySettingMapping 资源类型
description: MDM/Intune 映射的组策略设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d507687e6a14e276a177a5795afa55aa5fe3f051
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697474"
---
# <a name="grouppolicysettingmapping-resource-type"></a><span data-ttu-id="7c0c8-103">groupPolicySettingMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c0c8-103">groupPolicySettingMapping resource type</span></span>

<span data-ttu-id="7c0c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c0c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c0c8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c0c8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c0c8-107">MDM/Intune 映射的组策略设置。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-107">The Group Policy setting to MDM/Intune mapping.</span></span>

## <a name="methods"></a><span data-ttu-id="7c0c8-108">Methods</span><span class="sxs-lookup"><span data-stu-id="7c0c8-108">Methods</span></span>
|<span data-ttu-id="7c0c8-109">方法</span><span class="sxs-lookup"><span data-stu-id="7c0c8-109">Method</span></span>|<span data-ttu-id="7c0c8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c0c8-110">Return Type</span></span>|<span data-ttu-id="7c0c8-111">说明</span><span class="sxs-lookup"><span data-stu-id="7c0c8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7c0c8-112">列出 groupPolicySettingMappings</span><span class="sxs-lookup"><span data-stu-id="7c0c8-112">List groupPolicySettingMappings</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|<span data-ttu-id="7c0c8-113">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c0c8-113">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) collection</span></span>|<span data-ttu-id="7c0c8-114">列出 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-114">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>|
|[<span data-ttu-id="7c0c8-115">获取 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="7c0c8-115">Get groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[<span data-ttu-id="7c0c8-116">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="7c0c8-116">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="7c0c8-117">读取 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-117">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="7c0c8-118">创建 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="7c0c8-118">Create groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[<span data-ttu-id="7c0c8-119">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="7c0c8-119">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="7c0c8-120">创建新的 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-120">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="7c0c8-121">删除 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="7c0c8-121">Delete groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|<span data-ttu-id="7c0c8-122">无</span><span class="sxs-lookup"><span data-stu-id="7c0c8-122">None</span></span>|<span data-ttu-id="7c0c8-123">删除 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-123">Deletes a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>|
|[<span data-ttu-id="7c0c8-124">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="7c0c8-124">Update groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[<span data-ttu-id="7c0c8-125">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="7c0c8-125">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="7c0c8-126">更新 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-126">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c0c8-127">属性</span><span class="sxs-lookup"><span data-stu-id="7c0c8-127">Properties</span></span>
|<span data-ttu-id="7c0c8-128">属性</span><span class="sxs-lookup"><span data-stu-id="7c0c8-128">Property</span></span>|<span data-ttu-id="7c0c8-129">类型</span><span class="sxs-lookup"><span data-stu-id="7c0c8-129">Type</span></span>|<span data-ttu-id="7c0c8-130">说明</span><span class="sxs-lookup"><span data-stu-id="7c0c8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0c8-131">id</span><span class="sxs-lookup"><span data-stu-id="7c0c8-131">id</span></span>|<span data-ttu-id="7c0c8-132">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-132">String</span></span>|<span data-ttu-id="7c0c8-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7c0c8-133">Not yet documented</span></span>|
|<span data-ttu-id="7c0c8-134">parentId</span><span class="sxs-lookup"><span data-stu-id="7c0c8-134">parentId</span></span>|<span data-ttu-id="7c0c8-135">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-135">String</span></span>|<span data-ttu-id="7c0c8-136">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-136">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-137">childIdList</span><span class="sxs-lookup"><span data-stu-id="7c0c8-137">childIdList</span></span>|<span data-ttu-id="7c0c8-138">String collection</span><span class="sxs-lookup"><span data-stu-id="7c0c8-138">String collection</span></span>|<span data-ttu-id="7c0c8-139">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-139">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-140">settingName</span><span class="sxs-lookup"><span data-stu-id="7c0c8-140">settingName</span></span>|<span data-ttu-id="7c0c8-141">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-141">String</span></span>|<span data-ttu-id="7c0c8-142">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-142">The name of this group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-143">settingValue</span><span class="sxs-lookup"><span data-stu-id="7c0c8-143">settingValue</span></span>|<span data-ttu-id="7c0c8-144">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-144">String</span></span>|<span data-ttu-id="7c0c8-145">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-145">The value of this group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-146">settingValueType</span><span class="sxs-lookup"><span data-stu-id="7c0c8-146">settingValueType</span></span>|<span data-ttu-id="7c0c8-147">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-147">String</span></span>|<span data-ttu-id="7c0c8-148">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-148">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-149">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="7c0c8-149">settingDisplayName</span></span>|<span data-ttu-id="7c0c8-150">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-150">String</span></span>|<span data-ttu-id="7c0c8-151">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-151">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-152">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="7c0c8-152">settingDisplayValue</span></span>|<span data-ttu-id="7c0c8-153">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-153">String</span></span>|<span data-ttu-id="7c0c8-154">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-154">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-155">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="7c0c8-155">settingDisplayValueType</span></span>|<span data-ttu-id="7c0c8-156">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-156">String</span></span>|<span data-ttu-id="7c0c8-157">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-157">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="7c0c8-158">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="7c0c8-158">settingValueDisplayUnits</span></span>|<span data-ttu-id="7c0c8-159">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-159">String</span></span>|<span data-ttu-id="7c0c8-160">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="7c0c8-160">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="7c0c8-161">settingCategory</span><span class="sxs-lookup"><span data-stu-id="7c0c8-161">settingCategory</span></span>|<span data-ttu-id="7c0c8-162">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-162">String</span></span>|<span data-ttu-id="7c0c8-163">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-163">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="7c0c8-164">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="7c0c8-164">mdmCspName</span></span>|<span data-ttu-id="7c0c8-165">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-165">String</span></span>|<span data-ttu-id="7c0c8-166">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-166">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="7c0c8-167">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="7c0c8-167">mdmSettingUri</span></span>|<span data-ttu-id="7c0c8-168">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-168">String</span></span>|<span data-ttu-id="7c0c8-169">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-169">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="7c0c8-170">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="7c0c8-170">mdmMinimumOSVersion</span></span>|<span data-ttu-id="7c0c8-171">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0c8-171">Int32</span></span>|<span data-ttu-id="7c0c8-172">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-172">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="7c0c8-173">settingType</span><span class="sxs-lookup"><span data-stu-id="7c0c8-173">settingType</span></span>|[<span data-ttu-id="7c0c8-174">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="7c0c8-174">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="7c0c8-175">组策略的设置类型 (安全性或 admx) 。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-175">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="7c0c8-176">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-176">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="7c0c8-177">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="7c0c8-177">isMdmSupported</span></span>|<span data-ttu-id="7c0c8-178">布尔</span><span class="sxs-lookup"><span data-stu-id="7c0c8-178">Boolean</span></span>|<span data-ttu-id="7c0c8-179">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="7c0c8-179">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="7c0c8-180">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="7c0c8-180">mdmSupportedState</span></span>|[<span data-ttu-id="7c0c8-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="7c0c8-181">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="7c0c8-182">指示是否支持 Mdm 中的设置。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-182">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="7c0c8-183">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-183">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="7c0c8-184">settingScope</span><span class="sxs-lookup"><span data-stu-id="7c0c8-184">settingScope</span></span>|[<span data-ttu-id="7c0c8-185">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="7c0c8-185">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="7c0c8-186">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-186">The scope of the setting.</span></span> <span data-ttu-id="7c0c8-187">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-187">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="7c0c8-188">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="7c0c8-188">intuneSettingUriList</span></span>|<span data-ttu-id="7c0c8-189">String collection</span><span class="sxs-lookup"><span data-stu-id="7c0c8-189">String collection</span></span>|<span data-ttu-id="7c0c8-190">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="7c0c8-190">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="7c0c8-191">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7c0c8-191">intuneSettingDefinitionId</span></span>|<span data-ttu-id="7c0c8-192">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-192">String</span></span>|<span data-ttu-id="7c0c8-193">Intune 设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="7c0c8-193">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="7c0c8-194">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7c0c8-194">admxSettingDefinitionId</span></span>|<span data-ttu-id="7c0c8-195">String</span><span class="sxs-lookup"><span data-stu-id="7c0c8-195">String</span></span>|<span data-ttu-id="7c0c8-196">Admx 组策略 Id</span><span class="sxs-lookup"><span data-stu-id="7c0c8-196">Admx Group Policy Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c0c8-197">关系</span><span class="sxs-lookup"><span data-stu-id="7c0c8-197">Relationships</span></span>
<span data-ttu-id="7c0c8-198">无</span><span class="sxs-lookup"><span data-stu-id="7c0c8-198">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c0c8-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c0c8-199">JSON Representation</span></span>
<span data-ttu-id="7c0c8-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-200">Here is a JSON representation of the resource.</span></span>
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
  "intuneSettingDefinitionId": "String",
  "admxSettingDefinitionId": "String"
}
```





