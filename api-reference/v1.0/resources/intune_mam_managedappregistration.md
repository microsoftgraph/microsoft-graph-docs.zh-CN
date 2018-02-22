# <a name="managedappregistration-resource-type"></a><span data-ttu-id="fadef-101">managedAppRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="fadef-101">managedAppRegistration resource type</span></span>

> <span data-ttu-id="fadef-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fadef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fadef-103">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="fadef-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="fadef-104">ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fadef-104">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="fadef-105">方法</span><span class="sxs-lookup"><span data-stu-id="fadef-105">Methods</span></span>
|<span data-ttu-id="fadef-106">方法</span><span class="sxs-lookup"><span data-stu-id="fadef-106">Method</span></span>|<span data-ttu-id="fadef-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="fadef-107">Return Type</span></span>|<span data-ttu-id="fadef-108">说明</span><span class="sxs-lookup"><span data-stu-id="fadef-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fadef-109">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="fadef-109">List managedAppRegistrations</span></span>](../api/intune_mam_managedappregistration_list.md)|<span data-ttu-id="fadef-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fadef-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="fadef-111">列出 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fadef-111">List properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="fadef-112">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="fadef-112">Get managedAppRegistration</span></span>](../api/intune_mam_managedappregistration_get.md)|[<span data-ttu-id="fadef-113">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="fadef-113">managedAppRegistration</span></span>](../resources/intune_mam_managedappregistration.md)|<span data-ttu-id="fadef-114">读取 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fadef-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="fadef-115">getUserIdsWithFlaggedAppRegistration 函数</span><span class="sxs-lookup"><span data-stu-id="fadef-115">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|<span data-ttu-id="fadef-116">String collection</span><span class="sxs-lookup"><span data-stu-id="fadef-116">String collection</span></span>|<span data-ttu-id="fadef-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fadef-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fadef-118">属性</span><span class="sxs-lookup"><span data-stu-id="fadef-118">Properties</span></span>
|<span data-ttu-id="fadef-119">属性</span><span class="sxs-lookup"><span data-stu-id="fadef-119">Property</span></span>|<span data-ttu-id="fadef-120">类型</span><span class="sxs-lookup"><span data-stu-id="fadef-120">Type</span></span>|<span data-ttu-id="fadef-121">说明</span><span class="sxs-lookup"><span data-stu-id="fadef-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fadef-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fadef-122">createdDateTime</span></span>|<span data-ttu-id="fadef-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fadef-123">DateTimeOffset</span></span>|<span data-ttu-id="fadef-124">创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="fadef-124">Date and time of cube creation.</span></span>|
|<span data-ttu-id="fadef-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fadef-125">lastSyncDateTime</span></span>|<span data-ttu-id="fadef-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fadef-126">DateTimeOffset</span></span>|<span data-ttu-id="fadef-127">上次应用与管理服务同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fadef-127">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="fadef-128">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="fadef-128">applicationVersion</span></span>|<span data-ttu-id="fadef-129">String</span><span class="sxs-lookup"><span data-stu-id="fadef-129">String</span></span>|<span data-ttu-id="fadef-130">应用版本</span><span class="sxs-lookup"><span data-stu-id="fadef-130">App version</span></span>|
|<span data-ttu-id="fadef-131">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="fadef-131">managementSdkVersion</span></span>|<span data-ttu-id="fadef-132">String</span><span class="sxs-lookup"><span data-stu-id="fadef-132">String</span></span>|<span data-ttu-id="fadef-133">应用管理 SDK 版本</span><span class="sxs-lookup"><span data-stu-id="fadef-133">App management SDK version</span></span>|
|<span data-ttu-id="fadef-134">platformVersion</span><span class="sxs-lookup"><span data-stu-id="fadef-134">platformVersion</span></span>|<span data-ttu-id="fadef-135">String</span><span class="sxs-lookup"><span data-stu-id="fadef-135">String</span></span>|<span data-ttu-id="fadef-136">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="fadef-136">Operating System version</span></span>|
|<span data-ttu-id="fadef-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="fadef-137">deviceType</span></span>|<span data-ttu-id="fadef-138">String</span><span class="sxs-lookup"><span data-stu-id="fadef-138">String</span></span>|<span data-ttu-id="fadef-139">主机设备类型</span><span class="sxs-lookup"><span data-stu-id="fadef-139">Host device type</span></span>|
|<span data-ttu-id="fadef-140">deviceTag</span><span class="sxs-lookup"><span data-stu-id="fadef-140">deviceTag</span></span>|<span data-ttu-id="fadef-141">String</span><span class="sxs-lookup"><span data-stu-id="fadef-141">String</span></span>|<span data-ttu-id="fadef-142">应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。</span><span class="sxs-lookup"><span data-stu-id="fadef-142">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="fadef-143">不保证在所有情况下与应用关联。</span><span class="sxs-lookup"><span data-stu-id="fadef-143">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="fadef-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="fadef-144">deviceName</span></span>|<span data-ttu-id="fadef-145">String</span><span class="sxs-lookup"><span data-stu-id="fadef-145">String</span></span>|<span data-ttu-id="fadef-146">主机设备名称</span><span class="sxs-lookup"><span data-stu-id="fadef-146">Host device name</span></span>|
|<span data-ttu-id="fadef-147">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="fadef-147">flaggedReasons</span></span>|<span data-ttu-id="fadef-148">String collection</span><span class="sxs-lookup"><span data-stu-id="fadef-148">String collection</span></span>|<span data-ttu-id="fadef-149">标记应用注册的零个或多个原因。</span><span class="sxs-lookup"><span data-stu-id="fadef-149">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="fadef-150">例如，</span><span class="sxs-lookup"><span data-stu-id="fadef-150">E.g.</span></span> <span data-ttu-id="fadef-151">在取得 root 权限的设备上运行的应用</span><span class="sxs-lookup"><span data-stu-id="fadef-151">app running on rooted device</span></span>|
|<span data-ttu-id="fadef-152">userId</span><span class="sxs-lookup"><span data-stu-id="fadef-152">userID</span></span>|<span data-ttu-id="fadef-153">String</span><span class="sxs-lookup"><span data-stu-id="fadef-153">String</span></span>|<span data-ttu-id="fadef-154">此应用注册所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="fadef-154">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="fadef-155">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="fadef-155">appIdentifier</span></span>|[<span data-ttu-id="fadef-156">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fadef-156">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="fadef-157">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="fadef-157">The app package Identifier</span></span>|
|<span data-ttu-id="fadef-158">id</span><span class="sxs-lookup"><span data-stu-id="fadef-158">id</span></span>|<span data-ttu-id="fadef-159">String</span><span class="sxs-lookup"><span data-stu-id="fadef-159">String</span></span>|<span data-ttu-id="fadef-160">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fadef-160">Key of the setting.</span></span>|
|<span data-ttu-id="fadef-161">版本</span><span class="sxs-lookup"><span data-stu-id="fadef-161">version</span></span>|<span data-ttu-id="fadef-162">String</span><span class="sxs-lookup"><span data-stu-id="fadef-162">String</span></span>|<span data-ttu-id="fadef-163">实体版本。</span><span class="sxs-lookup"><span data-stu-id="fadef-163">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fadef-164">关系</span><span class="sxs-lookup"><span data-stu-id="fadef-164">Relationships</span></span>
|<span data-ttu-id="fadef-165">关系</span><span class="sxs-lookup"><span data-stu-id="fadef-165">Relationship</span></span>|<span data-ttu-id="fadef-166">类型</span><span class="sxs-lookup"><span data-stu-id="fadef-166">Type</span></span>|<span data-ttu-id="fadef-167">说明</span><span class="sxs-lookup"><span data-stu-id="fadef-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fadef-168">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="fadef-168">appliedPolicies</span></span>|<span data-ttu-id="fadef-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fadef-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="fadef-170">当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="fadef-170">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="fadef-171">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="fadef-171">intendedPolicies</span></span>|<span data-ttu-id="fadef-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fadef-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="fadef-173">目前适用于应用的零个或多个策略管理员。</span><span class="sxs-lookup"><span data-stu-id="fadef-173">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="fadef-174">操作</span><span class="sxs-lookup"><span data-stu-id="fadef-174">operations</span></span>|<span data-ttu-id="fadef-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fadef-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="fadef-176">在应用注册时触发的零个或多个长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="fadef-176">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fadef-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fadef-177">JSON Representation</span></span>
<span data-ttu-id="fadef-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fadef-178">Here is a JSON representation of the resource.</span></span>
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



