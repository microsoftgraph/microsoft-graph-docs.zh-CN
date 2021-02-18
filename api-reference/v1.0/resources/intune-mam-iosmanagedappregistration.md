---
title: iosManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 iOS 应用的同步详细信息。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58933395002bb4f63554e2a7225a89e64cfd8d02
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292502"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="455c8-104">iosManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="455c8-104">iosManagedAppRegistration resource type</span></span>

<span data-ttu-id="455c8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="455c8-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="455c8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="455c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="455c8-107">表示特定用户具有管理功能的 iOS 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="455c8-107">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="455c8-108">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="455c8-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="455c8-109">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-109">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="455c8-110">方法</span><span class="sxs-lookup"><span data-stu-id="455c8-110">Methods</span></span>
|<span data-ttu-id="455c8-111">方法</span><span class="sxs-lookup"><span data-stu-id="455c8-111">Method</span></span>|<span data-ttu-id="455c8-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="455c8-112">Return Type</span></span>|<span data-ttu-id="455c8-113">说明</span><span class="sxs-lookup"><span data-stu-id="455c8-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="455c8-114">List iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="455c8-114">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="455c8-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455c8-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="455c8-116">列出 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="455c8-116">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="455c8-117">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="455c8-117">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="455c8-118">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="455c8-118">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="455c8-119">读取 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="455c8-119">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="455c8-120">属性</span><span class="sxs-lookup"><span data-stu-id="455c8-120">Properties</span></span>
|<span data-ttu-id="455c8-121">属性</span><span class="sxs-lookup"><span data-stu-id="455c8-121">Property</span></span>|<span data-ttu-id="455c8-122">类型</span><span class="sxs-lookup"><span data-stu-id="455c8-122">Type</span></span>|<span data-ttu-id="455c8-123">说明</span><span class="sxs-lookup"><span data-stu-id="455c8-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455c8-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="455c8-124">createdDateTime</span></span>|<span data-ttu-id="455c8-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="455c8-125">DateTimeOffset</span></span>|<span data-ttu-id="455c8-126">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-126">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="455c8-127">lastSyncDateTime</span></span>|<span data-ttu-id="455c8-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="455c8-128">DateTimeOffset</span></span>|<span data-ttu-id="455c8-129">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="455c8-129">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="455c8-130">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-130">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="455c8-131">applicationVersion</span></span>|<span data-ttu-id="455c8-132">String</span><span class="sxs-lookup"><span data-stu-id="455c8-132">String</span></span>|<span data-ttu-id="455c8-133">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-133">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="455c8-134">managementSdkVersion</span></span>|<span data-ttu-id="455c8-135">String</span><span class="sxs-lookup"><span data-stu-id="455c8-135">String</span></span>|<span data-ttu-id="455c8-136">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-136">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="455c8-137">platformVersion</span></span>|<span data-ttu-id="455c8-138">String</span><span class="sxs-lookup"><span data-stu-id="455c8-138">String</span></span>|<span data-ttu-id="455c8-139">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-139">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="455c8-140">deviceType</span></span>|<span data-ttu-id="455c8-141">String</span><span class="sxs-lookup"><span data-stu-id="455c8-141">String</span></span>|<span data-ttu-id="455c8-142">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-142">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="455c8-143">deviceTag</span></span>|<span data-ttu-id="455c8-144">String</span><span class="sxs-lookup"><span data-stu-id="455c8-144">String</span></span>|<span data-ttu-id="455c8-145">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="455c8-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="455c8-146">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="455c8-146">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="455c8-147">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-147">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="455c8-148">deviceName</span></span>|<span data-ttu-id="455c8-149">String</span><span class="sxs-lookup"><span data-stu-id="455c8-149">String</span></span>|<span data-ttu-id="455c8-150">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-150">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="455c8-151">flaggedReasons</span></span>|<span data-ttu-id="455c8-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455c8-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="455c8-153">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="455c8-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="455c8-154">例如，</span><span class="sxs-lookup"><span data-stu-id="455c8-154">E.g.</span></span> <span data-ttu-id="455c8-155">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-155">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-156">userId</span><span class="sxs-lookup"><span data-stu-id="455c8-156">userId</span></span>|<span data-ttu-id="455c8-157">String</span><span class="sxs-lookup"><span data-stu-id="455c8-157">String</span></span>|<span data-ttu-id="455c8-158">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="455c8-158">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="455c8-159">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-159">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-160">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="455c8-160">appIdentifier</span></span>|[<span data-ttu-id="455c8-161">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="455c8-161">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="455c8-162">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-162">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-163">id</span><span class="sxs-lookup"><span data-stu-id="455c8-163">id</span></span>|<span data-ttu-id="455c8-164">String</span><span class="sxs-lookup"><span data-stu-id="455c8-164">String</span></span>|<span data-ttu-id="455c8-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="455c8-165">Key of the entity.</span></span> <span data-ttu-id="455c8-166">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-166">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-167">version</span><span class="sxs-lookup"><span data-stu-id="455c8-167">version</span></span>|<span data-ttu-id="455c8-168">String</span><span class="sxs-lookup"><span data-stu-id="455c8-168">String</span></span>|<span data-ttu-id="455c8-169">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="455c8-169">Version of the entity.</span></span> <span data-ttu-id="455c8-170">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-170">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="455c8-171">关系</span><span class="sxs-lookup"><span data-stu-id="455c8-171">Relationships</span></span>
|<span data-ttu-id="455c8-172">关系</span><span class="sxs-lookup"><span data-stu-id="455c8-172">Relationship</span></span>|<span data-ttu-id="455c8-173">类型</span><span class="sxs-lookup"><span data-stu-id="455c8-173">Type</span></span>|<span data-ttu-id="455c8-174">说明</span><span class="sxs-lookup"><span data-stu-id="455c8-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455c8-175">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="455c8-175">appliedPolicies</span></span>|<span data-ttu-id="455c8-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455c8-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="455c8-177">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="455c8-177">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="455c8-178">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-179">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="455c8-179">intendedPolicies</span></span>|<span data-ttu-id="455c8-180">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455c8-180">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="455c8-181">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="455c8-181">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="455c8-182">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-182">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="455c8-183">operations</span><span class="sxs-lookup"><span data-stu-id="455c8-183">operations</span></span>|<span data-ttu-id="455c8-184">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="455c8-184">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="455c8-185">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="455c8-185">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="455c8-186">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="455c8-186">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="455c8-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="455c8-187">JSON Representation</span></span>
<span data-ttu-id="455c8-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="455c8-188">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
  ],
}
-->







