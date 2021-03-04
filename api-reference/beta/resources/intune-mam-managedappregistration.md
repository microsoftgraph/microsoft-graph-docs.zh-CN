---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d527b4d0a6da5a54a6e167db063b8c4e06a6062
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444180"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="410ec-104">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="410ec-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="410ec-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="410ec-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="410ec-106">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="410ec-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="410ec-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="410ec-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="410ec-108">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="410ec-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="410ec-109">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="410ec-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="410ec-110">Methods</span><span class="sxs-lookup"><span data-stu-id="410ec-110">Methods</span></span>
|<span data-ttu-id="410ec-111">方法</span><span class="sxs-lookup"><span data-stu-id="410ec-111">Method</span></span>|<span data-ttu-id="410ec-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="410ec-112">Return Type</span></span>|<span data-ttu-id="410ec-113">说明</span><span class="sxs-lookup"><span data-stu-id="410ec-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="410ec-114">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="410ec-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="410ec-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="410ec-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="410ec-116">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="410ec-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="410ec-117">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="410ec-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="410ec-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="410ec-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="410ec-119">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="410ec-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="410ec-120">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="410ec-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="410ec-121">String collection</span><span class="sxs-lookup"><span data-stu-id="410ec-121">String collection</span></span>|<span data-ttu-id="410ec-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="410ec-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="410ec-123">属性</span><span class="sxs-lookup"><span data-stu-id="410ec-123">Properties</span></span>
|<span data-ttu-id="410ec-124">属性</span><span class="sxs-lookup"><span data-stu-id="410ec-124">Property</span></span>|<span data-ttu-id="410ec-125">类型</span><span class="sxs-lookup"><span data-stu-id="410ec-125">Type</span></span>|<span data-ttu-id="410ec-126">说明</span><span class="sxs-lookup"><span data-stu-id="410ec-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="410ec-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="410ec-127">createdDateTime</span></span>|<span data-ttu-id="410ec-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="410ec-128">DateTimeOffset</span></span>|<span data-ttu-id="410ec-129">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="410ec-129">Date and time of creation</span></span>|
|<span data-ttu-id="410ec-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="410ec-130">lastSyncDateTime</span></span>|<span data-ttu-id="410ec-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="410ec-131">DateTimeOffset</span></span>|<span data-ttu-id="410ec-132">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="410ec-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="410ec-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="410ec-133">applicationVersion</span></span>|<span data-ttu-id="410ec-134">String</span><span class="sxs-lookup"><span data-stu-id="410ec-134">String</span></span>|<span data-ttu-id="410ec-135">应用版本</span><span class="sxs-lookup"><span data-stu-id="410ec-135">App version</span></span>|
|<span data-ttu-id="410ec-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="410ec-136">managementSdkVersion</span></span>|<span data-ttu-id="410ec-137">String</span><span class="sxs-lookup"><span data-stu-id="410ec-137">String</span></span>|<span data-ttu-id="410ec-138">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="410ec-138">App management SDK version</span></span>|
|<span data-ttu-id="410ec-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="410ec-139">platformVersion</span></span>|<span data-ttu-id="410ec-140">String</span><span class="sxs-lookup"><span data-stu-id="410ec-140">String</span></span>|<span data-ttu-id="410ec-141">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="410ec-141">Operating System version</span></span>|
|<span data-ttu-id="410ec-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="410ec-142">deviceType</span></span>|<span data-ttu-id="410ec-143">String</span><span class="sxs-lookup"><span data-stu-id="410ec-143">String</span></span>|<span data-ttu-id="410ec-144">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="410ec-144">Host device type</span></span>|
|<span data-ttu-id="410ec-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="410ec-145">deviceTag</span></span>|<span data-ttu-id="410ec-146">String</span><span class="sxs-lookup"><span data-stu-id="410ec-146">String</span></span>|<span data-ttu-id="410ec-147">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="410ec-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="410ec-148">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="410ec-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="410ec-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="410ec-149">deviceName</span></span>|<span data-ttu-id="410ec-150">String</span><span class="sxs-lookup"><span data-stu-id="410ec-150">String</span></span>|<span data-ttu-id="410ec-151">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="410ec-151">Host device name</span></span>|
|<span data-ttu-id="410ec-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="410ec-152">managedDeviceId</span></span>|<span data-ttu-id="410ec-153">String</span><span class="sxs-lookup"><span data-stu-id="410ec-153">String</span></span>|<span data-ttu-id="410ec-154">主机设备的托管设备标识符。</span><span class="sxs-lookup"><span data-stu-id="410ec-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="410ec-155">即使托管主机设备，值也可以为空。</span><span class="sxs-lookup"><span data-stu-id="410ec-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="410ec-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="410ec-156">azureADDeviceId</span></span>|<span data-ttu-id="410ec-157">String</span><span class="sxs-lookup"><span data-stu-id="410ec-157">String</span></span>|<span data-ttu-id="410ec-158">主机设备的 Azure Active Directory 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="410ec-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="410ec-159">即使主机设备已注册 Azure Active Directory，值也可以为空。</span><span class="sxs-lookup"><span data-stu-id="410ec-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="410ec-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="410ec-160">deviceModel</span></span>|<span data-ttu-id="410ec-161">String</span><span class="sxs-lookup"><span data-stu-id="410ec-161">String</span></span>|<span data-ttu-id="410ec-162">当前应用注册的设备模型</span><span class="sxs-lookup"><span data-stu-id="410ec-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="410ec-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="410ec-163">deviceManufacturer</span></span>|<span data-ttu-id="410ec-164">String</span><span class="sxs-lookup"><span data-stu-id="410ec-164">String</span></span>|<span data-ttu-id="410ec-165">用于当前应用注册的设备制造商</span><span class="sxs-lookup"><span data-stu-id="410ec-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="410ec-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="410ec-166">flaggedReasons</span></span>|<span data-ttu-id="410ec-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="410ec-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="410ec-168">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="410ec-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="410ec-169">例如，</span><span class="sxs-lookup"><span data-stu-id="410ec-169">E.g.</span></span> <span data-ttu-id="410ec-170">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="410ec-170">app running on rooted device</span></span>|
|<span data-ttu-id="410ec-171">userId</span><span class="sxs-lookup"><span data-stu-id="410ec-171">userId</span></span>|<span data-ttu-id="410ec-172">String</span><span class="sxs-lookup"><span data-stu-id="410ec-172">String</span></span>|<span data-ttu-id="410ec-173">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="410ec-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="410ec-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="410ec-174">appIdentifier</span></span>|[<span data-ttu-id="410ec-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="410ec-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="410ec-176">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="410ec-176">The app package Identifier</span></span>|
|<span data-ttu-id="410ec-177">id</span><span class="sxs-lookup"><span data-stu-id="410ec-177">id</span></span>|<span data-ttu-id="410ec-178">String</span><span class="sxs-lookup"><span data-stu-id="410ec-178">String</span></span>|<span data-ttu-id="410ec-179">实体的键。</span><span class="sxs-lookup"><span data-stu-id="410ec-179">Key of the entity.</span></span>|
|<span data-ttu-id="410ec-180">version</span><span class="sxs-lookup"><span data-stu-id="410ec-180">version</span></span>|<span data-ttu-id="410ec-181">String</span><span class="sxs-lookup"><span data-stu-id="410ec-181">String</span></span>|<span data-ttu-id="410ec-182">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="410ec-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="410ec-183">关系</span><span class="sxs-lookup"><span data-stu-id="410ec-183">Relationships</span></span>
|<span data-ttu-id="410ec-184">关系</span><span class="sxs-lookup"><span data-stu-id="410ec-184">Relationship</span></span>|<span data-ttu-id="410ec-185">类型</span><span class="sxs-lookup"><span data-stu-id="410ec-185">Type</span></span>|<span data-ttu-id="410ec-186">说明</span><span class="sxs-lookup"><span data-stu-id="410ec-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="410ec-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="410ec-187">appliedPolicies</span></span>|<span data-ttu-id="410ec-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="410ec-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="410ec-189">注册应用上次与管理服务同步时，已应用零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="410ec-189">Zero or more policys already applied on the registered app when it last synchronized with management service.</span></span>|
|<span data-ttu-id="410ec-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="410ec-190">intendedPolicies</span></span>|<span data-ttu-id="410ec-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="410ec-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="410ec-192">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="410ec-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="410ec-193">操作</span><span class="sxs-lookup"><span data-stu-id="410ec-193">operations</span></span>|<span data-ttu-id="410ec-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="410ec-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="410ec-195">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="410ec-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="410ec-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="410ec-196">JSON Representation</span></span>
<span data-ttu-id="410ec-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="410ec-197">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




