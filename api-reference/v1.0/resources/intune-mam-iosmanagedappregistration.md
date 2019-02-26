---
title: iosManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 iOS 应用的同步详细信息。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29c8798898ea4e3e95ee051348363e0e0ba0ff71
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253671"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="5582b-104">iosManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="5582b-104">iosManagedAppRegistration resource type</span></span>

> <span data-ttu-id="5582b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5582b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5582b-106">表示特定用户具有管理功能的 iOS 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="5582b-106">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="5582b-107">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5582b-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="5582b-108">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-108">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5582b-109">方法</span><span class="sxs-lookup"><span data-stu-id="5582b-109">Methods</span></span>
|<span data-ttu-id="5582b-110">方法</span><span class="sxs-lookup"><span data-stu-id="5582b-110">Method</span></span>|<span data-ttu-id="5582b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5582b-111">Return Type</span></span>|<span data-ttu-id="5582b-112">说明</span><span class="sxs-lookup"><span data-stu-id="5582b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5582b-113">List iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="5582b-113">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="5582b-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5582b-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="5582b-115">列出 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5582b-115">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="5582b-116">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="5582b-116">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="5582b-117">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="5582b-117">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="5582b-118">读取 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5582b-118">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5582b-119">属性</span><span class="sxs-lookup"><span data-stu-id="5582b-119">Properties</span></span>
|<span data-ttu-id="5582b-120">属性</span><span class="sxs-lookup"><span data-stu-id="5582b-120">Property</span></span>|<span data-ttu-id="5582b-121">类型</span><span class="sxs-lookup"><span data-stu-id="5582b-121">Type</span></span>|<span data-ttu-id="5582b-122">说明</span><span class="sxs-lookup"><span data-stu-id="5582b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5582b-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5582b-123">createdDateTime</span></span>|<span data-ttu-id="5582b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5582b-124">DateTimeOffset</span></span>|<span data-ttu-id="5582b-125">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-125">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-126">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5582b-126">lastSyncDateTime</span></span>|<span data-ttu-id="5582b-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5582b-127">DateTimeOffset</span></span>|<span data-ttu-id="5582b-128">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5582b-128">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="5582b-129">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-129">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="5582b-130">applicationVersion</span></span>|<span data-ttu-id="5582b-131">String</span><span class="sxs-lookup"><span data-stu-id="5582b-131">String</span></span>|<span data-ttu-id="5582b-132">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-132">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="5582b-133">managementSdkVersion</span></span>|<span data-ttu-id="5582b-134">String</span><span class="sxs-lookup"><span data-stu-id="5582b-134">String</span></span>|<span data-ttu-id="5582b-135">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-135">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="5582b-136">platformVersion</span></span>|<span data-ttu-id="5582b-137">String</span><span class="sxs-lookup"><span data-stu-id="5582b-137">String</span></span>|<span data-ttu-id="5582b-138">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-138">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="5582b-139">deviceType</span></span>|<span data-ttu-id="5582b-140">String</span><span class="sxs-lookup"><span data-stu-id="5582b-140">String</span></span>|<span data-ttu-id="5582b-141">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-141">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="5582b-142">deviceTag</span></span>|<span data-ttu-id="5582b-143">String</span><span class="sxs-lookup"><span data-stu-id="5582b-143">String</span></span>|<span data-ttu-id="5582b-144">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="5582b-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="5582b-145">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="5582b-145">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="5582b-146">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-146">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="5582b-147">deviceName</span></span>|<span data-ttu-id="5582b-148">String</span><span class="sxs-lookup"><span data-stu-id="5582b-148">String</span></span>|<span data-ttu-id="5582b-149">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-149">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="5582b-150">flaggedReasons</span></span>|<span data-ttu-id="5582b-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="5582b-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="5582b-152">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="5582b-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="5582b-153">例如，</span><span class="sxs-lookup"><span data-stu-id="5582b-153">E.g.</span></span> <span data-ttu-id="5582b-154">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-154">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-155">userId</span><span class="sxs-lookup"><span data-stu-id="5582b-155">userId</span></span>|<span data-ttu-id="5582b-156">String</span><span class="sxs-lookup"><span data-stu-id="5582b-156">String</span></span>|<span data-ttu-id="5582b-157">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="5582b-157">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="5582b-158">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-158">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="5582b-159">appIdentifier</span></span>|[<span data-ttu-id="5582b-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5582b-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5582b-161">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-161">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-162">id</span><span class="sxs-lookup"><span data-stu-id="5582b-162">id</span></span>|<span data-ttu-id="5582b-163">字符串</span><span class="sxs-lookup"><span data-stu-id="5582b-163">String</span></span>|<span data-ttu-id="5582b-164">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5582b-164">Key of the entity.</span></span> <span data-ttu-id="5582b-165">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-165">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-166">version</span><span class="sxs-lookup"><span data-stu-id="5582b-166">version</span></span>|<span data-ttu-id="5582b-167">String</span><span class="sxs-lookup"><span data-stu-id="5582b-167">String</span></span>|<span data-ttu-id="5582b-168">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5582b-168">Version of the entity.</span></span> <span data-ttu-id="5582b-169">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5582b-170">关系</span><span class="sxs-lookup"><span data-stu-id="5582b-170">Relationships</span></span>
|<span data-ttu-id="5582b-171">关系</span><span class="sxs-lookup"><span data-stu-id="5582b-171">Relationship</span></span>|<span data-ttu-id="5582b-172">类型</span><span class="sxs-lookup"><span data-stu-id="5582b-172">Type</span></span>|<span data-ttu-id="5582b-173">说明</span><span class="sxs-lookup"><span data-stu-id="5582b-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5582b-174">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="5582b-174">appliedPolicies</span></span>|<span data-ttu-id="5582b-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5582b-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5582b-176">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="5582b-176">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="5582b-177">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-177">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-178">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="5582b-178">intendedPolicies</span></span>|<span data-ttu-id="5582b-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5582b-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5582b-180">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="5582b-180">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="5582b-181">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-181">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="5582b-182">operations</span><span class="sxs-lookup"><span data-stu-id="5582b-182">operations</span></span>|<span data-ttu-id="5582b-183">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5582b-183">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="5582b-184">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="5582b-184">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="5582b-185">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5582b-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5582b-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5582b-186">JSON Representation</span></span>
<span data-ttu-id="5582b-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5582b-187">Here is a JSON representation of the resource.</span></span>
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

