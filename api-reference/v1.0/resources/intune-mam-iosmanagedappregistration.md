---
title: iosManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 iOS 应用的同步详细信息。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a0896e848cc83bb2671b0a8d4160ec9dace5ca7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088501"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="6b595-104">iosManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b595-104">iosManagedAppRegistration resource type</span></span>

<span data-ttu-id="6b595-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b595-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b595-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b595-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b595-107">表示特定用户具有管理功能的 iOS 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="6b595-107">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="6b595-108">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6b595-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="6b595-109">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-109">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6b595-110">方法</span><span class="sxs-lookup"><span data-stu-id="6b595-110">Methods</span></span>
|<span data-ttu-id="6b595-111">方法</span><span class="sxs-lookup"><span data-stu-id="6b595-111">Method</span></span>|<span data-ttu-id="6b595-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="6b595-112">Return Type</span></span>|<span data-ttu-id="6b595-113">说明</span><span class="sxs-lookup"><span data-stu-id="6b595-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b595-114">List iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="6b595-114">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="6b595-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b595-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="6b595-116">列出 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b595-116">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="6b595-117">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6b595-117">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="6b595-118">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6b595-118">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="6b595-119">读取 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b595-119">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b595-120">属性</span><span class="sxs-lookup"><span data-stu-id="6b595-120">Properties</span></span>
|<span data-ttu-id="6b595-121">属性</span><span class="sxs-lookup"><span data-stu-id="6b595-121">Property</span></span>|<span data-ttu-id="6b595-122">类型</span><span class="sxs-lookup"><span data-stu-id="6b595-122">Type</span></span>|<span data-ttu-id="6b595-123">说明</span><span class="sxs-lookup"><span data-stu-id="6b595-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b595-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b595-124">createdDateTime</span></span>|<span data-ttu-id="6b595-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b595-125">DateTimeOffset</span></span>|<span data-ttu-id="6b595-126">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-126">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6b595-127">lastSyncDateTime</span></span>|<span data-ttu-id="6b595-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b595-128">DateTimeOffset</span></span>|<span data-ttu-id="6b595-129">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6b595-129">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="6b595-130">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-130">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="6b595-131">applicationVersion</span></span>|<span data-ttu-id="6b595-132">String</span><span class="sxs-lookup"><span data-stu-id="6b595-132">String</span></span>|<span data-ttu-id="6b595-133">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-133">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6b595-134">managementSdkVersion</span></span>|<span data-ttu-id="6b595-135">String</span><span class="sxs-lookup"><span data-stu-id="6b595-135">String</span></span>|<span data-ttu-id="6b595-136">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-136">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="6b595-137">platformVersion</span></span>|<span data-ttu-id="6b595-138">String</span><span class="sxs-lookup"><span data-stu-id="6b595-138">String</span></span>|<span data-ttu-id="6b595-139">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-139">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="6b595-140">deviceType</span></span>|<span data-ttu-id="6b595-141">String</span><span class="sxs-lookup"><span data-stu-id="6b595-141">String</span></span>|<span data-ttu-id="6b595-142">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-142">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6b595-143">deviceTag</span></span>|<span data-ttu-id="6b595-144">String</span><span class="sxs-lookup"><span data-stu-id="6b595-144">String</span></span>|<span data-ttu-id="6b595-145">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="6b595-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="6b595-146">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="6b595-146">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="6b595-147">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-147">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="6b595-148">deviceName</span></span>|<span data-ttu-id="6b595-149">String</span><span class="sxs-lookup"><span data-stu-id="6b595-149">String</span></span>|<span data-ttu-id="6b595-150">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-150">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="6b595-151">flaggedReasons</span></span>|<span data-ttu-id="6b595-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b595-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="6b595-153">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="6b595-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="6b595-154">例如，</span><span class="sxs-lookup"><span data-stu-id="6b595-154">E.g.</span></span> <span data-ttu-id="6b595-155">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-155">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-156">userId</span><span class="sxs-lookup"><span data-stu-id="6b595-156">userId</span></span>|<span data-ttu-id="6b595-157">String</span><span class="sxs-lookup"><span data-stu-id="6b595-157">String</span></span>|<span data-ttu-id="6b595-158">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6b595-158">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="6b595-159">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-159">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-160">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6b595-160">appIdentifier</span></span>|[<span data-ttu-id="6b595-161">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6b595-161">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6b595-162">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-162">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-163">id</span><span class="sxs-lookup"><span data-stu-id="6b595-163">id</span></span>|<span data-ttu-id="6b595-164">String</span><span class="sxs-lookup"><span data-stu-id="6b595-164">String</span></span>|<span data-ttu-id="6b595-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6b595-165">Key of the entity.</span></span> <span data-ttu-id="6b595-166">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-166">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-167">version</span><span class="sxs-lookup"><span data-stu-id="6b595-167">version</span></span>|<span data-ttu-id="6b595-168">String</span><span class="sxs-lookup"><span data-stu-id="6b595-168">String</span></span>|<span data-ttu-id="6b595-169">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6b595-169">Version of the entity.</span></span> <span data-ttu-id="6b595-170">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-170">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b595-171">关系</span><span class="sxs-lookup"><span data-stu-id="6b595-171">Relationships</span></span>
|<span data-ttu-id="6b595-172">关系</span><span class="sxs-lookup"><span data-stu-id="6b595-172">Relationship</span></span>|<span data-ttu-id="6b595-173">类型</span><span class="sxs-lookup"><span data-stu-id="6b595-173">Type</span></span>|<span data-ttu-id="6b595-174">说明</span><span class="sxs-lookup"><span data-stu-id="6b595-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b595-175">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="6b595-175">appliedPolicies</span></span>|<span data-ttu-id="6b595-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b595-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6b595-177">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="6b595-177">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="6b595-178">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-179">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="6b595-179">intendedPolicies</span></span>|<span data-ttu-id="6b595-180">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b595-180">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6b595-181">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="6b595-181">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="6b595-182">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-182">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6b595-183">operations</span><span class="sxs-lookup"><span data-stu-id="6b595-183">operations</span></span>|<span data-ttu-id="6b595-184">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b595-184">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="6b595-185">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="6b595-185">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="6b595-186">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6b595-186">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b595-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b595-187">JSON Representation</span></span>
<span data-ttu-id="6b595-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b595-188">Here is a JSON representation of the resource.</span></span>
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
     "Warning: /api-reference/v1.0/resources/intune-mam-iosmanagedappregistration.md/microsoft.graph.iosManagedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->







