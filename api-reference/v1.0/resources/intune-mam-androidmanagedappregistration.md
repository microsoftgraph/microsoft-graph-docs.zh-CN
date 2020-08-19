---
title: androidManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 Android 应用的同步详细信息。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f85bd029bdd038745984e339f87362333156841e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811348"
---
# <a name="androidmanagedappregistration-resource-type"></a><span data-ttu-id="cc02c-104">androidManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc02c-104">androidManagedAppRegistration resource type</span></span>

<span data-ttu-id="cc02c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc02c-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc02c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc02c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc02c-107">表示特定用户具有管理功能的 Android 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="cc02c-107">Represents the synchronization details of an android app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="cc02c-108">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cc02c-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="cc02c-109">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-109">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cc02c-110">方法</span><span class="sxs-lookup"><span data-stu-id="cc02c-110">Methods</span></span>
|<span data-ttu-id="cc02c-111">方法</span><span class="sxs-lookup"><span data-stu-id="cc02c-111">Method</span></span>|<span data-ttu-id="cc02c-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc02c-112">Return Type</span></span>|<span data-ttu-id="cc02c-113">说明</span><span class="sxs-lookup"><span data-stu-id="cc02c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc02c-114">List androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="cc02c-114">List androidManagedAppRegistrations</span></span>](../api/intune-mam-androidmanagedappregistration-list.md)|<span data-ttu-id="cc02c-115">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc02c-115">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) collection</span></span>|<span data-ttu-id="cc02c-116">列出 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc02c-116">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="cc02c-117">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cc02c-117">Get androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-get.md)|[<span data-ttu-id="cc02c-118">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cc02c-118">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="cc02c-119">读取 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc02c-119">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|
|[<span data-ttu-id="cc02c-120">创建 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cc02c-120">Create androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-create.md)|[<span data-ttu-id="cc02c-121">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cc02c-121">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="cc02c-122">创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc02c-122">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc02c-123">属性</span><span class="sxs-lookup"><span data-stu-id="cc02c-123">Properties</span></span>
|<span data-ttu-id="cc02c-124">属性</span><span class="sxs-lookup"><span data-stu-id="cc02c-124">Property</span></span>|<span data-ttu-id="cc02c-125">类型</span><span class="sxs-lookup"><span data-stu-id="cc02c-125">Type</span></span>|<span data-ttu-id="cc02c-126">说明</span><span class="sxs-lookup"><span data-stu-id="cc02c-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc02c-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc02c-127">createdDateTime</span></span>|<span data-ttu-id="cc02c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc02c-128">DateTimeOffset</span></span>|<span data-ttu-id="cc02c-129">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-129">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cc02c-130">lastSyncDateTime</span></span>|<span data-ttu-id="cc02c-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc02c-131">DateTimeOffset</span></span>|<span data-ttu-id="cc02c-132">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc02c-132">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="cc02c-133">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-133">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-134">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="cc02c-134">applicationVersion</span></span>|<span data-ttu-id="cc02c-135">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-135">String</span></span>|<span data-ttu-id="cc02c-136">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-136">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-137">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="cc02c-137">managementSdkVersion</span></span>|<span data-ttu-id="cc02c-138">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-138">String</span></span>|<span data-ttu-id="cc02c-139">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-139">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-140">platformVersion</span><span class="sxs-lookup"><span data-stu-id="cc02c-140">platformVersion</span></span>|<span data-ttu-id="cc02c-141">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-141">String</span></span>|<span data-ttu-id="cc02c-142">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-142">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-143">deviceType</span><span class="sxs-lookup"><span data-stu-id="cc02c-143">deviceType</span></span>|<span data-ttu-id="cc02c-144">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-144">String</span></span>|<span data-ttu-id="cc02c-145">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-145">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-146">deviceTag</span><span class="sxs-lookup"><span data-stu-id="cc02c-146">deviceTag</span></span>|<span data-ttu-id="cc02c-147">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-147">String</span></span>|<span data-ttu-id="cc02c-148">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="cc02c-148">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="cc02c-149">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="cc02c-149">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="cc02c-150">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-150">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="cc02c-151">deviceName</span></span>|<span data-ttu-id="cc02c-152">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-152">String</span></span>|<span data-ttu-id="cc02c-153">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-153">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-154">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="cc02c-154">flaggedReasons</span></span>|<span data-ttu-id="cc02c-155">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc02c-155">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="cc02c-156">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="cc02c-156">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="cc02c-157">例如，</span><span class="sxs-lookup"><span data-stu-id="cc02c-157">E.g.</span></span> <span data-ttu-id="cc02c-158">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-158">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-159">userId</span><span class="sxs-lookup"><span data-stu-id="cc02c-159">userId</span></span>|<span data-ttu-id="cc02c-160">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-160">String</span></span>|<span data-ttu-id="cc02c-161">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="cc02c-161">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="cc02c-162">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-162">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-163">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="cc02c-163">appIdentifier</span></span>|[<span data-ttu-id="cc02c-164">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="cc02c-164">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="cc02c-165">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-165">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-166">id</span><span class="sxs-lookup"><span data-stu-id="cc02c-166">id</span></span>|<span data-ttu-id="cc02c-167">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-167">String</span></span>|<span data-ttu-id="cc02c-168">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cc02c-168">Key of the entity.</span></span> <span data-ttu-id="cc02c-169">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-170">version</span><span class="sxs-lookup"><span data-stu-id="cc02c-170">version</span></span>|<span data-ttu-id="cc02c-171">String</span><span class="sxs-lookup"><span data-stu-id="cc02c-171">String</span></span>|<span data-ttu-id="cc02c-172">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="cc02c-172">Version of the entity.</span></span> <span data-ttu-id="cc02c-173">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-173">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc02c-174">关系</span><span class="sxs-lookup"><span data-stu-id="cc02c-174">Relationships</span></span>
|<span data-ttu-id="cc02c-175">关系</span><span class="sxs-lookup"><span data-stu-id="cc02c-175">Relationship</span></span>|<span data-ttu-id="cc02c-176">类型</span><span class="sxs-lookup"><span data-stu-id="cc02c-176">Type</span></span>|<span data-ttu-id="cc02c-177">说明</span><span class="sxs-lookup"><span data-stu-id="cc02c-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc02c-178">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="cc02c-178">appliedPolicies</span></span>|<span data-ttu-id="cc02c-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc02c-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="cc02c-180">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="cc02c-180">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="cc02c-181">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-181">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-182">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="cc02c-182">intendedPolicies</span></span>|<span data-ttu-id="cc02c-183">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc02c-183">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="cc02c-184">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="cc02c-184">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="cc02c-185">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cc02c-186">operations</span><span class="sxs-lookup"><span data-stu-id="cc02c-186">operations</span></span>|<span data-ttu-id="cc02c-187">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc02c-187">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="cc02c-188">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="cc02c-188">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="cc02c-189">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cc02c-189">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc02c-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc02c-190">JSON Representation</span></span>
<span data-ttu-id="cc02c-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc02c-191">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/appIdentifier:
      Type mismatch between example and table. Parameter name: appIdentifier; example type: (microsoft.graph.androidMobileAppIdentifier); table type: (microsoft.graph.mobileAppIdentifier)",
      "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/flaggedReasons:

      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->





