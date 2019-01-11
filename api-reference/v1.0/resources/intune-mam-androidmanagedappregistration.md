---
title: androidManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 Android 应用的同步详细信息。
localization_priority: Normal
ms.openlocfilehash: bf6af563a7cc7726a4fa068cb11a7865867406ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888331"
---
# <a name="androidmanagedappregistration-resource-type"></a><span data-ttu-id="cac0d-103">androidManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="cac0d-103">androidManagedAppRegistration resource type</span></span>

> <span data-ttu-id="cac0d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cac0d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cac0d-105">表示特定用户具有管理功能的 Android 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="cac0d-105">Represents the synchronization details of an android app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="cac0d-106">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cac0d-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

<span data-ttu-id="cac0d-107">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-107">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cac0d-108">方法</span><span class="sxs-lookup"><span data-stu-id="cac0d-108">Methods</span></span>
|<span data-ttu-id="cac0d-109">方法</span><span class="sxs-lookup"><span data-stu-id="cac0d-109">Method</span></span>|<span data-ttu-id="cac0d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cac0d-110">Return Type</span></span>|<span data-ttu-id="cac0d-111">说明</span><span class="sxs-lookup"><span data-stu-id="cac0d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cac0d-112">List androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="cac0d-112">List androidManagedAppRegistrations</span></span>](../api/intune-mam-androidmanagedappregistration-list.md)|<span data-ttu-id="cac0d-113">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cac0d-113">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) collection</span></span>|<span data-ttu-id="cac0d-114">列出 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cac0d-114">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="cac0d-115">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cac0d-115">Get androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-get.md)|[<span data-ttu-id="cac0d-116">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cac0d-116">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="cac0d-117">读取 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cac0d-117">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|
|[<span data-ttu-id="cac0d-118">Create androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cac0d-118">Create androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-create.md)|[<span data-ttu-id="cac0d-119">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cac0d-119">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="cac0d-120">创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cac0d-120">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cac0d-121">属性</span><span class="sxs-lookup"><span data-stu-id="cac0d-121">Properties</span></span>
|<span data-ttu-id="cac0d-122">属性</span><span class="sxs-lookup"><span data-stu-id="cac0d-122">Property</span></span>|<span data-ttu-id="cac0d-123">类型</span><span class="sxs-lookup"><span data-stu-id="cac0d-123">Type</span></span>|<span data-ttu-id="cac0d-124">说明</span><span class="sxs-lookup"><span data-stu-id="cac0d-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac0d-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cac0d-125">createdDateTime</span></span>|<span data-ttu-id="cac0d-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cac0d-126">DateTimeOffset</span></span>|<span data-ttu-id="cac0d-127">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-127">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cac0d-128">lastSyncDateTime</span></span>|<span data-ttu-id="cac0d-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cac0d-129">DateTimeOffset</span></span>|<span data-ttu-id="cac0d-130">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cac0d-130">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="cac0d-131">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-131">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="cac0d-132">applicationVersion</span></span>|<span data-ttu-id="cac0d-133">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-133">String</span></span>|<span data-ttu-id="cac0d-134">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-134">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="cac0d-135">managementSdkVersion</span></span>|<span data-ttu-id="cac0d-136">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-136">String</span></span>|<span data-ttu-id="cac0d-137">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-137">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="cac0d-138">platformVersion</span></span>|<span data-ttu-id="cac0d-139">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-139">String</span></span>|<span data-ttu-id="cac0d-140">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-140">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="cac0d-141">deviceType</span></span>|<span data-ttu-id="cac0d-142">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-142">String</span></span>|<span data-ttu-id="cac0d-143">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-143">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="cac0d-144">deviceTag</span></span>|<span data-ttu-id="cac0d-145">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-145">String</span></span>|<span data-ttu-id="cac0d-146">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="cac0d-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="cac0d-147">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="cac0d-147">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="cac0d-148">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-148">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="cac0d-149">deviceName</span></span>|<span data-ttu-id="cac0d-150">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-150">String</span></span>|<span data-ttu-id="cac0d-151">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-151">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-152">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="cac0d-152">flaggedReasons</span></span>|<span data-ttu-id="cac0d-153">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="cac0d-153">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="cac0d-154">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="cac0d-154">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="cac0d-155">例如，</span><span class="sxs-lookup"><span data-stu-id="cac0d-155">E.g.</span></span> <span data-ttu-id="cac0d-156">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-156">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-157">userId</span><span class="sxs-lookup"><span data-stu-id="cac0d-157">userId</span></span>|<span data-ttu-id="cac0d-158">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-158">String</span></span>|<span data-ttu-id="cac0d-159">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="cac0d-159">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="cac0d-160">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-160">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-161">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="cac0d-161">appIdentifier</span></span>|[<span data-ttu-id="cac0d-162">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="cac0d-162">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="cac0d-163">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-163">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-164">id</span><span class="sxs-lookup"><span data-stu-id="cac0d-164">id</span></span>|<span data-ttu-id="cac0d-165">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-165">String</span></span>|<span data-ttu-id="cac0d-166">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cac0d-166">Key of the entity.</span></span> <span data-ttu-id="cac0d-167">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-168">version</span><span class="sxs-lookup"><span data-stu-id="cac0d-168">version</span></span>|<span data-ttu-id="cac0d-169">String</span><span class="sxs-lookup"><span data-stu-id="cac0d-169">String</span></span>|<span data-ttu-id="cac0d-170">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="cac0d-170">Version of the entity.</span></span> <span data-ttu-id="cac0d-171">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-171">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cac0d-172">关系</span><span class="sxs-lookup"><span data-stu-id="cac0d-172">Relationships</span></span>
|<span data-ttu-id="cac0d-173">关系</span><span class="sxs-lookup"><span data-stu-id="cac0d-173">Relationship</span></span>|<span data-ttu-id="cac0d-174">类型</span><span class="sxs-lookup"><span data-stu-id="cac0d-174">Type</span></span>|<span data-ttu-id="cac0d-175">说明</span><span class="sxs-lookup"><span data-stu-id="cac0d-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac0d-176">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="cac0d-176">appliedPolicies</span></span>|<span data-ttu-id="cac0d-177">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cac0d-177">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="cac0d-178">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="cac0d-178">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="cac0d-179">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-179">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-180">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="cac0d-180">intendedPolicies</span></span>|<span data-ttu-id="cac0d-181">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cac0d-181">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="cac0d-182">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="cac0d-182">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="cac0d-183">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-183">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="cac0d-184">operations</span><span class="sxs-lookup"><span data-stu-id="cac0d-184">operations</span></span>|<span data-ttu-id="cac0d-185">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cac0d-185">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="cac0d-186">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="cac0d-186">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="cac0d-187">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="cac0d-187">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cac0d-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cac0d-188">JSON Representation</span></span>
<span data-ttu-id="cac0d-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cac0d-189">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->



