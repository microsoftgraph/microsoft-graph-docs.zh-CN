---
title: managedAppRegistration 资源类型
description: 'ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。 '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d6862af09e4bbe1b22d183b8d10c56ff2782f51
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341727"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="2351a-104">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="2351a-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="2351a-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2351a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2351a-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2351a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2351a-107">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="2351a-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="2351a-108">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2351a-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="2351a-109">方法</span><span class="sxs-lookup"><span data-stu-id="2351a-109">Methods</span></span>
|<span data-ttu-id="2351a-110">方法</span><span class="sxs-lookup"><span data-stu-id="2351a-110">Method</span></span>|<span data-ttu-id="2351a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2351a-111">Return Type</span></span>|<span data-ttu-id="2351a-112">说明</span><span class="sxs-lookup"><span data-stu-id="2351a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2351a-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="2351a-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="2351a-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2351a-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="2351a-115">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2351a-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="2351a-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2351a-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="2351a-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2351a-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="2351a-118">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2351a-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="2351a-119">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="2351a-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="2351a-120">String collection</span><span class="sxs-lookup"><span data-stu-id="2351a-120">String collection</span></span>|<span data-ttu-id="2351a-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2351a-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2351a-122">属性</span><span class="sxs-lookup"><span data-stu-id="2351a-122">Properties</span></span>
|<span data-ttu-id="2351a-123">属性</span><span class="sxs-lookup"><span data-stu-id="2351a-123">Property</span></span>|<span data-ttu-id="2351a-124">类型</span><span class="sxs-lookup"><span data-stu-id="2351a-124">Type</span></span>|<span data-ttu-id="2351a-125">说明</span><span class="sxs-lookup"><span data-stu-id="2351a-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2351a-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2351a-126">createdDateTime</span></span>|<span data-ttu-id="2351a-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2351a-127">DateTimeOffset</span></span>|<span data-ttu-id="2351a-128">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="2351a-128">Date and time of creation</span></span>|
|<span data-ttu-id="2351a-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2351a-129">lastSyncDateTime</span></span>|<span data-ttu-id="2351a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2351a-130">DateTimeOffset</span></span>|<span data-ttu-id="2351a-131">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2351a-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="2351a-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="2351a-132">applicationVersion</span></span>|<span data-ttu-id="2351a-133">String</span><span class="sxs-lookup"><span data-stu-id="2351a-133">String</span></span>|<span data-ttu-id="2351a-134">应用版本</span><span class="sxs-lookup"><span data-stu-id="2351a-134">App version</span></span>|
|<span data-ttu-id="2351a-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="2351a-135">managementSdkVersion</span></span>|<span data-ttu-id="2351a-136">String</span><span class="sxs-lookup"><span data-stu-id="2351a-136">String</span></span>|<span data-ttu-id="2351a-137">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="2351a-137">App management SDK version</span></span>|
|<span data-ttu-id="2351a-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="2351a-138">platformVersion</span></span>|<span data-ttu-id="2351a-139">String</span><span class="sxs-lookup"><span data-stu-id="2351a-139">String</span></span>|<span data-ttu-id="2351a-140">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="2351a-140">Operating System version</span></span>|
|<span data-ttu-id="2351a-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="2351a-141">deviceType</span></span>|<span data-ttu-id="2351a-142">String</span><span class="sxs-lookup"><span data-stu-id="2351a-142">String</span></span>|<span data-ttu-id="2351a-143">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="2351a-143">Host device type</span></span>|
|<span data-ttu-id="2351a-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="2351a-144">deviceTag</span></span>|<span data-ttu-id="2351a-145">String</span><span class="sxs-lookup"><span data-stu-id="2351a-145">String</span></span>|<span data-ttu-id="2351a-146">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="2351a-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="2351a-147">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="2351a-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="2351a-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="2351a-148">deviceName</span></span>|<span data-ttu-id="2351a-149">String</span><span class="sxs-lookup"><span data-stu-id="2351a-149">String</span></span>|<span data-ttu-id="2351a-150">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="2351a-150">Host device name</span></span>|
|<span data-ttu-id="2351a-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2351a-151">managedDeviceId</span></span>|<span data-ttu-id="2351a-152">String</span><span class="sxs-lookup"><span data-stu-id="2351a-152">String</span></span>|<span data-ttu-id="2351a-153">主机设备的托管设备标识符。</span><span class="sxs-lookup"><span data-stu-id="2351a-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="2351a-154">即使在托管主机设备时, 值也可能为空。</span><span class="sxs-lookup"><span data-stu-id="2351a-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="2351a-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="2351a-155">azureADDeviceId</span></span>|<span data-ttu-id="2351a-156">String</span><span class="sxs-lookup"><span data-stu-id="2351a-156">String</span></span>|<span data-ttu-id="2351a-157">主机设备的 Azure Active Directory 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="2351a-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="2351a-158">即使主机设备注册了 Azure Active Directory, 值也可能为空。</span><span class="sxs-lookup"><span data-stu-id="2351a-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="2351a-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2351a-159">deviceModel</span></span>|<span data-ttu-id="2351a-160">String</span><span class="sxs-lookup"><span data-stu-id="2351a-160">String</span></span>|<span data-ttu-id="2351a-161">当前应用程序注册的设备模型</span><span class="sxs-lookup"><span data-stu-id="2351a-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="2351a-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="2351a-162">deviceManufacturer</span></span>|<span data-ttu-id="2351a-163">String</span><span class="sxs-lookup"><span data-stu-id="2351a-163">String</span></span>|<span data-ttu-id="2351a-164">当前应用程序注册的设备制造商</span><span class="sxs-lookup"><span data-stu-id="2351a-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="2351a-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="2351a-165">flaggedReasons</span></span>|<span data-ttu-id="2351a-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="2351a-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="2351a-167">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="2351a-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="2351a-168">例如，</span><span class="sxs-lookup"><span data-stu-id="2351a-168">E.g.</span></span> <span data-ttu-id="2351a-169">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="2351a-169">app running on rooted device</span></span>|
|<span data-ttu-id="2351a-170">userId</span><span class="sxs-lookup"><span data-stu-id="2351a-170">userId</span></span>|<span data-ttu-id="2351a-171">String</span><span class="sxs-lookup"><span data-stu-id="2351a-171">String</span></span>|<span data-ttu-id="2351a-172">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2351a-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="2351a-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="2351a-173">appIdentifier</span></span>|[<span data-ttu-id="2351a-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2351a-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="2351a-175">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="2351a-175">The app package Identifier</span></span>|
|<span data-ttu-id="2351a-176">id</span><span class="sxs-lookup"><span data-stu-id="2351a-176">id</span></span>|<span data-ttu-id="2351a-177">字符串</span><span class="sxs-lookup"><span data-stu-id="2351a-177">String</span></span>|<span data-ttu-id="2351a-178">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2351a-178">Key of the entity.</span></span>|
|<span data-ttu-id="2351a-179">version</span><span class="sxs-lookup"><span data-stu-id="2351a-179">version</span></span>|<span data-ttu-id="2351a-180">String</span><span class="sxs-lookup"><span data-stu-id="2351a-180">String</span></span>|<span data-ttu-id="2351a-181">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="2351a-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2351a-182">关系</span><span class="sxs-lookup"><span data-stu-id="2351a-182">Relationships</span></span>
|<span data-ttu-id="2351a-183">关系</span><span class="sxs-lookup"><span data-stu-id="2351a-183">Relationship</span></span>|<span data-ttu-id="2351a-184">类型</span><span class="sxs-lookup"><span data-stu-id="2351a-184">Type</span></span>|<span data-ttu-id="2351a-185">说明</span><span class="sxs-lookup"><span data-stu-id="2351a-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2351a-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="2351a-186">appliedPolicies</span></span>|<span data-ttu-id="2351a-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2351a-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2351a-188">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="2351a-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="2351a-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="2351a-189">intendedPolicies</span></span>|<span data-ttu-id="2351a-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2351a-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2351a-191">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="2351a-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="2351a-192">操作</span><span class="sxs-lookup"><span data-stu-id="2351a-192">operations</span></span>|<span data-ttu-id="2351a-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2351a-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="2351a-194">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="2351a-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2351a-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2351a-195">JSON Representation</span></span>
<span data-ttu-id="2351a-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2351a-196">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration",
  "abstract": true
}-->
``` json
{
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```