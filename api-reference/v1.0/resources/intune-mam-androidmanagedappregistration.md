---
title: androidManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 Android 应用的同步详细信息。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 65d6cb4a0b47ab13e414880a88bdeb0f3526caa1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356581"
---
# <a name="androidmanagedappregistration-resource-type"></a><span data-ttu-id="d5b60-104">androidManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5b60-104">androidManagedAppRegistration resource type</span></span>

> <span data-ttu-id="d5b60-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5b60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b60-106">表示特定用户具有管理功能的 Android 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="d5b60-106">Represents the synchronization details of an android app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="d5b60-107">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d5b60-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="d5b60-108">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-108">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d5b60-109">方法</span><span class="sxs-lookup"><span data-stu-id="d5b60-109">Methods</span></span>
|<span data-ttu-id="d5b60-110">方法</span><span class="sxs-lookup"><span data-stu-id="d5b60-110">Method</span></span>|<span data-ttu-id="d5b60-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5b60-111">Return Type</span></span>|<span data-ttu-id="d5b60-112">说明</span><span class="sxs-lookup"><span data-stu-id="d5b60-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5b60-113">List androidManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d5b60-113">List androidManagedAppRegistrations</span></span>](../api/intune-mam-androidmanagedappregistration-list.md)|<span data-ttu-id="d5b60-114">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5b60-114">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) collection</span></span>|<span data-ttu-id="d5b60-115">列出 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5b60-115">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="d5b60-116">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d5b60-116">Get androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-get.md)|[<span data-ttu-id="d5b60-117">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d5b60-117">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="d5b60-118">读取 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5b60-118">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|
|[<span data-ttu-id="d5b60-119">创建 androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d5b60-119">Create androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-create.md)|[<span data-ttu-id="d5b60-120">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d5b60-120">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="d5b60-121">创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5b60-121">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5b60-122">属性</span><span class="sxs-lookup"><span data-stu-id="d5b60-122">Properties</span></span>
|<span data-ttu-id="d5b60-123">属性</span><span class="sxs-lookup"><span data-stu-id="d5b60-123">Property</span></span>|<span data-ttu-id="d5b60-124">类型</span><span class="sxs-lookup"><span data-stu-id="d5b60-124">Type</span></span>|<span data-ttu-id="d5b60-125">说明</span><span class="sxs-lookup"><span data-stu-id="d5b60-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b60-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5b60-126">createdDateTime</span></span>|<span data-ttu-id="d5b60-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5b60-127">DateTimeOffset</span></span>|<span data-ttu-id="d5b60-128">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-128">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d5b60-129">lastSyncDateTime</span></span>|<span data-ttu-id="d5b60-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5b60-130">DateTimeOffset</span></span>|<span data-ttu-id="d5b60-131">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d5b60-131">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="d5b60-132">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-132">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d5b60-133">applicationVersion</span></span>|<span data-ttu-id="d5b60-134">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-134">String</span></span>|<span data-ttu-id="d5b60-135">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-135">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d5b60-136">managementSdkVersion</span></span>|<span data-ttu-id="d5b60-137">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-137">String</span></span>|<span data-ttu-id="d5b60-138">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-138">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d5b60-139">platformVersion</span></span>|<span data-ttu-id="d5b60-140">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-140">String</span></span>|<span data-ttu-id="d5b60-141">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-141">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="d5b60-142">deviceType</span></span>|<span data-ttu-id="d5b60-143">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-143">String</span></span>|<span data-ttu-id="d5b60-144">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-144">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d5b60-145">deviceTag</span></span>|<span data-ttu-id="d5b60-146">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-146">String</span></span>|<span data-ttu-id="d5b60-147">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="d5b60-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d5b60-148">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="d5b60-148">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="d5b60-149">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-149">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="d5b60-150">deviceName</span></span>|<span data-ttu-id="d5b60-151">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-151">String</span></span>|<span data-ttu-id="d5b60-152">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-152">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-153">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d5b60-153">flaggedReasons</span></span>|<span data-ttu-id="d5b60-154">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="d5b60-154">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d5b60-155">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="d5b60-155">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d5b60-156">例如，</span><span class="sxs-lookup"><span data-stu-id="d5b60-156">E.g.</span></span> <span data-ttu-id="d5b60-157">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-157">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-158">userId</span><span class="sxs-lookup"><span data-stu-id="d5b60-158">userId</span></span>|<span data-ttu-id="d5b60-159">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-159">String</span></span>|<span data-ttu-id="d5b60-160">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d5b60-160">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="d5b60-161">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-161">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-162">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5b60-162">appIdentifier</span></span>|[<span data-ttu-id="d5b60-163">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5b60-163">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d5b60-164">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-164">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-165">id</span><span class="sxs-lookup"><span data-stu-id="d5b60-165">id</span></span>|<span data-ttu-id="d5b60-166">字符串</span><span class="sxs-lookup"><span data-stu-id="d5b60-166">String</span></span>|<span data-ttu-id="d5b60-167">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d5b60-167">Key of the entity.</span></span> <span data-ttu-id="d5b60-168">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-169">version</span><span class="sxs-lookup"><span data-stu-id="d5b60-169">version</span></span>|<span data-ttu-id="d5b60-170">String</span><span class="sxs-lookup"><span data-stu-id="d5b60-170">String</span></span>|<span data-ttu-id="d5b60-171">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d5b60-171">Version of the entity.</span></span> <span data-ttu-id="d5b60-172">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-172">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5b60-173">关系</span><span class="sxs-lookup"><span data-stu-id="d5b60-173">Relationships</span></span>
|<span data-ttu-id="d5b60-174">关系</span><span class="sxs-lookup"><span data-stu-id="d5b60-174">Relationship</span></span>|<span data-ttu-id="d5b60-175">类型</span><span class="sxs-lookup"><span data-stu-id="d5b60-175">Type</span></span>|<span data-ttu-id="d5b60-176">说明</span><span class="sxs-lookup"><span data-stu-id="d5b60-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b60-177">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="d5b60-177">appliedPolicies</span></span>|<span data-ttu-id="d5b60-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5b60-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d5b60-179">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="d5b60-179">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="d5b60-180">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-180">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-181">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="d5b60-181">intendedPolicies</span></span>|<span data-ttu-id="d5b60-182">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5b60-182">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d5b60-183">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="d5b60-183">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="d5b60-184">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d5b60-185">operations</span><span class="sxs-lookup"><span data-stu-id="d5b60-185">operations</span></span>|<span data-ttu-id="d5b60-186">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5b60-186">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d5b60-187">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="d5b60-187">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="d5b60-188">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d5b60-188">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5b60-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5b60-189">JSON Representation</span></span>
<span data-ttu-id="d5b60-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5b60-190">Here is a JSON representation of the resource.</span></span>
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
 

