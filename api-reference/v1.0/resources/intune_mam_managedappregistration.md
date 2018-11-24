# <a name="managedappregistration-resource-type"></a><span data-ttu-id="43b68-101">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="43b68-101">managedAppRegistration resource type</span></span>

> <span data-ttu-id="43b68-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="43b68-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43b68-103">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="43b68-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="43b68-104">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="43b68-104">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="43b68-105">方法</span><span class="sxs-lookup"><span data-stu-id="43b68-105">Methods</span></span>
|<span data-ttu-id="43b68-106">方法</span><span class="sxs-lookup"><span data-stu-id="43b68-106">Method</span></span>|<span data-ttu-id="43b68-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="43b68-107">Return Type</span></span>|<span data-ttu-id="43b68-108">说明</span><span class="sxs-lookup"><span data-stu-id="43b68-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43b68-109">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="43b68-109">List managedAppRegistrations</span></span>](../api/intune_mam_managedappregistration_list.md)|<span data-ttu-id="43b68-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43b68-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="43b68-111">列出 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43b68-111">List properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="43b68-112">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="43b68-112">Get managedAppRegistration</span></span>](../api/intune_mam_managedappregistration_get.md)|[<span data-ttu-id="43b68-113">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="43b68-113">managedAppRegistration</span></span>](../resources/intune_mam_managedappregistration.md)|<span data-ttu-id="43b68-114">读取 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43b68-114">Read properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="43b68-115">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="43b68-115">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|<span data-ttu-id="43b68-116">String collection</span><span class="sxs-lookup"><span data-stu-id="43b68-116">String collection</span></span>|<span data-ttu-id="43b68-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="43b68-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="43b68-118">属性</span><span class="sxs-lookup"><span data-stu-id="43b68-118">Properties</span></span>
|<span data-ttu-id="43b68-119">属性</span><span class="sxs-lookup"><span data-stu-id="43b68-119">Property</span></span>|<span data-ttu-id="43b68-120">类型</span><span class="sxs-lookup"><span data-stu-id="43b68-120">Type</span></span>|<span data-ttu-id="43b68-121">说明</span><span class="sxs-lookup"><span data-stu-id="43b68-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b68-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43b68-122">createdDateTime</span></span>|<span data-ttu-id="43b68-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43b68-123">DateTimeOffset</span></span>|<span data-ttu-id="43b68-124">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="43b68-124">Date and time of creation</span></span>|
|<span data-ttu-id="43b68-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="43b68-125">lastSyncDateTime</span></span>|<span data-ttu-id="43b68-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43b68-126">DateTimeOffset</span></span>|<span data-ttu-id="43b68-127">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="43b68-127">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="43b68-128">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="43b68-128">applicationVersion</span></span>|<span data-ttu-id="43b68-129">String</span><span class="sxs-lookup"><span data-stu-id="43b68-129">String</span></span>|<span data-ttu-id="43b68-130">应用版本</span><span class="sxs-lookup"><span data-stu-id="43b68-130">App version</span></span>|
|<span data-ttu-id="43b68-131">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="43b68-131">managementSdkVersion</span></span>|<span data-ttu-id="43b68-132">String</span><span class="sxs-lookup"><span data-stu-id="43b68-132">String</span></span>|<span data-ttu-id="43b68-133">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="43b68-133">App management SDK version</span></span>|
|<span data-ttu-id="43b68-134">platformVersion</span><span class="sxs-lookup"><span data-stu-id="43b68-134">platformVersion</span></span>|<span data-ttu-id="43b68-135">String</span><span class="sxs-lookup"><span data-stu-id="43b68-135">String</span></span>|<span data-ttu-id="43b68-136">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="43b68-136">Operating System version</span></span>|
|<span data-ttu-id="43b68-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="43b68-137">deviceType</span></span>|<span data-ttu-id="43b68-138">String</span><span class="sxs-lookup"><span data-stu-id="43b68-138">String</span></span>|<span data-ttu-id="43b68-139">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="43b68-139">Host device type</span></span>|
|<span data-ttu-id="43b68-140">deviceTag</span><span class="sxs-lookup"><span data-stu-id="43b68-140">deviceTag</span></span>|<span data-ttu-id="43b68-141">String</span><span class="sxs-lookup"><span data-stu-id="43b68-141">String</span></span>|<span data-ttu-id="43b68-142">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="43b68-142">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="43b68-143">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="43b68-143">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="43b68-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="43b68-144">deviceName</span></span>|<span data-ttu-id="43b68-145">String</span><span class="sxs-lookup"><span data-stu-id="43b68-145">String</span></span>|<span data-ttu-id="43b68-146">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="43b68-146">Host device name</span></span>|
|<span data-ttu-id="43b68-147">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="43b68-147">flaggedReasons</span></span>|<span data-ttu-id="43b68-148">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="43b68-148">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="43b68-149">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="43b68-149">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="43b68-150">例如，</span><span class="sxs-lookup"><span data-stu-id="43b68-150">E.g.</span></span> <span data-ttu-id="43b68-151">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="43b68-151">app running on rooted device</span></span>|
|<span data-ttu-id="43b68-152">userId</span><span class="sxs-lookup"><span data-stu-id="43b68-152">userId</span></span>|<span data-ttu-id="43b68-153">String</span><span class="sxs-lookup"><span data-stu-id="43b68-153">String</span></span>|<span data-ttu-id="43b68-154">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="43b68-154">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="43b68-155">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="43b68-155">appIdentifier</span></span>|[<span data-ttu-id="43b68-156">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="43b68-156">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="43b68-157">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="43b68-157">The app package Identifier</span></span>|
|<span data-ttu-id="43b68-158">id</span><span class="sxs-lookup"><span data-stu-id="43b68-158">id</span></span>|<span data-ttu-id="43b68-159">String</span><span class="sxs-lookup"><span data-stu-id="43b68-159">String</span></span>|<span data-ttu-id="43b68-160">实体的键。</span><span class="sxs-lookup"><span data-stu-id="43b68-160">Key of the entity.</span></span>|
|<span data-ttu-id="43b68-161">版本</span><span class="sxs-lookup"><span data-stu-id="43b68-161">version</span></span>|<span data-ttu-id="43b68-162">String</span><span class="sxs-lookup"><span data-stu-id="43b68-162">String</span></span>|<span data-ttu-id="43b68-163">实体版本。</span><span class="sxs-lookup"><span data-stu-id="43b68-163">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43b68-164">关系</span><span class="sxs-lookup"><span data-stu-id="43b68-164">Relationships</span></span>
|<span data-ttu-id="43b68-165">关系</span><span class="sxs-lookup"><span data-stu-id="43b68-165">Relationship</span></span>|<span data-ttu-id="43b68-166">类型</span><span class="sxs-lookup"><span data-stu-id="43b68-166">Type</span></span>|<span data-ttu-id="43b68-167">说明</span><span class="sxs-lookup"><span data-stu-id="43b68-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b68-168">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="43b68-168">appliedPolicies</span></span>|<span data-ttu-id="43b68-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43b68-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="43b68-170">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="43b68-170">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="43b68-171">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="43b68-171">intendedPolicies</span></span>|<span data-ttu-id="43b68-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43b68-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="43b68-173">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="43b68-173">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="43b68-174">操作</span><span class="sxs-lookup"><span data-stu-id="43b68-174">operations</span></span>|<span data-ttu-id="43b68-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43b68-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="43b68-176">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="43b68-176">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43b68-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43b68-177">JSON Representation</span></span>
<span data-ttu-id="43b68-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43b68-178">Here is a JSON representation of the resource.</span></span>
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
     "Warning: /api-reference/v1.0/resources/intune_mam_managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
