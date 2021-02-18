---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8d2c9043e9283258b904cef1a61a3ce502f69601
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291893"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="9fb6c-104">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fb6c-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="9fb6c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fb6c-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fb6c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fb6c-107">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="9fb6c-108">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="9fb6c-109">方法</span><span class="sxs-lookup"><span data-stu-id="9fb6c-109">Methods</span></span>
|<span data-ttu-id="9fb6c-110">方法</span><span class="sxs-lookup"><span data-stu-id="9fb6c-110">Method</span></span>|<span data-ttu-id="9fb6c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9fb6c-111">Return Type</span></span>|<span data-ttu-id="9fb6c-112">说明</span><span class="sxs-lookup"><span data-stu-id="9fb6c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9fb6c-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="9fb6c-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="9fb6c-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fb6c-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="9fb6c-115">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="9fb6c-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9fb6c-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="9fb6c-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9fb6c-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="9fb6c-118">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="9fb6c-119">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="9fb6c-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="9fb6c-120">String collection</span><span class="sxs-lookup"><span data-stu-id="9fb6c-120">String collection</span></span>|<span data-ttu-id="9fb6c-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9fb6c-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9fb6c-122">属性</span><span class="sxs-lookup"><span data-stu-id="9fb6c-122">Properties</span></span>
|<span data-ttu-id="9fb6c-123">属性</span><span class="sxs-lookup"><span data-stu-id="9fb6c-123">Property</span></span>|<span data-ttu-id="9fb6c-124">类型</span><span class="sxs-lookup"><span data-stu-id="9fb6c-124">Type</span></span>|<span data-ttu-id="9fb6c-125">说明</span><span class="sxs-lookup"><span data-stu-id="9fb6c-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fb6c-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fb6c-126">createdDateTime</span></span>|<span data-ttu-id="9fb6c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fb6c-127">DateTimeOffset</span></span>|<span data-ttu-id="9fb6c-128">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="9fb6c-128">Date and time of creation</span></span>|
|<span data-ttu-id="9fb6c-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9fb6c-129">lastSyncDateTime</span></span>|<span data-ttu-id="9fb6c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fb6c-130">DateTimeOffset</span></span>|<span data-ttu-id="9fb6c-131">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="9fb6c-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="9fb6c-132">applicationVersion</span></span>|<span data-ttu-id="9fb6c-133">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-133">String</span></span>|<span data-ttu-id="9fb6c-134">应用版本</span><span class="sxs-lookup"><span data-stu-id="9fb6c-134">App version</span></span>|
|<span data-ttu-id="9fb6c-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="9fb6c-135">managementSdkVersion</span></span>|<span data-ttu-id="9fb6c-136">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-136">String</span></span>|<span data-ttu-id="9fb6c-137">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="9fb6c-137">App management SDK version</span></span>|
|<span data-ttu-id="9fb6c-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="9fb6c-138">platformVersion</span></span>|<span data-ttu-id="9fb6c-139">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-139">String</span></span>|<span data-ttu-id="9fb6c-140">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="9fb6c-140">Operating System version</span></span>|
|<span data-ttu-id="9fb6c-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="9fb6c-141">deviceType</span></span>|<span data-ttu-id="9fb6c-142">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-142">String</span></span>|<span data-ttu-id="9fb6c-143">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="9fb6c-143">Host device type</span></span>|
|<span data-ttu-id="9fb6c-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="9fb6c-144">deviceTag</span></span>|<span data-ttu-id="9fb6c-145">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-145">String</span></span>|<span data-ttu-id="9fb6c-146">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="9fb6c-147">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="9fb6c-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="9fb6c-148">deviceName</span></span>|<span data-ttu-id="9fb6c-149">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-149">String</span></span>|<span data-ttu-id="9fb6c-150">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="9fb6c-150">Host device name</span></span>|
|<span data-ttu-id="9fb6c-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="9fb6c-151">flaggedReasons</span></span>|<span data-ttu-id="9fb6c-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fb6c-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="9fb6c-153">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="9fb6c-154">例如，</span><span class="sxs-lookup"><span data-stu-id="9fb6c-154">E.g.</span></span> <span data-ttu-id="9fb6c-155">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="9fb6c-155">app running on rooted device</span></span>|
|<span data-ttu-id="9fb6c-156">userId</span><span class="sxs-lookup"><span data-stu-id="9fb6c-156">userId</span></span>|<span data-ttu-id="9fb6c-157">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-157">String</span></span>|<span data-ttu-id="9fb6c-158">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-158">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="9fb6c-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fb6c-159">appIdentifier</span></span>|[<span data-ttu-id="9fb6c-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fb6c-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9fb6c-161">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="9fb6c-161">The app package Identifier</span></span>|
|<span data-ttu-id="9fb6c-162">id</span><span class="sxs-lookup"><span data-stu-id="9fb6c-162">id</span></span>|<span data-ttu-id="9fb6c-163">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-163">String</span></span>|<span data-ttu-id="9fb6c-164">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-164">Key of the entity.</span></span>|
|<span data-ttu-id="9fb6c-165">version</span><span class="sxs-lookup"><span data-stu-id="9fb6c-165">version</span></span>|<span data-ttu-id="9fb6c-166">String</span><span class="sxs-lookup"><span data-stu-id="9fb6c-166">String</span></span>|<span data-ttu-id="9fb6c-167">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-167">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fb6c-168">关系</span><span class="sxs-lookup"><span data-stu-id="9fb6c-168">Relationships</span></span>
|<span data-ttu-id="9fb6c-169">关系</span><span class="sxs-lookup"><span data-stu-id="9fb6c-169">Relationship</span></span>|<span data-ttu-id="9fb6c-170">类型</span><span class="sxs-lookup"><span data-stu-id="9fb6c-170">Type</span></span>|<span data-ttu-id="9fb6c-171">说明</span><span class="sxs-lookup"><span data-stu-id="9fb6c-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fb6c-172">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="9fb6c-172">appliedPolicies</span></span>|<span data-ttu-id="9fb6c-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fb6c-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9fb6c-174">注册应用上次与管理服务同步时，已应用零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-174">Zero or more policys already applied on the registered app when it last synchronized with management service.</span></span>|
|<span data-ttu-id="9fb6c-175">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="9fb6c-175">intendedPolicies</span></span>|<span data-ttu-id="9fb6c-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fb6c-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9fb6c-177">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-177">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="9fb6c-178">操作</span><span class="sxs-lookup"><span data-stu-id="9fb6c-178">operations</span></span>|<span data-ttu-id="9fb6c-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fb6c-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="9fb6c-180">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-180">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fb6c-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fb6c-181">JSON Representation</span></span>
<span data-ttu-id="9fb6c-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fb6c-182">Here is a JSON representation of the resource.</span></span>
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
  ],
}
-->








