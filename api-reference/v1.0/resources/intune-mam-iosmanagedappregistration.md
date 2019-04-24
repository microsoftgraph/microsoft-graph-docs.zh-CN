---
title: iosManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 iOS 应用的同步详细信息。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29c8798898ea4e3e95ee051348363e0e0ba0ff71
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465487"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="590fa-104">iosManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="590fa-104">iosManagedAppRegistration resource type</span></span>

> <span data-ttu-id="590fa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="590fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="590fa-106">表示特定用户具有管理功能的 iOS 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="590fa-106">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="590fa-107">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="590fa-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="590fa-108">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-108">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="590fa-109">方法</span><span class="sxs-lookup"><span data-stu-id="590fa-109">Methods</span></span>
|<span data-ttu-id="590fa-110">方法</span><span class="sxs-lookup"><span data-stu-id="590fa-110">Method</span></span>|<span data-ttu-id="590fa-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="590fa-111">Return Type</span></span>|<span data-ttu-id="590fa-112">说明</span><span class="sxs-lookup"><span data-stu-id="590fa-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="590fa-113">List iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="590fa-113">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="590fa-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="590fa-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="590fa-115">列出 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="590fa-115">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="590fa-116">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="590fa-116">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="590fa-117">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="590fa-117">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="590fa-118">读取 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="590fa-118">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="590fa-119">属性</span><span class="sxs-lookup"><span data-stu-id="590fa-119">Properties</span></span>
|<span data-ttu-id="590fa-120">属性</span><span class="sxs-lookup"><span data-stu-id="590fa-120">Property</span></span>|<span data-ttu-id="590fa-121">类型</span><span class="sxs-lookup"><span data-stu-id="590fa-121">Type</span></span>|<span data-ttu-id="590fa-122">说明</span><span class="sxs-lookup"><span data-stu-id="590fa-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="590fa-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="590fa-123">createdDateTime</span></span>|<span data-ttu-id="590fa-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590fa-124">DateTimeOffset</span></span>|<span data-ttu-id="590fa-125">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-125">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-126">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="590fa-126">lastSyncDateTime</span></span>|<span data-ttu-id="590fa-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590fa-127">DateTimeOffset</span></span>|<span data-ttu-id="590fa-128">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="590fa-128">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="590fa-129">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-129">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="590fa-130">applicationVersion</span></span>|<span data-ttu-id="590fa-131">字符串</span><span class="sxs-lookup"><span data-stu-id="590fa-131">String</span></span>|<span data-ttu-id="590fa-132">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-132">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="590fa-133">managementSdkVersion</span></span>|<span data-ttu-id="590fa-134">字符串</span><span class="sxs-lookup"><span data-stu-id="590fa-134">String</span></span>|<span data-ttu-id="590fa-135">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-135">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="590fa-136">platformVersion</span></span>|<span data-ttu-id="590fa-137">字符串</span><span class="sxs-lookup"><span data-stu-id="590fa-137">String</span></span>|<span data-ttu-id="590fa-138">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-138">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="590fa-139">deviceType</span></span>|<span data-ttu-id="590fa-140">字符串</span><span class="sxs-lookup"><span data-stu-id="590fa-140">String</span></span>|<span data-ttu-id="590fa-141">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-141">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="590fa-142">deviceTag</span></span>|<span data-ttu-id="590fa-143">String</span><span class="sxs-lookup"><span data-stu-id="590fa-143">String</span></span>|<span data-ttu-id="590fa-144">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="590fa-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="590fa-145">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="590fa-145">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="590fa-146">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-146">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="590fa-147">deviceName</span></span>|<span data-ttu-id="590fa-148">字符串</span><span class="sxs-lookup"><span data-stu-id="590fa-148">String</span></span>|<span data-ttu-id="590fa-149">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-149">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="590fa-150">flaggedReasons</span></span>|<span data-ttu-id="590fa-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="590fa-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="590fa-152">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="590fa-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="590fa-153">例如，</span><span class="sxs-lookup"><span data-stu-id="590fa-153">E.g.</span></span> <span data-ttu-id="590fa-154">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-154">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-155">userId</span><span class="sxs-lookup"><span data-stu-id="590fa-155">userId</span></span>|<span data-ttu-id="590fa-156">String</span><span class="sxs-lookup"><span data-stu-id="590fa-156">String</span></span>|<span data-ttu-id="590fa-157">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="590fa-157">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="590fa-158">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-158">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="590fa-159">appIdentifier</span></span>|[<span data-ttu-id="590fa-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="590fa-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="590fa-161">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-161">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-162">id</span><span class="sxs-lookup"><span data-stu-id="590fa-162">id</span></span>|<span data-ttu-id="590fa-163">String</span><span class="sxs-lookup"><span data-stu-id="590fa-163">String</span></span>|<span data-ttu-id="590fa-164">实体的键。</span><span class="sxs-lookup"><span data-stu-id="590fa-164">Key of the entity.</span></span> <span data-ttu-id="590fa-165">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-165">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-166">version</span><span class="sxs-lookup"><span data-stu-id="590fa-166">version</span></span>|<span data-ttu-id="590fa-167">字符串</span><span class="sxs-lookup"><span data-stu-id="590fa-167">String</span></span>|<span data-ttu-id="590fa-168">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="590fa-168">Version of the entity.</span></span> <span data-ttu-id="590fa-169">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="590fa-170">关系</span><span class="sxs-lookup"><span data-stu-id="590fa-170">Relationships</span></span>
|<span data-ttu-id="590fa-171">关系</span><span class="sxs-lookup"><span data-stu-id="590fa-171">Relationship</span></span>|<span data-ttu-id="590fa-172">类型</span><span class="sxs-lookup"><span data-stu-id="590fa-172">Type</span></span>|<span data-ttu-id="590fa-173">说明</span><span class="sxs-lookup"><span data-stu-id="590fa-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="590fa-174">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="590fa-174">appliedPolicies</span></span>|<span data-ttu-id="590fa-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="590fa-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="590fa-176">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="590fa-176">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="590fa-177">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-177">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-178">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="590fa-178">intendedPolicies</span></span>|<span data-ttu-id="590fa-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="590fa-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="590fa-180">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="590fa-180">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="590fa-181">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-181">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="590fa-182">operations</span><span class="sxs-lookup"><span data-stu-id="590fa-182">operations</span></span>|<span data-ttu-id="590fa-183">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="590fa-183">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="590fa-184">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="590fa-184">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="590fa-185">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="590fa-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="590fa-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="590fa-186">JSON Representation</span></span>
<span data-ttu-id="590fa-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="590fa-187">Here is a JSON representation of the resource.</span></span>
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

