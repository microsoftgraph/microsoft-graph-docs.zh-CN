---
title: groupPolicySettingMapping 资源类型
description: MDM/Intune 映射的组策略设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d6d513f16debcec4c636101591e966eef58cd260
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528136"
---
# <a name="grouppolicysettingmapping-resource-type"></a><span data-ttu-id="200b0-103">groupPolicySettingMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="200b0-103">groupPolicySettingMapping resource type</span></span>

<span data-ttu-id="200b0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="200b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="200b0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="200b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="200b0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="200b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="200b0-107">MDM/Intune 映射的组策略设置。</span><span class="sxs-lookup"><span data-stu-id="200b0-107">The Group Policy setting to MDM/Intune mapping.</span></span>

## <a name="methods"></a><span data-ttu-id="200b0-108">方法</span><span class="sxs-lookup"><span data-stu-id="200b0-108">Methods</span></span>
|<span data-ttu-id="200b0-109">方法</span><span class="sxs-lookup"><span data-stu-id="200b0-109">Method</span></span>|<span data-ttu-id="200b0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="200b0-110">Return Type</span></span>|<span data-ttu-id="200b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="200b0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="200b0-112">列出 groupPolicySettingMappings</span><span class="sxs-lookup"><span data-stu-id="200b0-112">List groupPolicySettingMappings</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|<span data-ttu-id="200b0-113">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)集合</span><span class="sxs-lookup"><span data-stu-id="200b0-113">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) collection</span></span>|<span data-ttu-id="200b0-114">列出[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="200b0-114">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>|
|[<span data-ttu-id="200b0-115">获取 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="200b0-115">Get groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[<span data-ttu-id="200b0-116">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="200b0-116">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="200b0-117">读取[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="200b0-117">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="200b0-118">创建 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="200b0-118">Create groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[<span data-ttu-id="200b0-119">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="200b0-119">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="200b0-120">创建新的[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象。</span><span class="sxs-lookup"><span data-stu-id="200b0-120">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="200b0-121">删除 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="200b0-121">Delete groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|<span data-ttu-id="200b0-122">无</span><span class="sxs-lookup"><span data-stu-id="200b0-122">None</span></span>|<span data-ttu-id="200b0-123">删除[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。</span><span class="sxs-lookup"><span data-stu-id="200b0-123">Deletes a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>|
|[<span data-ttu-id="200b0-124">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="200b0-124">Update groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[<span data-ttu-id="200b0-125">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="200b0-125">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="200b0-126">更新[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="200b0-126">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="200b0-127">属性</span><span class="sxs-lookup"><span data-stu-id="200b0-127">Properties</span></span>
|<span data-ttu-id="200b0-128">属性</span><span class="sxs-lookup"><span data-stu-id="200b0-128">Property</span></span>|<span data-ttu-id="200b0-129">类型</span><span class="sxs-lookup"><span data-stu-id="200b0-129">Type</span></span>|<span data-ttu-id="200b0-130">说明</span><span class="sxs-lookup"><span data-stu-id="200b0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="200b0-131">id</span><span class="sxs-lookup"><span data-stu-id="200b0-131">id</span></span>|<span data-ttu-id="200b0-132">String</span><span class="sxs-lookup"><span data-stu-id="200b0-132">String</span></span>|<span data-ttu-id="200b0-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="200b0-133">Not yet documented</span></span>|
|<span data-ttu-id="200b0-134">parentId</span><span class="sxs-lookup"><span data-stu-id="200b0-134">parentId</span></span>|<span data-ttu-id="200b0-135">String</span><span class="sxs-lookup"><span data-stu-id="200b0-135">String</span></span>|<span data-ttu-id="200b0-136">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="200b0-136">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="200b0-137">childIdList</span><span class="sxs-lookup"><span data-stu-id="200b0-137">childIdList</span></span>|<span data-ttu-id="200b0-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="200b0-138">String collection</span></span>|<span data-ttu-id="200b0-139">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="200b0-139">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="200b0-140">settingName</span><span class="sxs-lookup"><span data-stu-id="200b0-140">settingName</span></span>|<span data-ttu-id="200b0-141">String</span><span class="sxs-lookup"><span data-stu-id="200b0-141">String</span></span>|<span data-ttu-id="200b0-142">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="200b0-142">The name of this group policy setting.</span></span>|
|<span data-ttu-id="200b0-143">settingValue</span><span class="sxs-lookup"><span data-stu-id="200b0-143">settingValue</span></span>|<span data-ttu-id="200b0-144">String</span><span class="sxs-lookup"><span data-stu-id="200b0-144">String</span></span>|<span data-ttu-id="200b0-145">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="200b0-145">The value of this group policy setting.</span></span>|
|<span data-ttu-id="200b0-146">settingValueType</span><span class="sxs-lookup"><span data-stu-id="200b0-146">settingValueType</span></span>|<span data-ttu-id="200b0-147">String</span><span class="sxs-lookup"><span data-stu-id="200b0-147">String</span></span>|<span data-ttu-id="200b0-148">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="200b0-148">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="200b0-149">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="200b0-149">settingDisplayName</span></span>|<span data-ttu-id="200b0-150">String</span><span class="sxs-lookup"><span data-stu-id="200b0-150">String</span></span>|<span data-ttu-id="200b0-151">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="200b0-151">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="200b0-152">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="200b0-152">settingDisplayValue</span></span>|<span data-ttu-id="200b0-153">String</span><span class="sxs-lookup"><span data-stu-id="200b0-153">String</span></span>|<span data-ttu-id="200b0-154">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="200b0-154">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="200b0-155">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="200b0-155">settingDisplayValueType</span></span>|<span data-ttu-id="200b0-156">String</span><span class="sxs-lookup"><span data-stu-id="200b0-156">String</span></span>|<span data-ttu-id="200b0-157">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="200b0-157">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="200b0-158">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="200b0-158">settingValueDisplayUnits</span></span>|<span data-ttu-id="200b0-159">String</span><span class="sxs-lookup"><span data-stu-id="200b0-159">String</span></span>|<span data-ttu-id="200b0-160">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="200b0-160">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="200b0-161">settingCategory</span><span class="sxs-lookup"><span data-stu-id="200b0-161">settingCategory</span></span>|<span data-ttu-id="200b0-162">String</span><span class="sxs-lookup"><span data-stu-id="200b0-162">String</span></span>|<span data-ttu-id="200b0-163">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="200b0-163">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="200b0-164">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="200b0-164">mdmCspName</span></span>|<span data-ttu-id="200b0-165">String</span><span class="sxs-lookup"><span data-stu-id="200b0-165">String</span></span>|<span data-ttu-id="200b0-166">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="200b0-166">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="200b0-167">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="200b0-167">mdmSettingUri</span></span>|<span data-ttu-id="200b0-168">String</span><span class="sxs-lookup"><span data-stu-id="200b0-168">String</span></span>|<span data-ttu-id="200b0-169">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="200b0-169">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="200b0-170">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="200b0-170">mdmMinimumOSVersion</span></span>|<span data-ttu-id="200b0-171">Int32</span><span class="sxs-lookup"><span data-stu-id="200b0-171">Int32</span></span>|<span data-ttu-id="200b0-172">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="200b0-172">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="200b0-173">settingType</span><span class="sxs-lookup"><span data-stu-id="200b0-173">settingType</span></span>|[<span data-ttu-id="200b0-174">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="200b0-174">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="200b0-175">组策略的设置类型（安全性或 admx）。</span><span class="sxs-lookup"><span data-stu-id="200b0-175">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="200b0-176">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="200b0-176">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="200b0-177">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="200b0-177">isMdmSupported</span></span>|<span data-ttu-id="200b0-178">布尔</span><span class="sxs-lookup"><span data-stu-id="200b0-178">Boolean</span></span>|<span data-ttu-id="200b0-179">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="200b0-179">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="200b0-180">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="200b0-180">mdmSupportedState</span></span>|[<span data-ttu-id="200b0-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="200b0-181">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="200b0-182">指示是否支持 Mdm 中的设置。</span><span class="sxs-lookup"><span data-stu-id="200b0-182">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="200b0-183">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="200b0-183">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="200b0-184">settingScope</span><span class="sxs-lookup"><span data-stu-id="200b0-184">settingScope</span></span>|[<span data-ttu-id="200b0-185">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="200b0-185">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="200b0-186">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="200b0-186">The scope of the setting.</span></span> <span data-ttu-id="200b0-187">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="200b0-187">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="200b0-188">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="200b0-188">intuneSettingUriList</span></span>|<span data-ttu-id="200b0-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="200b0-189">String collection</span></span>|<span data-ttu-id="200b0-190">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="200b0-190">The list of Intune Setting URIs this group policy setting maps to</span></span>|

## <a name="relationships"></a><span data-ttu-id="200b0-191">关系</span><span class="sxs-lookup"><span data-stu-id="200b0-191">Relationships</span></span>
<span data-ttu-id="200b0-192">无</span><span class="sxs-lookup"><span data-stu-id="200b0-192">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="200b0-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="200b0-193">JSON Representation</span></span>
<span data-ttu-id="200b0-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="200b0-194">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```



