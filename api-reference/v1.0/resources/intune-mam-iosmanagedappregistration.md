---
title: iosManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 iOS 应用的同步详细信息。
localization_priority: Normal
ms.openlocfilehash: eb36bf1e96a8b7a54daf9d02b4cc2765a1844d4c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868066"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="6bd7e-103">iosManagedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bd7e-103">iosManagedAppRegistration resource type</span></span>

> <span data-ttu-id="6bd7e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bd7e-105">表示特定用户具有管理功能的 iOS 应用的同步详细信息。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-105">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="6bd7e-106">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

<span data-ttu-id="6bd7e-107">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-107">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6bd7e-108">方法</span><span class="sxs-lookup"><span data-stu-id="6bd7e-108">Methods</span></span>
|<span data-ttu-id="6bd7e-109">方法</span><span class="sxs-lookup"><span data-stu-id="6bd7e-109">Method</span></span>|<span data-ttu-id="6bd7e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6bd7e-110">Return Type</span></span>|<span data-ttu-id="6bd7e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6bd7e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bd7e-112">List iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="6bd7e-112">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="6bd7e-113">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bd7e-113">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="6bd7e-114">列出 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-114">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="6bd7e-115">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6bd7e-115">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="6bd7e-116">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6bd7e-116">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="6bd7e-117">读取 [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-117">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bd7e-118">属性</span><span class="sxs-lookup"><span data-stu-id="6bd7e-118">Properties</span></span>
|<span data-ttu-id="6bd7e-119">属性</span><span class="sxs-lookup"><span data-stu-id="6bd7e-119">Property</span></span>|<span data-ttu-id="6bd7e-120">类型</span><span class="sxs-lookup"><span data-stu-id="6bd7e-120">Type</span></span>|<span data-ttu-id="6bd7e-121">说明</span><span class="sxs-lookup"><span data-stu-id="6bd7e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bd7e-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bd7e-122">createdDateTime</span></span>|<span data-ttu-id="6bd7e-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bd7e-123">DateTimeOffset</span></span>|<span data-ttu-id="6bd7e-124">创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-124">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6bd7e-125">lastSyncDateTime</span></span>|<span data-ttu-id="6bd7e-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bd7e-126">DateTimeOffset</span></span>|<span data-ttu-id="6bd7e-127">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-127">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="6bd7e-128">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-128">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-129">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="6bd7e-129">applicationVersion</span></span>|<span data-ttu-id="6bd7e-130">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-130">String</span></span>|<span data-ttu-id="6bd7e-131">应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-131">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-132">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6bd7e-132">managementSdkVersion</span></span>|<span data-ttu-id="6bd7e-133">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-133">String</span></span>|<span data-ttu-id="6bd7e-134">应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-134">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-135">platformVersion</span><span class="sxs-lookup"><span data-stu-id="6bd7e-135">platformVersion</span></span>|<span data-ttu-id="6bd7e-136">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-136">String</span></span>|<span data-ttu-id="6bd7e-137">操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-137">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="6bd7e-138">deviceType</span></span>|<span data-ttu-id="6bd7e-139">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-139">String</span></span>|<span data-ttu-id="6bd7e-140">主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-140">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-141">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6bd7e-141">deviceTag</span></span>|<span data-ttu-id="6bd7e-142">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-142">String</span></span>|<span data-ttu-id="6bd7e-143">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-143">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="6bd7e-144">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-144">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="6bd7e-145">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-145">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="6bd7e-146">deviceName</span></span>|<span data-ttu-id="6bd7e-147">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-147">String</span></span>|<span data-ttu-id="6bd7e-148">主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-148">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="6bd7e-149">flaggedReasons</span></span>|<span data-ttu-id="6bd7e-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bd7e-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="6bd7e-151">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="6bd7e-152">例如，</span><span class="sxs-lookup"><span data-stu-id="6bd7e-152">E.g.</span></span> <span data-ttu-id="6bd7e-153">应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-153">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-154">userId</span><span class="sxs-lookup"><span data-stu-id="6bd7e-154">userId</span></span>|<span data-ttu-id="6bd7e-155">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-155">String</span></span>|<span data-ttu-id="6bd7e-156">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-156">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="6bd7e-157">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-157">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6bd7e-158">appIdentifier</span></span>|[<span data-ttu-id="6bd7e-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6bd7e-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6bd7e-160">应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-160">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-161">id</span><span class="sxs-lookup"><span data-stu-id="6bd7e-161">id</span></span>|<span data-ttu-id="6bd7e-162">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-162">String</span></span>|<span data-ttu-id="6bd7e-163">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-163">Key of the entity.</span></span> <span data-ttu-id="6bd7e-164">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-165">version</span><span class="sxs-lookup"><span data-stu-id="6bd7e-165">version</span></span>|<span data-ttu-id="6bd7e-166">String</span><span class="sxs-lookup"><span data-stu-id="6bd7e-166">String</span></span>|<span data-ttu-id="6bd7e-167">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-167">Version of the entity.</span></span> <span data-ttu-id="6bd7e-168">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bd7e-169">关系</span><span class="sxs-lookup"><span data-stu-id="6bd7e-169">Relationships</span></span>
|<span data-ttu-id="6bd7e-170">关系</span><span class="sxs-lookup"><span data-stu-id="6bd7e-170">Relationship</span></span>|<span data-ttu-id="6bd7e-171">类型</span><span class="sxs-lookup"><span data-stu-id="6bd7e-171">Type</span></span>|<span data-ttu-id="6bd7e-172">说明</span><span class="sxs-lookup"><span data-stu-id="6bd7e-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bd7e-173">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="6bd7e-173">appliedPolicies</span></span>|<span data-ttu-id="6bd7e-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bd7e-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6bd7e-175">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-175">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="6bd7e-176">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-176">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-177">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="6bd7e-177">intendedPolicies</span></span>|<span data-ttu-id="6bd7e-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bd7e-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6bd7e-179">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-179">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="6bd7e-180">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-180">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6bd7e-181">operations</span><span class="sxs-lookup"><span data-stu-id="6bd7e-181">operations</span></span>|<span data-ttu-id="6bd7e-182">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bd7e-182">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="6bd7e-183">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-183">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="6bd7e-184">继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6bd7e-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bd7e-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bd7e-185">JSON Representation</span></span>
<span data-ttu-id="6bd7e-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bd7e-186">Here is a JSON representation of the resource.</span></span>
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
