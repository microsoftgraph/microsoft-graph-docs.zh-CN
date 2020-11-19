---
title: groupPolicySettingMapping 资源类型
description: MDM/Intune 映射的组策略设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db235993f9ddb87c11407136676608ab8d1c1992
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298650"
---
# <a name="grouppolicysettingmapping-resource-type"></a><span data-ttu-id="755ad-103">groupPolicySettingMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="755ad-103">groupPolicySettingMapping resource type</span></span>

<span data-ttu-id="755ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="755ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="755ad-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="755ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="755ad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="755ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="755ad-107">MDM/Intune 映射的组策略设置。</span><span class="sxs-lookup"><span data-stu-id="755ad-107">The Group Policy setting to MDM/Intune mapping.</span></span>

## <a name="methods"></a><span data-ttu-id="755ad-108">Methods</span><span class="sxs-lookup"><span data-stu-id="755ad-108">Methods</span></span>
|<span data-ttu-id="755ad-109">方法</span><span class="sxs-lookup"><span data-stu-id="755ad-109">Method</span></span>|<span data-ttu-id="755ad-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="755ad-110">Return Type</span></span>|<span data-ttu-id="755ad-111">Description</span><span class="sxs-lookup"><span data-stu-id="755ad-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="755ad-112">列出 groupPolicySettingMappings</span><span class="sxs-lookup"><span data-stu-id="755ad-112">List groupPolicySettingMappings</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|<span data-ttu-id="755ad-113">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 集合</span><span class="sxs-lookup"><span data-stu-id="755ad-113">[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) collection</span></span>|<span data-ttu-id="755ad-114">列出 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="755ad-114">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>|
|[<span data-ttu-id="755ad-115">获取 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="755ad-115">Get groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[<span data-ttu-id="755ad-116">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="755ad-116">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="755ad-117">读取 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="755ad-117">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="755ad-118">创建 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="755ad-118">Create groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[<span data-ttu-id="755ad-119">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="755ad-119">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="755ad-120">创建新的 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="755ad-120">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|
|[<span data-ttu-id="755ad-121">删除 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="755ad-121">Delete groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|<span data-ttu-id="755ad-122">无</span><span class="sxs-lookup"><span data-stu-id="755ad-122">None</span></span>|<span data-ttu-id="755ad-123">删除 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。</span><span class="sxs-lookup"><span data-stu-id="755ad-123">Deletes a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>|
|[<span data-ttu-id="755ad-124">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="755ad-124">Update groupPolicySettingMapping</span></span>](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[<span data-ttu-id="755ad-125">groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="755ad-125">groupPolicySettingMapping</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|<span data-ttu-id="755ad-126">更新 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="755ad-126">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="755ad-127">属性</span><span class="sxs-lookup"><span data-stu-id="755ad-127">Properties</span></span>
|<span data-ttu-id="755ad-128">属性</span><span class="sxs-lookup"><span data-stu-id="755ad-128">Property</span></span>|<span data-ttu-id="755ad-129">类型</span><span class="sxs-lookup"><span data-stu-id="755ad-129">Type</span></span>|<span data-ttu-id="755ad-130">说明</span><span class="sxs-lookup"><span data-stu-id="755ad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="755ad-131">id</span><span class="sxs-lookup"><span data-stu-id="755ad-131">id</span></span>|<span data-ttu-id="755ad-132">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-132">String</span></span>|<span data-ttu-id="755ad-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="755ad-133">Not yet documented</span></span>|
|<span data-ttu-id="755ad-134">parentId</span><span class="sxs-lookup"><span data-stu-id="755ad-134">parentId</span></span>|<span data-ttu-id="755ad-135">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-135">String</span></span>|<span data-ttu-id="755ad-136">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="755ad-136">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="755ad-137">childIdList</span><span class="sxs-lookup"><span data-stu-id="755ad-137">childIdList</span></span>|<span data-ttu-id="755ad-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="755ad-138">String collection</span></span>|<span data-ttu-id="755ad-139">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="755ad-139">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="755ad-140">settingName</span><span class="sxs-lookup"><span data-stu-id="755ad-140">settingName</span></span>|<span data-ttu-id="755ad-141">String</span><span class="sxs-lookup"><span data-stu-id="755ad-141">String</span></span>|<span data-ttu-id="755ad-142">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="755ad-142">The name of this group policy setting.</span></span>|
|<span data-ttu-id="755ad-143">settingValue</span><span class="sxs-lookup"><span data-stu-id="755ad-143">settingValue</span></span>|<span data-ttu-id="755ad-144">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-144">String</span></span>|<span data-ttu-id="755ad-145">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="755ad-145">The value of this group policy setting.</span></span>|
|<span data-ttu-id="755ad-146">settingValueType</span><span class="sxs-lookup"><span data-stu-id="755ad-146">settingValueType</span></span>|<span data-ttu-id="755ad-147">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-147">String</span></span>|<span data-ttu-id="755ad-148">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="755ad-148">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="755ad-149">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="755ad-149">settingDisplayName</span></span>|<span data-ttu-id="755ad-150">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-150">String</span></span>|<span data-ttu-id="755ad-151">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="755ad-151">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="755ad-152">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="755ad-152">settingDisplayValue</span></span>|<span data-ttu-id="755ad-153">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-153">String</span></span>|<span data-ttu-id="755ad-154">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="755ad-154">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="755ad-155">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="755ad-155">settingDisplayValueType</span></span>|<span data-ttu-id="755ad-156">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-156">String</span></span>|<span data-ttu-id="755ad-157">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="755ad-157">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="755ad-158">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="755ad-158">settingValueDisplayUnits</span></span>|<span data-ttu-id="755ad-159">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-159">String</span></span>|<span data-ttu-id="755ad-160">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="755ad-160">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="755ad-161">settingCategory</span><span class="sxs-lookup"><span data-stu-id="755ad-161">settingCategory</span></span>|<span data-ttu-id="755ad-162">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-162">String</span></span>|<span data-ttu-id="755ad-163">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="755ad-163">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="755ad-164">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="755ad-164">mdmCspName</span></span>|<span data-ttu-id="755ad-165">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-165">String</span></span>|<span data-ttu-id="755ad-166">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="755ad-166">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="755ad-167">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="755ad-167">mdmSettingUri</span></span>|<span data-ttu-id="755ad-168">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-168">String</span></span>|<span data-ttu-id="755ad-169">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="755ad-169">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="755ad-170">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="755ad-170">mdmMinimumOSVersion</span></span>|<span data-ttu-id="755ad-171">Int32</span><span class="sxs-lookup"><span data-stu-id="755ad-171">Int32</span></span>|<span data-ttu-id="755ad-172">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="755ad-172">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="755ad-173">settingType</span><span class="sxs-lookup"><span data-stu-id="755ad-173">settingType</span></span>|[<span data-ttu-id="755ad-174">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="755ad-174">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="755ad-175">组策略的设置类型 (安全性或 admx) 。</span><span class="sxs-lookup"><span data-stu-id="755ad-175">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="755ad-176">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="755ad-176">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="755ad-177">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="755ad-177">isMdmSupported</span></span>|<span data-ttu-id="755ad-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="755ad-178">Boolean</span></span>|<span data-ttu-id="755ad-179">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="755ad-179">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="755ad-180">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="755ad-180">mdmSupportedState</span></span>|[<span data-ttu-id="755ad-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="755ad-181">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="755ad-182">指示是否支持 Mdm 中的设置。</span><span class="sxs-lookup"><span data-stu-id="755ad-182">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="755ad-183">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="755ad-183">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="755ad-184">settingScope</span><span class="sxs-lookup"><span data-stu-id="755ad-184">settingScope</span></span>|[<span data-ttu-id="755ad-185">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="755ad-185">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="755ad-186">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="755ad-186">The scope of the setting.</span></span> <span data-ttu-id="755ad-187">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="755ad-187">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="755ad-188">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="755ad-188">intuneSettingUriList</span></span>|<span data-ttu-id="755ad-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="755ad-189">String collection</span></span>|<span data-ttu-id="755ad-190">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="755ad-190">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="755ad-191">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="755ad-191">intuneSettingDefinitionId</span></span>|<span data-ttu-id="755ad-192">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-192">String</span></span>|<span data-ttu-id="755ad-193">Intune 设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="755ad-193">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="755ad-194">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="755ad-194">admxSettingDefinitionId</span></span>|<span data-ttu-id="755ad-195">字符串</span><span class="sxs-lookup"><span data-stu-id="755ad-195">String</span></span>|<span data-ttu-id="755ad-196">Admx 组策略 Id</span><span class="sxs-lookup"><span data-stu-id="755ad-196">Admx Group Policy Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="755ad-197">关系</span><span class="sxs-lookup"><span data-stu-id="755ad-197">Relationships</span></span>
<span data-ttu-id="755ad-198">无</span><span class="sxs-lookup"><span data-stu-id="755ad-198">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="755ad-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="755ad-199">JSON Representation</span></span>
<span data-ttu-id="755ad-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="755ad-200">Here is a JSON representation of the resource.</span></span>
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




