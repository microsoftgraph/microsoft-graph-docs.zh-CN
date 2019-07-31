---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6b259c7a17d769dcaeaa79126c10c028e5d97df7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967957"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="5aee7-104">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="5aee7-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="5aee7-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5aee7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5aee7-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5aee7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5aee7-107">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="5aee7-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="5aee7-108">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5aee7-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="5aee7-109">方法</span><span class="sxs-lookup"><span data-stu-id="5aee7-109">Methods</span></span>
|<span data-ttu-id="5aee7-110">方法</span><span class="sxs-lookup"><span data-stu-id="5aee7-110">Method</span></span>|<span data-ttu-id="5aee7-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5aee7-111">Return Type</span></span>|<span data-ttu-id="5aee7-112">说明</span><span class="sxs-lookup"><span data-stu-id="5aee7-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5aee7-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="5aee7-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="5aee7-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5aee7-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="5aee7-115">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5aee7-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="5aee7-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="5aee7-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="5aee7-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="5aee7-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="5aee7-118">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5aee7-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="5aee7-119">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="5aee7-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="5aee7-120">String collection</span><span class="sxs-lookup"><span data-stu-id="5aee7-120">String collection</span></span>|<span data-ttu-id="5aee7-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5aee7-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5aee7-122">属性</span><span class="sxs-lookup"><span data-stu-id="5aee7-122">Properties</span></span>
|<span data-ttu-id="5aee7-123">属性</span><span class="sxs-lookup"><span data-stu-id="5aee7-123">Property</span></span>|<span data-ttu-id="5aee7-124">类型</span><span class="sxs-lookup"><span data-stu-id="5aee7-124">Type</span></span>|<span data-ttu-id="5aee7-125">说明</span><span class="sxs-lookup"><span data-stu-id="5aee7-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aee7-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5aee7-126">createdDateTime</span></span>|<span data-ttu-id="5aee7-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aee7-127">DateTimeOffset</span></span>|<span data-ttu-id="5aee7-128">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="5aee7-128">Date and time of creation</span></span>|
|<span data-ttu-id="5aee7-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5aee7-129">lastSyncDateTime</span></span>|<span data-ttu-id="5aee7-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aee7-130">DateTimeOffset</span></span>|<span data-ttu-id="5aee7-131">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5aee7-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="5aee7-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="5aee7-132">applicationVersion</span></span>|<span data-ttu-id="5aee7-133">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-133">String</span></span>|<span data-ttu-id="5aee7-134">应用版本</span><span class="sxs-lookup"><span data-stu-id="5aee7-134">App version</span></span>|
|<span data-ttu-id="5aee7-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="5aee7-135">managementSdkVersion</span></span>|<span data-ttu-id="5aee7-136">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-136">String</span></span>|<span data-ttu-id="5aee7-137">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="5aee7-137">App management SDK version</span></span>|
|<span data-ttu-id="5aee7-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="5aee7-138">platformVersion</span></span>|<span data-ttu-id="5aee7-139">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-139">String</span></span>|<span data-ttu-id="5aee7-140">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="5aee7-140">Operating System version</span></span>|
|<span data-ttu-id="5aee7-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="5aee7-141">deviceType</span></span>|<span data-ttu-id="5aee7-142">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-142">String</span></span>|<span data-ttu-id="5aee7-143">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="5aee7-143">Host device type</span></span>|
|<span data-ttu-id="5aee7-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="5aee7-144">deviceTag</span></span>|<span data-ttu-id="5aee7-145">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-145">String</span></span>|<span data-ttu-id="5aee7-146">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="5aee7-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="5aee7-147">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="5aee7-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="5aee7-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="5aee7-148">deviceName</span></span>|<span data-ttu-id="5aee7-149">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-149">String</span></span>|<span data-ttu-id="5aee7-150">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="5aee7-150">Host device name</span></span>|
|<span data-ttu-id="5aee7-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5aee7-151">managedDeviceId</span></span>|<span data-ttu-id="5aee7-152">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-152">String</span></span>|<span data-ttu-id="5aee7-153">主机设备的托管设备标识符。</span><span class="sxs-lookup"><span data-stu-id="5aee7-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="5aee7-154">即使在托管主机设备时, 值也可能为空。</span><span class="sxs-lookup"><span data-stu-id="5aee7-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="5aee7-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="5aee7-155">azureADDeviceId</span></span>|<span data-ttu-id="5aee7-156">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-156">String</span></span>|<span data-ttu-id="5aee7-157">主机设备的 Azure Active Directory 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="5aee7-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="5aee7-158">即使主机设备注册了 Azure Active Directory, 值也可能为空。</span><span class="sxs-lookup"><span data-stu-id="5aee7-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="5aee7-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5aee7-159">deviceModel</span></span>|<span data-ttu-id="5aee7-160">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-160">String</span></span>|<span data-ttu-id="5aee7-161">当前应用程序注册的设备模型</span><span class="sxs-lookup"><span data-stu-id="5aee7-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="5aee7-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="5aee7-162">deviceManufacturer</span></span>|<span data-ttu-id="5aee7-163">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-163">String</span></span>|<span data-ttu-id="5aee7-164">当前应用程序注册的设备制造商</span><span class="sxs-lookup"><span data-stu-id="5aee7-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="5aee7-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="5aee7-165">flaggedReasons</span></span>|<span data-ttu-id="5aee7-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="5aee7-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="5aee7-167">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="5aee7-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="5aee7-168">例如，</span><span class="sxs-lookup"><span data-stu-id="5aee7-168">E.g.</span></span> <span data-ttu-id="5aee7-169">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="5aee7-169">app running on rooted device</span></span>|
|<span data-ttu-id="5aee7-170">userId</span><span class="sxs-lookup"><span data-stu-id="5aee7-170">userId</span></span>|<span data-ttu-id="5aee7-171">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-171">String</span></span>|<span data-ttu-id="5aee7-172">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="5aee7-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="5aee7-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="5aee7-173">appIdentifier</span></span>|[<span data-ttu-id="5aee7-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5aee7-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5aee7-175">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="5aee7-175">The app package Identifier</span></span>|
|<span data-ttu-id="5aee7-176">id</span><span class="sxs-lookup"><span data-stu-id="5aee7-176">id</span></span>|<span data-ttu-id="5aee7-177">字符串</span><span class="sxs-lookup"><span data-stu-id="5aee7-177">String</span></span>|<span data-ttu-id="5aee7-178">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5aee7-178">Key of the entity.</span></span>|
|<span data-ttu-id="5aee7-179">version</span><span class="sxs-lookup"><span data-stu-id="5aee7-179">version</span></span>|<span data-ttu-id="5aee7-180">String</span><span class="sxs-lookup"><span data-stu-id="5aee7-180">String</span></span>|<span data-ttu-id="5aee7-181">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5aee7-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aee7-182">关系</span><span class="sxs-lookup"><span data-stu-id="5aee7-182">Relationships</span></span>
|<span data-ttu-id="5aee7-183">关系</span><span class="sxs-lookup"><span data-stu-id="5aee7-183">Relationship</span></span>|<span data-ttu-id="5aee7-184">类型</span><span class="sxs-lookup"><span data-stu-id="5aee7-184">Type</span></span>|<span data-ttu-id="5aee7-185">说明</span><span class="sxs-lookup"><span data-stu-id="5aee7-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aee7-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="5aee7-186">appliedPolicies</span></span>|<span data-ttu-id="5aee7-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5aee7-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5aee7-188">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="5aee7-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="5aee7-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="5aee7-189">intendedPolicies</span></span>|<span data-ttu-id="5aee7-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5aee7-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5aee7-191">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="5aee7-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="5aee7-192">操作</span><span class="sxs-lookup"><span data-stu-id="5aee7-192">operations</span></span>|<span data-ttu-id="5aee7-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5aee7-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="5aee7-194">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="5aee7-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5aee7-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5aee7-195">JSON Representation</span></span>
<span data-ttu-id="5aee7-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aee7-196">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
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





