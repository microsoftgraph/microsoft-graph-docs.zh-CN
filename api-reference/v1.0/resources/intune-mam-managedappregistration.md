---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a7b10a7d960c449aee4f911f4992955bde18724
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037910"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="3bc3c-104">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="3bc3c-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="3bc3c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bc3c-106">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="3bc3c-107">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="3bc3c-108">方法</span><span class="sxs-lookup"><span data-stu-id="3bc3c-108">Methods</span></span>
|<span data-ttu-id="3bc3c-109">方法</span><span class="sxs-lookup"><span data-stu-id="3bc3c-109">Method</span></span>|<span data-ttu-id="3bc3c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3bc3c-110">Return Type</span></span>|<span data-ttu-id="3bc3c-111">说明</span><span class="sxs-lookup"><span data-stu-id="3bc3c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3bc3c-112">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="3bc3c-112">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="3bc3c-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bc3c-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="3bc3c-114">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-114">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="3bc3c-115">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="3bc3c-115">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="3bc3c-116">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="3bc3c-116">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="3bc3c-117">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-117">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="3bc3c-118">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="3bc3c-118">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="3bc3c-119">String collection</span><span class="sxs-lookup"><span data-stu-id="3bc3c-119">String collection</span></span>|<span data-ttu-id="3bc3c-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3bc3c-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3bc3c-121">属性</span><span class="sxs-lookup"><span data-stu-id="3bc3c-121">Properties</span></span>
|<span data-ttu-id="3bc3c-122">属性</span><span class="sxs-lookup"><span data-stu-id="3bc3c-122">Property</span></span>|<span data-ttu-id="3bc3c-123">类型</span><span class="sxs-lookup"><span data-stu-id="3bc3c-123">Type</span></span>|<span data-ttu-id="3bc3c-124">说明</span><span class="sxs-lookup"><span data-stu-id="3bc3c-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bc3c-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc3c-125">createdDateTime</span></span>|<span data-ttu-id="3bc3c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc3c-126">DateTimeOffset</span></span>|<span data-ttu-id="3bc3c-127">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="3bc3c-127">Date and time of creation</span></span>|
|<span data-ttu-id="3bc3c-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc3c-128">lastSyncDateTime</span></span>|<span data-ttu-id="3bc3c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc3c-129">DateTimeOffset</span></span>|<span data-ttu-id="3bc3c-130">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-130">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="3bc3c-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="3bc3c-131">applicationVersion</span></span>|<span data-ttu-id="3bc3c-132">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-132">String</span></span>|<span data-ttu-id="3bc3c-133">应用版本</span><span class="sxs-lookup"><span data-stu-id="3bc3c-133">App version</span></span>|
|<span data-ttu-id="3bc3c-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="3bc3c-134">managementSdkVersion</span></span>|<span data-ttu-id="3bc3c-135">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-135">String</span></span>|<span data-ttu-id="3bc3c-136">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="3bc3c-136">App management SDK version</span></span>|
|<span data-ttu-id="3bc3c-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="3bc3c-137">platformVersion</span></span>|<span data-ttu-id="3bc3c-138">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-138">String</span></span>|<span data-ttu-id="3bc3c-139">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="3bc3c-139">Operating System version</span></span>|
|<span data-ttu-id="3bc3c-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="3bc3c-140">deviceType</span></span>|<span data-ttu-id="3bc3c-141">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-141">String</span></span>|<span data-ttu-id="3bc3c-142">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="3bc3c-142">Host device type</span></span>|
|<span data-ttu-id="3bc3c-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="3bc3c-143">deviceTag</span></span>|<span data-ttu-id="3bc3c-144">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-144">String</span></span>|<span data-ttu-id="3bc3c-145">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="3bc3c-146">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-146">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="3bc3c-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="3bc3c-147">deviceName</span></span>|<span data-ttu-id="3bc3c-148">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-148">String</span></span>|<span data-ttu-id="3bc3c-149">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="3bc3c-149">Host device name</span></span>|
|<span data-ttu-id="3bc3c-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="3bc3c-150">flaggedReasons</span></span>|<span data-ttu-id="3bc3c-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="3bc3c-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="3bc3c-152">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="3bc3c-153">例如，</span><span class="sxs-lookup"><span data-stu-id="3bc3c-153">E.g.</span></span> <span data-ttu-id="3bc3c-154">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="3bc3c-154">app running on rooted device</span></span>|
|<span data-ttu-id="3bc3c-155">userId</span><span class="sxs-lookup"><span data-stu-id="3bc3c-155">userId</span></span>|<span data-ttu-id="3bc3c-156">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-156">String</span></span>|<span data-ttu-id="3bc3c-157">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-157">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="3bc3c-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="3bc3c-158">appIdentifier</span></span>|[<span data-ttu-id="3bc3c-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="3bc3c-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="3bc3c-160">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="3bc3c-160">The app package Identifier</span></span>|
|<span data-ttu-id="3bc3c-161">id</span><span class="sxs-lookup"><span data-stu-id="3bc3c-161">id</span></span>|<span data-ttu-id="3bc3c-162">字符串</span><span class="sxs-lookup"><span data-stu-id="3bc3c-162">String</span></span>|<span data-ttu-id="3bc3c-163">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-163">Key of the entity.</span></span>|
|<span data-ttu-id="3bc3c-164">version</span><span class="sxs-lookup"><span data-stu-id="3bc3c-164">version</span></span>|<span data-ttu-id="3bc3c-165">String</span><span class="sxs-lookup"><span data-stu-id="3bc3c-165">String</span></span>|<span data-ttu-id="3bc3c-166">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-166">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bc3c-167">关系</span><span class="sxs-lookup"><span data-stu-id="3bc3c-167">Relationships</span></span>
|<span data-ttu-id="3bc3c-168">关系</span><span class="sxs-lookup"><span data-stu-id="3bc3c-168">Relationship</span></span>|<span data-ttu-id="3bc3c-169">类型</span><span class="sxs-lookup"><span data-stu-id="3bc3c-169">Type</span></span>|<span data-ttu-id="3bc3c-170">说明</span><span class="sxs-lookup"><span data-stu-id="3bc3c-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bc3c-171">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="3bc3c-171">appliedPolicies</span></span>|<span data-ttu-id="3bc3c-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bc3c-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="3bc3c-173">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-173">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="3bc3c-174">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="3bc3c-174">intendedPolicies</span></span>|<span data-ttu-id="3bc3c-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bc3c-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="3bc3c-176">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-176">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="3bc3c-177">操作</span><span class="sxs-lookup"><span data-stu-id="3bc3c-177">operations</span></span>|<span data-ttu-id="3bc3c-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bc3c-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="3bc3c-179">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-179">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bc3c-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bc3c-180">JSON Representation</span></span>
<span data-ttu-id="3bc3c-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bc3c-181">Here is a JSON representation of the resource.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


