# <a name="user-resource-type"></a><span data-ttu-id="a50c1-101">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="a50c1-101">user resource type</span></span>

> <span data-ttu-id="a50c1-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a50c1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a50c1-103">表示 Azure Active Directory 用户对象。</span><span class="sxs-lookup"><span data-stu-id="a50c1-103">Represents an Azure Active Directory user object.</span></span>
## <a name="methods"></a><span data-ttu-id="a50c1-104">方法</span><span class="sxs-lookup"><span data-stu-id="a50c1-104">Methods</span></span>
|<span data-ttu-id="a50c1-105">方法</span><span class="sxs-lookup"><span data-stu-id="a50c1-105">Method</span></span>|<span data-ttu-id="a50c1-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="a50c1-106">Return Type</span></span>|<span data-ttu-id="a50c1-107">说明</span><span class="sxs-lookup"><span data-stu-id="a50c1-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a50c1-108">List users</span><span class="sxs-lookup"><span data-stu-id="a50c1-108">List users</span></span>](../api/intune_mam_user_list.md)|<span data-ttu-id="a50c1-109">[user](../resources/intune_mam_user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a50c1-109">[user](../resources/intune_mam_user.md) collection</span></span>|<span data-ttu-id="a50c1-110">列出 [user](../resources/intune_mam_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a50c1-110">List properties and relationships of the [user](../resources/intune_mam_user.md) objects.</span></span>|
|[<span data-ttu-id="a50c1-111">获取 user</span><span class="sxs-lookup"><span data-stu-id="a50c1-111">Get user</span></span>](../api/intune_mam_user_get.md)|[<span data-ttu-id="a50c1-112">user</span><span class="sxs-lookup"><span data-stu-id="a50c1-112">user</span></span>](../resources/intune_mam_user.md)|<span data-ttu-id="a50c1-113">读取 [user](../resources/intune_mam_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a50c1-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_user.md) object.</span></span>|
|[<span data-ttu-id="a50c1-114">创建 user</span><span class="sxs-lookup"><span data-stu-id="a50c1-114">Create user</span></span>](../api/intune_mam_user_create.md)|[<span data-ttu-id="a50c1-115">user</span><span class="sxs-lookup"><span data-stu-id="a50c1-115">user</span></span>](../resources/intune_mam_user.md)|<span data-ttu-id="a50c1-116">创建新的 [user](../resources/intune_mam_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a50c1-116">Create a new user object.</span></span>|
|[<span data-ttu-id="a50c1-117">删除 user</span><span class="sxs-lookup"><span data-stu-id="a50c1-117">Delete user</span></span>](../api/intune_mam_user_delete.md)|<span data-ttu-id="a50c1-118">无</span><span class="sxs-lookup"><span data-stu-id="a50c1-118">None</span></span>|<span data-ttu-id="a50c1-119">删除 [user](../resources/intune_mam_user.md)。</span><span class="sxs-lookup"><span data-stu-id="a50c1-119">Deletes a [user](../resources/intune_mam_user.md).</span></span>|
|[<span data-ttu-id="a50c1-120">更新 user</span><span class="sxs-lookup"><span data-stu-id="a50c1-120">Update user</span></span>](../api/intune_mam_user_update.md)|[<span data-ttu-id="a50c1-121">user</span><span class="sxs-lookup"><span data-stu-id="a50c1-121">user</span></span>](../resources/intune_mam_user.md)|<span data-ttu-id="a50c1-122">更新 [user](../resources/intune_mam_user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a50c1-122">Update the properties of a user object.</span></span>|
|[<span data-ttu-id="a50c1-123">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="a50c1-123">getManagedAppDiagnosticStatuses function</span></span>](../api/intune_mam_user_getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="a50c1-124">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a50c1-124">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="a50c1-125">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="a50c1-125">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="a50c1-126">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="a50c1-126">getManagedAppPolicies function</span></span>](../api/intune_mam_user_getmanagedapppolicies.md)|<span data-ttu-id="a50c1-127">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a50c1-127">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="a50c1-128">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="a50c1-128">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="a50c1-129">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="a50c1-129">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="a50c1-130">无</span><span class="sxs-lookup"><span data-stu-id="a50c1-130">None</span></span>|<span data-ttu-id="a50c1-131">对含有指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="a50c1-131">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="a50c1-132">属性</span><span class="sxs-lookup"><span data-stu-id="a50c1-132">Properties</span></span>
|<span data-ttu-id="a50c1-133">属性</span><span class="sxs-lookup"><span data-stu-id="a50c1-133">Property</span></span>|<span data-ttu-id="a50c1-134">类型</span><span class="sxs-lookup"><span data-stu-id="a50c1-134">Type</span></span>|<span data-ttu-id="a50c1-135">说明</span><span class="sxs-lookup"><span data-stu-id="a50c1-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a50c1-136">id</span><span class="sxs-lookup"><span data-stu-id="a50c1-136">id</span></span>|<span data-ttu-id="a50c1-137">String</span><span class="sxs-lookup"><span data-stu-id="a50c1-137">String</span></span>|<span data-ttu-id="a50c1-138">用户标识符。</span><span class="sxs-lookup"><span data-stu-id="a50c1-138">The user identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a50c1-139">关系</span><span class="sxs-lookup"><span data-stu-id="a50c1-139">Relationships</span></span>
|<span data-ttu-id="a50c1-140">关系</span><span class="sxs-lookup"><span data-stu-id="a50c1-140">Relationship</span></span>|<span data-ttu-id="a50c1-141">类型</span><span class="sxs-lookup"><span data-stu-id="a50c1-141">Type</span></span>|<span data-ttu-id="a50c1-142">说明</span><span class="sxs-lookup"><span data-stu-id="a50c1-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a50c1-143">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="a50c1-143">managedAppRegistrations</span></span>|<span data-ttu-id="a50c1-144">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a50c1-144">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="a50c1-145">属于用户的零个或多个托管的应用注册。</span><span class="sxs-lookup"><span data-stu-id="a50c1-145">Zero or more managed app registrations that belong to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a50c1-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a50c1-146">JSON Representation</span></span>
<span data-ttu-id="a50c1-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a50c1-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



