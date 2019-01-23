---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a343dba3df1274693449b8f7cbefd83b131138c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421436"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="c74e0-104">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c74e0-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="c74e0-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c74e0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c74e0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c74e0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c74e0-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c74e0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c74e0-108">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="c74e0-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="c74e0-109">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c74e0-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="c74e0-110">方法</span><span class="sxs-lookup"><span data-stu-id="c74e0-110">Methods</span></span>
|<span data-ttu-id="c74e0-111">方法</span><span class="sxs-lookup"><span data-stu-id="c74e0-111">Method</span></span>|<span data-ttu-id="c74e0-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c74e0-112">Return Type</span></span>|<span data-ttu-id="c74e0-113">说明</span><span class="sxs-lookup"><span data-stu-id="c74e0-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c74e0-114">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c74e0-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="c74e0-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c74e0-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="c74e0-116">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c74e0-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="c74e0-117">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c74e0-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="c74e0-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c74e0-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="c74e0-119">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c74e0-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="c74e0-120">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="c74e0-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="c74e0-121">String collection</span><span class="sxs-lookup"><span data-stu-id="c74e0-121">String collection</span></span>|<span data-ttu-id="c74e0-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c74e0-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c74e0-123">属性</span><span class="sxs-lookup"><span data-stu-id="c74e0-123">Properties</span></span>
|<span data-ttu-id="c74e0-124">属性</span><span class="sxs-lookup"><span data-stu-id="c74e0-124">Property</span></span>|<span data-ttu-id="c74e0-125">类型</span><span class="sxs-lookup"><span data-stu-id="c74e0-125">Type</span></span>|<span data-ttu-id="c74e0-126">说明</span><span class="sxs-lookup"><span data-stu-id="c74e0-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c74e0-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c74e0-127">createdDateTime</span></span>|<span data-ttu-id="c74e0-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74e0-128">DateTimeOffset</span></span>|<span data-ttu-id="c74e0-129">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="c74e0-129">Date and time of creation</span></span>|
|<span data-ttu-id="c74e0-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c74e0-130">lastSyncDateTime</span></span>|<span data-ttu-id="c74e0-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74e0-131">DateTimeOffset</span></span>|<span data-ttu-id="c74e0-132">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c74e0-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="c74e0-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c74e0-133">applicationVersion</span></span>|<span data-ttu-id="c74e0-134">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-134">String</span></span>|<span data-ttu-id="c74e0-135">应用版本</span><span class="sxs-lookup"><span data-stu-id="c74e0-135">App version</span></span>|
|<span data-ttu-id="c74e0-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c74e0-136">managementSdkVersion</span></span>|<span data-ttu-id="c74e0-137">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-137">String</span></span>|<span data-ttu-id="c74e0-138">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="c74e0-138">App management SDK version</span></span>|
|<span data-ttu-id="c74e0-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c74e0-139">platformVersion</span></span>|<span data-ttu-id="c74e0-140">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-140">String</span></span>|<span data-ttu-id="c74e0-141">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="c74e0-141">Operating System version</span></span>|
|<span data-ttu-id="c74e0-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="c74e0-142">deviceType</span></span>|<span data-ttu-id="c74e0-143">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-143">String</span></span>|<span data-ttu-id="c74e0-144">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="c74e0-144">Host device type</span></span>|
|<span data-ttu-id="c74e0-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c74e0-145">deviceTag</span></span>|<span data-ttu-id="c74e0-146">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-146">String</span></span>|<span data-ttu-id="c74e0-147">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="c74e0-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c74e0-148">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="c74e0-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="c74e0-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="c74e0-149">deviceName</span></span>|<span data-ttu-id="c74e0-150">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-150">String</span></span>|<span data-ttu-id="c74e0-151">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="c74e0-151">Host device name</span></span>|
|<span data-ttu-id="c74e0-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c74e0-152">managedDeviceId</span></span>|<span data-ttu-id="c74e0-153">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-153">String</span></span>|<span data-ttu-id="c74e0-154">主机设备管理的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c74e0-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="c74e0-155">即使托管主机设备，则可能为空值。</span><span class="sxs-lookup"><span data-stu-id="c74e0-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="c74e0-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="c74e0-156">azureADDeviceId</span></span>|<span data-ttu-id="c74e0-157">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-157">String</span></span>|<span data-ttu-id="c74e0-158">主机设备 Azure Active Directory 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c74e0-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="c74e0-159">即使主机设备注册的 Azure Active Directory，值可能为空。</span><span class="sxs-lookup"><span data-stu-id="c74e0-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="c74e0-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c74e0-160">deviceModel</span></span>|<span data-ttu-id="c74e0-161">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-161">String</span></span>|<span data-ttu-id="c74e0-162">当前应用程序注册设备模型</span><span class="sxs-lookup"><span data-stu-id="c74e0-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="c74e0-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="c74e0-163">deviceManufacturer</span></span>|<span data-ttu-id="c74e0-164">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-164">String</span></span>|<span data-ttu-id="c74e0-165">设备制造商的当前应用程序注册</span><span class="sxs-lookup"><span data-stu-id="c74e0-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="c74e0-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c74e0-166">flaggedReasons</span></span>|<span data-ttu-id="c74e0-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="c74e0-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c74e0-168">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="c74e0-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c74e0-169">例如，</span><span class="sxs-lookup"><span data-stu-id="c74e0-169">E.g.</span></span> <span data-ttu-id="c74e0-170">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="c74e0-170">app running on rooted device</span></span>|
|<span data-ttu-id="c74e0-171">userId</span><span class="sxs-lookup"><span data-stu-id="c74e0-171">userId</span></span>|<span data-ttu-id="c74e0-172">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-172">String</span></span>|<span data-ttu-id="c74e0-173">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="c74e0-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="c74e0-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c74e0-174">appIdentifier</span></span>|[<span data-ttu-id="c74e0-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c74e0-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c74e0-176">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="c74e0-176">The app package Identifier</span></span>|
|<span data-ttu-id="c74e0-177">id</span><span class="sxs-lookup"><span data-stu-id="c74e0-177">id</span></span>|<span data-ttu-id="c74e0-178">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-178">String</span></span>|<span data-ttu-id="c74e0-179">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c74e0-179">Key of the entity.</span></span>|
|<span data-ttu-id="c74e0-180">version</span><span class="sxs-lookup"><span data-stu-id="c74e0-180">version</span></span>|<span data-ttu-id="c74e0-181">String</span><span class="sxs-lookup"><span data-stu-id="c74e0-181">String</span></span>|<span data-ttu-id="c74e0-182">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c74e0-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c74e0-183">关系</span><span class="sxs-lookup"><span data-stu-id="c74e0-183">Relationships</span></span>
|<span data-ttu-id="c74e0-184">关系</span><span class="sxs-lookup"><span data-stu-id="c74e0-184">Relationship</span></span>|<span data-ttu-id="c74e0-185">类型</span><span class="sxs-lookup"><span data-stu-id="c74e0-185">Type</span></span>|<span data-ttu-id="c74e0-186">说明</span><span class="sxs-lookup"><span data-stu-id="c74e0-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c74e0-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c74e0-187">appliedPolicies</span></span>|<span data-ttu-id="c74e0-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c74e0-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c74e0-189">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="c74e0-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="c74e0-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="c74e0-190">intendedPolicies</span></span>|<span data-ttu-id="c74e0-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c74e0-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c74e0-192">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="c74e0-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="c74e0-193">操作</span><span class="sxs-lookup"><span data-stu-id="c74e0-193">operations</span></span>|<span data-ttu-id="c74e0-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c74e0-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="c74e0-195">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="c74e0-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c74e0-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c74e0-196">JSON Representation</span></span>
<span data-ttu-id="c74e0-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c74e0-197">Here is a JSON representation of the resource.</span></span>
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




