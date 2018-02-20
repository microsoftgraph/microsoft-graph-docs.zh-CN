# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="dc998-101">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc998-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="dc998-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dc998-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc998-103">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="dc998-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="dc998-104">方法</span><span class="sxs-lookup"><span data-stu-id="dc998-104">Methods</span></span>
|<span data-ttu-id="dc998-105">方法</span><span class="sxs-lookup"><span data-stu-id="dc998-105">Method</span></span>|<span data-ttu-id="dc998-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc998-106">Return Type</span></span>|<span data-ttu-id="dc998-107">说明</span><span class="sxs-lookup"><span data-stu-id="dc998-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc998-108">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="dc998-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="dc998-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc998-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="dc998-110">列出 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc998-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="dc998-111">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dc998-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="dc998-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dc998-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="dc998-113">读取 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc998-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="dc998-114">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="dc998-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="dc998-115">无</span><span class="sxs-lookup"><span data-stu-id="dc998-115">None</span></span>|<span data-ttu-id="dc998-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dc998-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="dc998-117">属性</span><span class="sxs-lookup"><span data-stu-id="dc998-117">Properties</span></span>
|<span data-ttu-id="dc998-118">属性</span><span class="sxs-lookup"><span data-stu-id="dc998-118">Property</span></span>|<span data-ttu-id="dc998-119">类型</span><span class="sxs-lookup"><span data-stu-id="dc998-119">Type</span></span>|<span data-ttu-id="dc998-120">说明</span><span class="sxs-lookup"><span data-stu-id="dc998-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc998-121">displayName</span><span class="sxs-lookup"><span data-stu-id="dc998-121">displayName</span></span>|<span data-ttu-id="dc998-122">String</span><span class="sxs-lookup"><span data-stu-id="dc998-122">String</span></span>|<span data-ttu-id="dc998-123">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="dc998-123">Policy display name.</span></span>|
|<span data-ttu-id="dc998-124">description</span><span class="sxs-lookup"><span data-stu-id="dc998-124">description</span></span>|<span data-ttu-id="dc998-125">String</span><span class="sxs-lookup"><span data-stu-id="dc998-125">String</span></span>|<span data-ttu-id="dc998-126">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="dc998-126">The policy's description.</span></span>|
|<span data-ttu-id="dc998-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc998-127">createdDateTime</span></span>|<span data-ttu-id="dc998-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc998-128">DateTimeOffset</span></span>|<span data-ttu-id="dc998-129">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dc998-129">The date and time when the page was created.</span></span>|
|<span data-ttu-id="dc998-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc998-130">lastModifiedDateTime</span></span>|<span data-ttu-id="dc998-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc998-131">DateTimeOffset</span></span>|<span data-ttu-id="dc998-132">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="dc998-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="dc998-133">id</span><span class="sxs-lookup"><span data-stu-id="dc998-133">id</span></span>|<span data-ttu-id="dc998-134">String</span><span class="sxs-lookup"><span data-stu-id="dc998-134">String</span></span>|<span data-ttu-id="dc998-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dc998-135">Key of the setting.</span></span>|
|<span data-ttu-id="dc998-136">version</span><span class="sxs-lookup"><span data-stu-id="dc998-136">version</span></span>|<span data-ttu-id="dc998-137">String</span><span class="sxs-lookup"><span data-stu-id="dc998-137">String</span></span>|<span data-ttu-id="dc998-138">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="dc998-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc998-139">关系</span><span class="sxs-lookup"><span data-stu-id="dc998-139">Relationships</span></span>
<span data-ttu-id="dc998-140">无</span><span class="sxs-lookup"><span data-stu-id="dc998-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc998-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc998-141">JSON Representation</span></span>
<span data-ttu-id="dc998-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc998-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



