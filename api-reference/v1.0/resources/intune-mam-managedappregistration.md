---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。
ms.openlocfilehash: efccea80c953ee4eac07588a21944d10810f8532
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008374"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="31aa3-103">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="31aa3-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="31aa3-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="31aa3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31aa3-105">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="31aa3-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="31aa3-106">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="31aa3-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="31aa3-107">方法</span><span class="sxs-lookup"><span data-stu-id="31aa3-107">Methods</span></span>
|<span data-ttu-id="31aa3-108">方法</span><span class="sxs-lookup"><span data-stu-id="31aa3-108">Method</span></span>|<span data-ttu-id="31aa3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="31aa3-109">Return Type</span></span>|<span data-ttu-id="31aa3-110">说明</span><span class="sxs-lookup"><span data-stu-id="31aa3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31aa3-111">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="31aa3-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="31aa3-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31aa3-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="31aa3-113">列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31aa3-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="31aa3-114">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31aa3-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="31aa3-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31aa3-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="31aa3-116">读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31aa3-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="31aa3-117">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="31aa3-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="31aa3-118">String collection</span><span class="sxs-lookup"><span data-stu-id="31aa3-118">String collection</span></span>|<span data-ttu-id="31aa3-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31aa3-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="31aa3-120">属性</span><span class="sxs-lookup"><span data-stu-id="31aa3-120">Properties</span></span>
|<span data-ttu-id="31aa3-121">属性</span><span class="sxs-lookup"><span data-stu-id="31aa3-121">Property</span></span>|<span data-ttu-id="31aa3-122">类型</span><span class="sxs-lookup"><span data-stu-id="31aa3-122">Type</span></span>|<span data-ttu-id="31aa3-123">说明</span><span class="sxs-lookup"><span data-stu-id="31aa3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31aa3-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31aa3-124">createdDateTime</span></span>|<span data-ttu-id="31aa3-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31aa3-125">DateTimeOffset</span></span>|<span data-ttu-id="31aa3-126">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="31aa3-126">Date and time of creation</span></span>|
|<span data-ttu-id="31aa3-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="31aa3-127">lastSyncDateTime</span></span>|<span data-ttu-id="31aa3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31aa3-128">DateTimeOffset</span></span>|<span data-ttu-id="31aa3-129">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="31aa3-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="31aa3-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="31aa3-130">applicationVersion</span></span>|<span data-ttu-id="31aa3-131">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-131">String</span></span>|<span data-ttu-id="31aa3-132">应用版本</span><span class="sxs-lookup"><span data-stu-id="31aa3-132">App version</span></span>|
|<span data-ttu-id="31aa3-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="31aa3-133">managementSdkVersion</span></span>|<span data-ttu-id="31aa3-134">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-134">String</span></span>|<span data-ttu-id="31aa3-135">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="31aa3-135">App management SDK version</span></span>|
|<span data-ttu-id="31aa3-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="31aa3-136">platformVersion</span></span>|<span data-ttu-id="31aa3-137">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-137">String</span></span>|<span data-ttu-id="31aa3-138">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="31aa3-138">Operating System version</span></span>|
|<span data-ttu-id="31aa3-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="31aa3-139">deviceType</span></span>|<span data-ttu-id="31aa3-140">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-140">String</span></span>|<span data-ttu-id="31aa3-141">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="31aa3-141">Host device type</span></span>|
|<span data-ttu-id="31aa3-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="31aa3-142">deviceTag</span></span>|<span data-ttu-id="31aa3-143">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-143">String</span></span>|<span data-ttu-id="31aa3-144">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="31aa3-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="31aa3-145">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="31aa3-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="31aa3-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="31aa3-146">deviceName</span></span>|<span data-ttu-id="31aa3-147">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-147">String</span></span>|<span data-ttu-id="31aa3-148">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="31aa3-148">Host device name</span></span>|
|<span data-ttu-id="31aa3-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="31aa3-149">flaggedReasons</span></span>|<span data-ttu-id="31aa3-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="31aa3-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="31aa3-151">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="31aa3-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="31aa3-152">例如，</span><span class="sxs-lookup"><span data-stu-id="31aa3-152">E.g.</span></span> <span data-ttu-id="31aa3-153">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="31aa3-153">app running on rooted device</span></span>|
|<span data-ttu-id="31aa3-154">userId</span><span class="sxs-lookup"><span data-stu-id="31aa3-154">userId</span></span>|<span data-ttu-id="31aa3-155">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-155">String</span></span>|<span data-ttu-id="31aa3-156">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="31aa3-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="31aa3-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="31aa3-157">appIdentifier</span></span>|[<span data-ttu-id="31aa3-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="31aa3-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="31aa3-159">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="31aa3-159">The app package Identifier</span></span>|
|<span data-ttu-id="31aa3-160">id</span><span class="sxs-lookup"><span data-stu-id="31aa3-160">id</span></span>|<span data-ttu-id="31aa3-161">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-161">String</span></span>|<span data-ttu-id="31aa3-162">实体的键。</span><span class="sxs-lookup"><span data-stu-id="31aa3-162">Key of the entity.</span></span>|
|<span data-ttu-id="31aa3-163">version</span><span class="sxs-lookup"><span data-stu-id="31aa3-163">version</span></span>|<span data-ttu-id="31aa3-164">String</span><span class="sxs-lookup"><span data-stu-id="31aa3-164">String</span></span>|<span data-ttu-id="31aa3-165">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="31aa3-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31aa3-166">关系</span><span class="sxs-lookup"><span data-stu-id="31aa3-166">Relationships</span></span>
|<span data-ttu-id="31aa3-167">关系</span><span class="sxs-lookup"><span data-stu-id="31aa3-167">Relationship</span></span>|<span data-ttu-id="31aa3-168">类型</span><span class="sxs-lookup"><span data-stu-id="31aa3-168">Type</span></span>|<span data-ttu-id="31aa3-169">说明</span><span class="sxs-lookup"><span data-stu-id="31aa3-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31aa3-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="31aa3-170">appliedPolicies</span></span>|<span data-ttu-id="31aa3-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31aa3-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="31aa3-172">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="31aa3-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="31aa3-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="31aa3-173">intendedPolicies</span></span>|<span data-ttu-id="31aa3-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31aa3-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="31aa3-175">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="31aa3-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="31aa3-176">操作</span><span class="sxs-lookup"><span data-stu-id="31aa3-176">operations</span></span>|<span data-ttu-id="31aa3-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31aa3-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="31aa3-178">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="31aa3-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31aa3-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31aa3-179">JSON Representation</span></span>
<span data-ttu-id="31aa3-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31aa3-180">Here is a JSON representation of the resource.</span></span>
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
