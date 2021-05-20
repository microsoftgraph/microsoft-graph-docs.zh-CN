---
title: mobilityManagementPolicy 资源类型
description: 移动管理策略表示在 Azure AD 中配置的移动性管理应用程序的自动注册策略。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7f0c073d0737c634872009fffa5425ffe74f4e54
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547403"
---
# <a name="mobilitymanagementpolicy-resource-type"></a><span data-ttu-id="d951e-103">mobilityManagementPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d951e-103">mobilityManagementPolicy resource type</span></span>

<span data-ttu-id="d951e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d951e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d951e-105">在 Azure AD 中，移动管理策略表示 MDM 或 MAM (移动管理自动注册) 配置。</span><span class="sxs-lookup"><span data-stu-id="d951e-105">In Azure AD, a mobility management policy represents an auto-enrollment configuration for a mobility management (MDM or MAM) application.</span></span> <span data-ttu-id="d951e-106">这些策略仅适用于基于 Windows 10 操作系统及其派生 (Surface Hub、Hololens 等) 。</span><span class="sxs-lookup"><span data-stu-id="d951e-106">These policies are only applicable to devices based on Windows 10 OS and its derivatives (Surface Hub, Hololens etc.).</span></span> <span data-ttu-id="d951e-107">[自动注册](https://docs.microsoft.com/windows/client-management/mdm/azure-ad-and-microsoft-intune-automatic-mdm-enrollment-in-the-new-portal)使组织能够自动将设备注册到所选移动管理应用程序中，作为[Azure AD](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-join)加入或[Azure AD](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-register)注册过程的一部分，Windows 10注册。</span><span class="sxs-lookup"><span data-stu-id="d951e-107">[Auto-enrollment](https://docs.microsoft.com/windows/client-management/mdm/azure-ad-and-microsoft-intune-automatic-mdm-enrollment-in-the-new-portal) enables organizations to automatically enroll devices into their chosen mobility management application as part of [Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-join) or [Azure AD register](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-register) process on Windows 10 devices.</span></span>

## <a name="methods"></a><span data-ttu-id="d951e-108">方法</span><span class="sxs-lookup"><span data-stu-id="d951e-108">Methods</span></span>

|<span data-ttu-id="d951e-109">方法</span><span class="sxs-lookup"><span data-stu-id="d951e-109">Method</span></span>|<span data-ttu-id="d951e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d951e-110">Return type</span></span>|<span data-ttu-id="d951e-111">说明</span><span class="sxs-lookup"><span data-stu-id="d951e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d951e-112">列出 mobileDeviceManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="d951e-112">List mobileDeviceManagementPolicies</span></span>](../api/mobiledevicemanagementpolicies-list.md)|<span data-ttu-id="d951e-113">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d951e-113">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) collection</span></span>|<span data-ttu-id="d951e-114">获取移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d951e-114">Get a list of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects and their properties for mobile device management applications.</span></span>|
|[<span data-ttu-id="d951e-115">获取 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-115">Get mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-get.md)|[<span data-ttu-id="d951e-116">mobilityManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-116">mobilityManagementPolicy</span></span>](../resources/mobilitymanagementpolicy.md)|<span data-ttu-id="d951e-117">读取移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d951e-117">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="d951e-118">更新 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-118">Update mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-update.md)|<span data-ttu-id="d951e-119">无</span><span class="sxs-lookup"><span data-stu-id="d951e-119">None</span></span>|<span data-ttu-id="d951e-120">更新移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d951e-120">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="d951e-121">列出 mobileDeviceManagementPolicy 的 includedGroups</span><span class="sxs-lookup"><span data-stu-id="d951e-121">List includedGroups of mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-list-includedgroups.md)|<span data-ttu-id="d951e-122">[group](../resources/group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d951e-122">[group](../resources/group.md) collection</span></span>|<span data-ttu-id="d951e-123">列出移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的组。</span><span class="sxs-lookup"><span data-stu-id="d951e-123">List included groups for a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="d951e-124">将组添加到 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-124">Add group to mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-post-includedgroups.md)|<span data-ttu-id="d951e-125">无</span><span class="sxs-lookup"><span data-stu-id="d951e-125">None</span></span>|<span data-ttu-id="d951e-126">将组添加到移动设备管理 [应用程序的 mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d951e-126">Add a group to the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="d951e-127">从 mobileDeviceManagementPolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="d951e-127">Delete group from mobileDeviceManagementPolicy</span></span>](../api/mobiledevicemanagementpolicies-delete-includedgroups.md)|<span data-ttu-id="d951e-128">无</span><span class="sxs-lookup"><span data-stu-id="d951e-128">None</span></span>|<span data-ttu-id="d951e-129">从移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象中删除组。</span><span class="sxs-lookup"><span data-stu-id="d951e-129">Delete a group from the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile device management application.</span></span>|
|[<span data-ttu-id="d951e-130">列出 mobileAppManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="d951e-130">List mobileAppManagementPolicies</span></span>](../api/mobileappmanagementpolicies-list.md)|<span data-ttu-id="d951e-131">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d951e-131">[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) collection</span></span>|<span data-ttu-id="d951e-132">获取移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d951e-132">Get a list of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects and their properties for mobile app management applications.</span></span>|
|[<span data-ttu-id="d951e-133">获取 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-133">Get mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-get.md)|[<span data-ttu-id="d951e-134">mobilityManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-134">mobilityManagementPolicy</span></span>](../resources/mobilitymanagementpolicy.md)|<span data-ttu-id="d951e-135">读取移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d951e-135">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|
|[<span data-ttu-id="d951e-136">更新 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-136">Update mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-update.md)|<span data-ttu-id="d951e-137">无</span><span class="sxs-lookup"><span data-stu-id="d951e-137">None</span></span>|<span data-ttu-id="d951e-138">更新移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d951e-138">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|
|[<span data-ttu-id="d951e-139">列出 mobileAppManagementPolicy 的 includedGroups</span><span class="sxs-lookup"><span data-stu-id="d951e-139">List includedGroups of mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-list-includedgroups.md)|<span data-ttu-id="d951e-140">[group](../resources/group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d951e-140">[group](../resources/group.md) collection</span></span>|<span data-ttu-id="d951e-141">列出移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的组。</span><span class="sxs-lookup"><span data-stu-id="d951e-141">List included groups for a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|
|[<span data-ttu-id="d951e-142">将组添加到 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d951e-142">Add group to mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-post-includedgroups.md)|<span data-ttu-id="d951e-143">无</span><span class="sxs-lookup"><span data-stu-id="d951e-143">None</span></span>|<span data-ttu-id="d951e-144">将组添加到 [移动应用管理应用程序的 mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d951e-144">Add a group to the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>
|[<span data-ttu-id="d951e-145">从 mobileAppManagementPolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="d951e-145">Delete group from mobileAppManagementPolicy</span></span>](../api/mobileappmanagementpolicies-delete-includedgroups.md)|<span data-ttu-id="d951e-146">无</span><span class="sxs-lookup"><span data-stu-id="d951e-146">None</span></span>|<span data-ttu-id="d951e-147">从移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象中删除组。</span><span class="sxs-lookup"><span data-stu-id="d951e-147">Delete a group from the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object for a mobile app management application.</span></span>|

## <a name="properties"></a><span data-ttu-id="d951e-148">属性</span><span class="sxs-lookup"><span data-stu-id="d951e-148">Properties</span></span>

|<span data-ttu-id="d951e-149">属性</span><span class="sxs-lookup"><span data-stu-id="d951e-149">Property</span></span>|<span data-ttu-id="d951e-150">类型</span><span class="sxs-lookup"><span data-stu-id="d951e-150">Type</span></span>|<span data-ttu-id="d951e-151">说明</span><span class="sxs-lookup"><span data-stu-id="d951e-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d951e-152">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d951e-152">appliesTo</span></span>|<span data-ttu-id="d951e-153">policyScope</span><span class="sxs-lookup"><span data-stu-id="d951e-153">policyScope</span></span>|<span data-ttu-id="d951e-154">指示移动管理策略的用户作用域。</span><span class="sxs-lookup"><span data-stu-id="d951e-154">Indicates the user scope of the mobility management policy.</span></span> <span data-ttu-id="d951e-155">可取值为：`none`、`all`、`selected`。</span><span class="sxs-lookup"><span data-stu-id="d951e-155">Possible values are: `none`, `all`, `selected`.</span></span>|
|<span data-ttu-id="d951e-156">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="d951e-156">complianceUrl</span></span>|<span data-ttu-id="d951e-157">String</span><span class="sxs-lookup"><span data-stu-id="d951e-157">String</span></span>|<span data-ttu-id="d951e-158">移动管理应用程序的合规性 URL。</span><span class="sxs-lookup"><span data-stu-id="d951e-158">Compliance URL of the mobility management application.</span></span>|
|<span data-ttu-id="d951e-159">说明</span><span class="sxs-lookup"><span data-stu-id="d951e-159">description</span></span>|<span data-ttu-id="d951e-160">String</span><span class="sxs-lookup"><span data-stu-id="d951e-160">String</span></span>|<span data-ttu-id="d951e-161">移动管理应用程序的说明。</span><span class="sxs-lookup"><span data-stu-id="d951e-161">Description of the mobility management application.</span></span>|
|<span data-ttu-id="d951e-162">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="d951e-162">discoveryUrl</span></span>|<span data-ttu-id="d951e-163">String</span><span class="sxs-lookup"><span data-stu-id="d951e-163">String</span></span>|<span data-ttu-id="d951e-164">移动管理应用程序的发现 URL。</span><span class="sxs-lookup"><span data-stu-id="d951e-164">Discovery URL of the mobility management application.</span></span>|
|<span data-ttu-id="d951e-165">displayName</span><span class="sxs-lookup"><span data-stu-id="d951e-165">displayName</span></span>|<span data-ttu-id="d951e-166">String</span><span class="sxs-lookup"><span data-stu-id="d951e-166">String</span></span>|<span data-ttu-id="d951e-167">移动管理应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d951e-167">Display name of the mobility management application.</span></span>|
|<span data-ttu-id="d951e-168">id</span><span class="sxs-lookup"><span data-stu-id="d951e-168">id</span></span>|<span data-ttu-id="d951e-169">String</span><span class="sxs-lookup"><span data-stu-id="d951e-169">String</span></span>|<span data-ttu-id="d951e-170">移动管理应用程序的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="d951e-170">Object Id of the mobility management application.</span></span>|
|<span data-ttu-id="d951e-171">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="d951e-171">termsOfUseUrl</span></span>|<span data-ttu-id="d951e-172">String</span><span class="sxs-lookup"><span data-stu-id="d951e-172">String</span></span>|<span data-ttu-id="d951e-173">移动管理应用程序的使用条款 URL。</span><span class="sxs-lookup"><span data-stu-id="d951e-173">Terms of Use URL of the mobility management application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d951e-174">关系</span><span class="sxs-lookup"><span data-stu-id="d951e-174">Relationships</span></span>

|<span data-ttu-id="d951e-175">关系</span><span class="sxs-lookup"><span data-stu-id="d951e-175">Relationship</span></span>|<span data-ttu-id="d951e-176">类型</span><span class="sxs-lookup"><span data-stu-id="d951e-176">Type</span></span>|<span data-ttu-id="d951e-177">说明</span><span class="sxs-lookup"><span data-stu-id="d951e-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d951e-178">includedGroups</span><span class="sxs-lookup"><span data-stu-id="d951e-178">includedGroups</span></span>|<span data-ttu-id="d951e-179">[group](../resources/group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d951e-179">[group](../resources/group.md) collection</span></span>|<span data-ttu-id="d951e-180">移动性管理应用程序作用域下的 Azure AD 组（如果 appliesTo 为 ） `selected`</span><span class="sxs-lookup"><span data-stu-id="d951e-180">Azure AD groups under the scope of the mobility management application if appliesTo is `selected`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d951e-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d951e-181">JSON representation</span></span>

<span data-ttu-id="d951e-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d951e-182">The following is a JSON representation of the resource.</span></span>
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
