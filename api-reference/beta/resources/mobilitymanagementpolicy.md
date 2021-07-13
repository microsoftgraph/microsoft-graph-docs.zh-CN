---
title: mobilityManagementPolicy 资源类型
description: 移动管理策略表示在 Azure AD 中配置的移动性管理应用程序的自动注册策略。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6c2035d96293a28f4d8289606df709fc64d9c3e7
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401538"
---
# <a name="mobilitymanagementpolicy-resource-type"></a><span data-ttu-id="00ee3-103">mobilityManagementPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="00ee3-103">mobilityManagementPolicy resource type</span></span>

<span data-ttu-id="00ee3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00ee3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00ee3-105">在 Azure AD 中，移动管理策略表示 MDM 或 MAM (移动管理自动注册) 配置。</span><span class="sxs-lookup"><span data-stu-id="00ee3-105">In Azure AD, a mobility management policy represents an auto-enrollment configuration for a mobility management (MDM or MAM) application.</span></span> <span data-ttu-id="00ee3-106">这些策略仅适用于基于 Windows 10 操作系统及其派生 (Surface Hub、Hololens 等) 。</span><span class="sxs-lookup"><span data-stu-id="00ee3-106">These policies are only applicable to devices based on Windows 10 OS and its derivatives (Surface Hub, Hololens etc.).</span></span> <span data-ttu-id="00ee3-107">[自动注册](/windows/client-management/mdm/azure-ad-and-microsoft-intune-automatic-mdm-enrollment-in-the-new-portal)使组织能够自动将设备注册到所选移动管理应用程序中，作为[Azure AD](/azure/active-directory/devices/concept-azure-ad-join)加入或[Azure AD](/azure/active-directory/devices/concept-azure-ad-register)注册过程的一部分，Windows 10注册。</span><span class="sxs-lookup"><span data-stu-id="00ee3-107">[Auto-enrollment](/windows/client-management/mdm/azure-ad-and-microsoft-intune-automatic-mdm-enrollment-in-the-new-portal) enables organizations to automatically enroll devices into their chosen mobility management application as part of [Azure AD join](/azure/active-directory/devices/concept-azure-ad-join) or [Azure AD register](/azure/active-directory/devices/concept-azure-ad-register) process on Windows 10 devices.</span></span>

## <a name="methods"></a><span data-ttu-id="00ee3-108">方法</span><span class="sxs-lookup"><span data-stu-id="00ee3-108">Methods</span></span>

|<span data-ttu-id="00ee3-109">方法</span><span class="sxs-lookup"><span data-stu-id="00ee3-109">Method</span></span>|<span data-ttu-id="00ee3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="00ee3-110">Return type</span></span>|<span data-ttu-id="00ee3-111">说明</span><span class="sxs-lookup"><span data-stu-id="00ee3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00ee3-112">列出 mobileDeviceManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="00ee3-112">List mobileDeviceManagementPolicies</span></span>](../api/mobiledevicemanagementpolicies-list.md)|<span data-ttu-id="00ee3-113">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00ee3-113">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) collection</span></span>|<span data-ttu-id="00ee3-114">获取移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="00ee3-114">Get a list of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects and their properties for mobile device management applications.</span></span>|
|[<span data-ttu-id="00ee3-115">获取 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-115">Get mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-get.md)|[<span data-ttu-id="00ee3-116">mobilityManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-116">mobilityManagementPolicy</span></span>](../resources/mobilitymanagementpolicy.md)|<span data-ttu-id="00ee3-117">读取移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00ee3-117">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="00ee3-118">更新 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-118">Update mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-update.md)|<span data-ttu-id="00ee3-119">无</span><span class="sxs-lookup"><span data-stu-id="00ee3-119">None</span></span>|<span data-ttu-id="00ee3-120">更新移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00ee3-120">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="00ee3-121">列出 mobileDeviceManagementPolicy 的 includedGroups</span><span class="sxs-lookup"><span data-stu-id="00ee3-121">List includedGroups of mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-list-includedgroups.md)|<span data-ttu-id="00ee3-122">[group](../resources/group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00ee3-122">[group](../resources/group.md) collection</span></span>|<span data-ttu-id="00ee3-123">列出移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的组。</span><span class="sxs-lookup"><span data-stu-id="00ee3-123">List included groups for a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="00ee3-124">将组添加到 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-124">Add group to mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-post-includedgroups.md)|<span data-ttu-id="00ee3-125">无</span><span class="sxs-lookup"><span data-stu-id="00ee3-125">None</span></span>|<span data-ttu-id="00ee3-126">将组添加到移动设备管理 [应用程序的 mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00ee3-126">Add a group to the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="00ee3-127">从 mobileDeviceManagementPolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="00ee3-127">Delete group from mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-delete-includedgroups.md)|<span data-ttu-id="00ee3-128">无</span><span class="sxs-lookup"><span data-stu-id="00ee3-128">None</span></span>|<span data-ttu-id="00ee3-129">从移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象中删除组。</span><span class="sxs-lookup"><span data-stu-id="00ee3-129">Delete a group from the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="00ee3-130">列出 mobileAppManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="00ee3-130">List mobileAppManagementPolicies</span></span>](../api/mobileappmanagementpolicies-list.md)|<span data-ttu-id="00ee3-131">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00ee3-131">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) collection</span></span>|<span data-ttu-id="00ee3-132">获取移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="00ee3-132">Get a list of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects and their properties for mobile app management applications.</span></span>|
|[<span data-ttu-id="00ee3-133">获取 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-133">Get mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-get.md)|[<span data-ttu-id="00ee3-134">mobilityManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-134">mobilityManagementPolicy</span></span>](../resources/mobilitymanagementpolicy.md)|<span data-ttu-id="00ee3-135">读取移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00ee3-135">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|
|[<span data-ttu-id="00ee3-136">更新 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-136">Update mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-update.md)|<span data-ttu-id="00ee3-137">无</span><span class="sxs-lookup"><span data-stu-id="00ee3-137">None</span></span>|<span data-ttu-id="00ee3-138">更新移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00ee3-138">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|
|[<span data-ttu-id="00ee3-139">列出 mobileAppManagementPolicy 的 includedGroups</span><span class="sxs-lookup"><span data-stu-id="00ee3-139">List includedGroups of mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-list-includedgroups.md)|<span data-ttu-id="00ee3-140">[group](../resources/group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00ee3-140">[group](../resources/group.md) collection</span></span>|<span data-ttu-id="00ee3-141">列出移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的组。</span><span class="sxs-lookup"><span data-stu-id="00ee3-141">List included groups for a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|
|[<span data-ttu-id="00ee3-142">将组添加到 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="00ee3-142">Add group to mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-post-includedgroups.md)|<span data-ttu-id="00ee3-143">无</span><span class="sxs-lookup"><span data-stu-id="00ee3-143">None</span></span>|<span data-ttu-id="00ee3-144">将组添加到 [移动应用管理应用程序的 mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00ee3-144">Add a group to the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>
|[<span data-ttu-id="00ee3-145">从 mobileAppManagementPolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="00ee3-145">Delete group from mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-delete-includedgroups.md)|<span data-ttu-id="00ee3-146">无</span><span class="sxs-lookup"><span data-stu-id="00ee3-146">None</span></span>|<span data-ttu-id="00ee3-147">从移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象中删除组。</span><span class="sxs-lookup"><span data-stu-id="00ee3-147">Delete a group from the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|

## <a name="properties"></a><span data-ttu-id="00ee3-148">属性</span><span class="sxs-lookup"><span data-stu-id="00ee3-148">Properties</span></span>

|<span data-ttu-id="00ee3-149">属性</span><span class="sxs-lookup"><span data-stu-id="00ee3-149">Property</span></span>|<span data-ttu-id="00ee3-150">类型</span><span class="sxs-lookup"><span data-stu-id="00ee3-150">Type</span></span>|<span data-ttu-id="00ee3-151">说明</span><span class="sxs-lookup"><span data-stu-id="00ee3-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00ee3-152">appliesTo</span><span class="sxs-lookup"><span data-stu-id="00ee3-152">appliesTo</span></span>|<span data-ttu-id="00ee3-153">policyScope</span><span class="sxs-lookup"><span data-stu-id="00ee3-153">policyScope</span></span>|<span data-ttu-id="00ee3-154">指示移动管理策略的用户作用域。</span><span class="sxs-lookup"><span data-stu-id="00ee3-154">Indicates the user scope of the mobility management policy.</span></span> <span data-ttu-id="00ee3-155">可取值为：`none`、`all`、`selected`。</span><span class="sxs-lookup"><span data-stu-id="00ee3-155">Possible values are: `none`, `all`, `selected`.</span></span>|
|<span data-ttu-id="00ee3-156">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="00ee3-156">complianceUrl</span></span>|<span data-ttu-id="00ee3-157">String</span><span class="sxs-lookup"><span data-stu-id="00ee3-157">String</span></span>|<span data-ttu-id="00ee3-158">移动管理应用程序的合规性 URL。</span><span class="sxs-lookup"><span data-stu-id="00ee3-158">Compliance URL of the mobility management application.</span></span>|
|<span data-ttu-id="00ee3-159">说明</span><span class="sxs-lookup"><span data-stu-id="00ee3-159">description</span></span>|<span data-ttu-id="00ee3-160">String</span><span class="sxs-lookup"><span data-stu-id="00ee3-160">String</span></span>|<span data-ttu-id="00ee3-161">移动管理应用程序的说明。</span><span class="sxs-lookup"><span data-stu-id="00ee3-161">Description of the mobility management application.</span></span>|
|<span data-ttu-id="00ee3-162">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="00ee3-162">discoveryUrl</span></span>|<span data-ttu-id="00ee3-163">String</span><span class="sxs-lookup"><span data-stu-id="00ee3-163">String</span></span>|<span data-ttu-id="00ee3-164">移动管理应用程序的发现 URL。</span><span class="sxs-lookup"><span data-stu-id="00ee3-164">Discovery URL of the mobility management application.</span></span>|
|<span data-ttu-id="00ee3-165">displayName</span><span class="sxs-lookup"><span data-stu-id="00ee3-165">displayName</span></span>|<span data-ttu-id="00ee3-166">String</span><span class="sxs-lookup"><span data-stu-id="00ee3-166">String</span></span>|<span data-ttu-id="00ee3-167">移动管理应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="00ee3-167">Display name of the mobility management application.</span></span>|
|<span data-ttu-id="00ee3-168">id</span><span class="sxs-lookup"><span data-stu-id="00ee3-168">id</span></span>|<span data-ttu-id="00ee3-169">String</span><span class="sxs-lookup"><span data-stu-id="00ee3-169">String</span></span>|<span data-ttu-id="00ee3-170">移动管理应用程序的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="00ee3-170">Object Id of the mobility management application.</span></span>|
|<span data-ttu-id="00ee3-171">isValid</span><span class="sxs-lookup"><span data-stu-id="00ee3-171">isValid</span></span>|<span data-ttu-id="00ee3-172">布尔</span><span class="sxs-lookup"><span data-stu-id="00ee3-172">Boolean</span></span>|<span data-ttu-id="00ee3-173">策略是否有效。</span><span class="sxs-lookup"><span data-stu-id="00ee3-173">Whether policy is valid.</span></span> <span data-ttu-id="00ee3-174">无效的策略可能无法更新，应删除。</span><span class="sxs-lookup"><span data-stu-id="00ee3-174">Invalid policies may not be updated and should be deleted.</span></span>|
|<span data-ttu-id="00ee3-175">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="00ee3-175">termsOfUseUrl</span></span>|<span data-ttu-id="00ee3-176">String</span><span class="sxs-lookup"><span data-stu-id="00ee3-176">String</span></span>|<span data-ttu-id="00ee3-177">移动管理应用程序的使用条款 URL。</span><span class="sxs-lookup"><span data-stu-id="00ee3-177">Terms of Use URL of the mobility management application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00ee3-178">关系</span><span class="sxs-lookup"><span data-stu-id="00ee3-178">Relationships</span></span>

|<span data-ttu-id="00ee3-179">关系</span><span class="sxs-lookup"><span data-stu-id="00ee3-179">Relationship</span></span>|<span data-ttu-id="00ee3-180">类型</span><span class="sxs-lookup"><span data-stu-id="00ee3-180">Type</span></span>|<span data-ttu-id="00ee3-181">说明</span><span class="sxs-lookup"><span data-stu-id="00ee3-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00ee3-182">includedGroups</span><span class="sxs-lookup"><span data-stu-id="00ee3-182">includedGroups</span></span>|<span data-ttu-id="00ee3-183">[group](../resources/group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00ee3-183">[group](../resources/group.md) collection</span></span>|<span data-ttu-id="00ee3-184">移动性管理应用程序作用域下的 Azure AD 组（如果 appliesTo 为 ） `selected`</span><span class="sxs-lookup"><span data-stu-id="00ee3-184">Azure AD groups under the scope of the mobility management application if appliesTo is `selected`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00ee3-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00ee3-185">JSON representation</span></span>

<span data-ttu-id="00ee3-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00ee3-186">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobilityManagementPolicy",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "appliesTo": "String",
  "complianceUrl": "String",
  "description": "String",
  "discoveryUrl": "String",
  "displayName": "String",
  "isValid": "Boolean",
  "termsOfUseUrl": "String"
}
```

<!-- uuid: 5c98f801-d1c4-44eb-ac11-f72b6754deda
2020-03-23T22:34:45.203Z -->
<!-- {
  "type": "#page.annotation",
  "description": "mobilityManagementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
