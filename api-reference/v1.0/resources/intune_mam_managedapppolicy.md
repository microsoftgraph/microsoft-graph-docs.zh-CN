# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="d482a-101">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d482a-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="d482a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d482a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d482a-103">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="d482a-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="d482a-104">方法</span><span class="sxs-lookup"><span data-stu-id="d482a-104">Methods</span></span>
|<span data-ttu-id="d482a-105">方法</span><span class="sxs-lookup"><span data-stu-id="d482a-105">Method</span></span>|<span data-ttu-id="d482a-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="d482a-106">Return Type</span></span>|<span data-ttu-id="d482a-107">说明</span><span class="sxs-lookup"><span data-stu-id="d482a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d482a-108">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="d482a-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="d482a-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d482a-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="d482a-110">列出 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d482a-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="d482a-111">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="d482a-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="d482a-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="d482a-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="d482a-113">读取 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d482a-113">Read properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="d482a-114">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="d482a-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="d482a-115">无</span><span class="sxs-lookup"><span data-stu-id="d482a-115">None</span></span>|<span data-ttu-id="d482a-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d482a-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d482a-117">属性</span><span class="sxs-lookup"><span data-stu-id="d482a-117">Properties</span></span>
|<span data-ttu-id="d482a-118">属性</span><span class="sxs-lookup"><span data-stu-id="d482a-118">Property</span></span>|<span data-ttu-id="d482a-119">类型</span><span class="sxs-lookup"><span data-stu-id="d482a-119">Type</span></span>|<span data-ttu-id="d482a-120">说明</span><span class="sxs-lookup"><span data-stu-id="d482a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d482a-121">displayName</span><span class="sxs-lookup"><span data-stu-id="d482a-121">displayName</span></span>|<span data-ttu-id="d482a-122">字符串</span><span class="sxs-lookup"><span data-stu-id="d482a-122">String</span></span>|<span data-ttu-id="d482a-123">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="d482a-123">Policy display name.</span></span>|
|<span data-ttu-id="d482a-124">描述</span><span class="sxs-lookup"><span data-stu-id="d482a-124">description</span></span>|<span data-ttu-id="d482a-125">字符串</span><span class="sxs-lookup"><span data-stu-id="d482a-125">String</span></span>|<span data-ttu-id="d482a-126">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d482a-126">The policy's description.</span></span>|
|<span data-ttu-id="d482a-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d482a-127">createdDateTime</span></span>|<span data-ttu-id="d482a-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d482a-128">DateTimeOffset</span></span>|<span data-ttu-id="d482a-129">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d482a-129">The date and time the policy was created.</span></span>|
|<span data-ttu-id="d482a-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d482a-130">lastModifiedDateTime</span></span>|<span data-ttu-id="d482a-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d482a-131">DateTimeOffset</span></span>|<span data-ttu-id="d482a-132">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="d482a-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="d482a-133">ID</span><span class="sxs-lookup"><span data-stu-id="d482a-133">id</span></span>|<span data-ttu-id="d482a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d482a-134">String</span></span>|<span data-ttu-id="d482a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d482a-135">Key of the entity.</span></span>|
|<span data-ttu-id="d482a-136">version</span><span class="sxs-lookup"><span data-stu-id="d482a-136">version</span></span>|<span data-ttu-id="d482a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="d482a-137">String</span></span>|<span data-ttu-id="d482a-138">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d482a-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d482a-139">关系</span><span class="sxs-lookup"><span data-stu-id="d482a-139">Relationships</span></span>
<span data-ttu-id="d482a-140">无</span><span class="sxs-lookup"><span data-stu-id="d482a-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d482a-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d482a-141">JSON Representation</span></span>
<span data-ttu-id="d482a-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d482a-142">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}-->
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








