---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8eff848b54d3a84f6fb60d2c8335d71417f2afb0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755754"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="d2d35-104">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2d35-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="d2d35-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2d35-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2d35-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2d35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d35-107">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="d2d35-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="d2d35-108">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2d35-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="d2d35-109">Methods</span><span class="sxs-lookup"><span data-stu-id="d2d35-109">Methods</span></span>
|<span data-ttu-id="d2d35-110">方法</span><span class="sxs-lookup"><span data-stu-id="d2d35-110">Method</span></span>|<span data-ttu-id="d2d35-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2d35-111">Return Type</span></span>|<span data-ttu-id="d2d35-112">Description</span><span class="sxs-lookup"><span data-stu-id="d2d35-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2d35-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d2d35-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="d2d35-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2d35-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="d2d35-115">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2d35-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="d2d35-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d2d35-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="d2d35-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d2d35-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="d2d35-118">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2d35-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="d2d35-119">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="d2d35-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="d2d35-120">String collection</span><span class="sxs-lookup"><span data-stu-id="d2d35-120">String collection</span></span>|<span data-ttu-id="d2d35-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2d35-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d2d35-122">属性</span><span class="sxs-lookup"><span data-stu-id="d2d35-122">Properties</span></span>
|<span data-ttu-id="d2d35-123">属性</span><span class="sxs-lookup"><span data-stu-id="d2d35-123">Property</span></span>|<span data-ttu-id="d2d35-124">类型</span><span class="sxs-lookup"><span data-stu-id="d2d35-124">Type</span></span>|<span data-ttu-id="d2d35-125">说明</span><span class="sxs-lookup"><span data-stu-id="d2d35-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d35-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d35-126">createdDateTime</span></span>|<span data-ttu-id="d2d35-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d35-127">DateTimeOffset</span></span>|<span data-ttu-id="d2d35-128">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="d2d35-128">Date and time of creation</span></span>|
|<span data-ttu-id="d2d35-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d35-129">lastSyncDateTime</span></span>|<span data-ttu-id="d2d35-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d35-130">DateTimeOffset</span></span>|<span data-ttu-id="d2d35-131">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d2d35-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="d2d35-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d2d35-132">applicationVersion</span></span>|<span data-ttu-id="d2d35-133">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-133">String</span></span>|<span data-ttu-id="d2d35-134">应用版本</span><span class="sxs-lookup"><span data-stu-id="d2d35-134">App version</span></span>|
|<span data-ttu-id="d2d35-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d2d35-135">managementSdkVersion</span></span>|<span data-ttu-id="d2d35-136">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-136">String</span></span>|<span data-ttu-id="d2d35-137">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="d2d35-137">App management SDK version</span></span>|
|<span data-ttu-id="d2d35-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d2d35-138">platformVersion</span></span>|<span data-ttu-id="d2d35-139">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-139">String</span></span>|<span data-ttu-id="d2d35-140">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="d2d35-140">Operating System version</span></span>|
|<span data-ttu-id="d2d35-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="d2d35-141">deviceType</span></span>|<span data-ttu-id="d2d35-142">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-142">String</span></span>|<span data-ttu-id="d2d35-143">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="d2d35-143">Host device type</span></span>|
|<span data-ttu-id="d2d35-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d2d35-144">deviceTag</span></span>|<span data-ttu-id="d2d35-145">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-145">String</span></span>|<span data-ttu-id="d2d35-146">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="d2d35-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d2d35-147">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="d2d35-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="d2d35-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="d2d35-148">deviceName</span></span>|<span data-ttu-id="d2d35-149">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-149">String</span></span>|<span data-ttu-id="d2d35-150">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="d2d35-150">Host device name</span></span>|
|<span data-ttu-id="d2d35-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d2d35-151">flaggedReasons</span></span>|<span data-ttu-id="d2d35-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2d35-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d2d35-153">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="d2d35-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d2d35-154">例如，</span><span class="sxs-lookup"><span data-stu-id="d2d35-154">E.g.</span></span> <span data-ttu-id="d2d35-155">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="d2d35-155">app running on rooted device</span></span>|
|<span data-ttu-id="d2d35-156">userId</span><span class="sxs-lookup"><span data-stu-id="d2d35-156">userId</span></span>|<span data-ttu-id="d2d35-157">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-157">String</span></span>|<span data-ttu-id="d2d35-158">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d2d35-158">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="d2d35-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d2d35-159">appIdentifier</span></span>|[<span data-ttu-id="d2d35-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d2d35-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d2d35-161">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="d2d35-161">The app package Identifier</span></span>|
|<span data-ttu-id="d2d35-162">id</span><span class="sxs-lookup"><span data-stu-id="d2d35-162">id</span></span>|<span data-ttu-id="d2d35-163">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-163">String</span></span>|<span data-ttu-id="d2d35-164">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2d35-164">Key of the entity.</span></span>|
|<span data-ttu-id="d2d35-165">version</span><span class="sxs-lookup"><span data-stu-id="d2d35-165">version</span></span>|<span data-ttu-id="d2d35-166">String</span><span class="sxs-lookup"><span data-stu-id="d2d35-166">String</span></span>|<span data-ttu-id="d2d35-167">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d2d35-167">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2d35-168">关系</span><span class="sxs-lookup"><span data-stu-id="d2d35-168">Relationships</span></span>
|<span data-ttu-id="d2d35-169">关系</span><span class="sxs-lookup"><span data-stu-id="d2d35-169">Relationship</span></span>|<span data-ttu-id="d2d35-170">类型</span><span class="sxs-lookup"><span data-stu-id="d2d35-170">Type</span></span>|<span data-ttu-id="d2d35-171">Description</span><span class="sxs-lookup"><span data-stu-id="d2d35-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d35-172">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="d2d35-172">appliedPolicies</span></span>|<span data-ttu-id="d2d35-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2d35-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d2d35-174">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="d2d35-174">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="d2d35-175">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="d2d35-175">intendedPolicies</span></span>|<span data-ttu-id="d2d35-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2d35-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d2d35-177">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="d2d35-177">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="d2d35-178">操作</span><span class="sxs-lookup"><span data-stu-id="d2d35-178">operations</span></span>|<span data-ttu-id="d2d35-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2d35-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d2d35-180">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="d2d35-180">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2d35-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2d35-181">JSON Representation</span></span>
<span data-ttu-id="d2d35-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2d35-182">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




