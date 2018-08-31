# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="d99fa-101">managedAppPolicyDeploymentSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d99fa-101">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="d99fa-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d99fa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d99fa-103">ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。</span><span class="sxs-lookup"><span data-stu-id="d99fa-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
## <a name="methods"></a><span data-ttu-id="d99fa-104">方法</span><span class="sxs-lookup"><span data-stu-id="d99fa-104">Methods</span></span>
|<span data-ttu-id="d99fa-105">方法</span><span class="sxs-lookup"><span data-stu-id="d99fa-105">Method</span></span>|<span data-ttu-id="d99fa-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="d99fa-106">Return Type</span></span>|<span data-ttu-id="d99fa-107">说明</span><span class="sxs-lookup"><span data-stu-id="d99fa-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d99fa-108">Get managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="d99fa-108">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune_mam_managedapppolicydeploymentsummary_get.md)|[<span data-ttu-id="d99fa-109">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="d99fa-109">managedAppPolicyDeploymentSummary</span></span>](../resources/intune_mam_managedapppolicydeploymentsummary.md)|<span data-ttu-id="d99fa-110">读取 [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d99fa-110">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="d99fa-111">Update managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="d99fa-111">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune_mam_managedapppolicydeploymentsummary_update.md)|[<span data-ttu-id="d99fa-112">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="d99fa-112">managedAppPolicyDeploymentSummary</span></span>](../resources/intune_mam_managedapppolicydeploymentsummary.md)|<span data-ttu-id="d99fa-113">更新 [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d99fa-113">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d99fa-114">属性</span><span class="sxs-lookup"><span data-stu-id="d99fa-114">Properties</span></span>
|<span data-ttu-id="d99fa-115">属性</span><span class="sxs-lookup"><span data-stu-id="d99fa-115">Property</span></span>|<span data-ttu-id="d99fa-116">类型</span><span class="sxs-lookup"><span data-stu-id="d99fa-116">Type</span></span>|<span data-ttu-id="d99fa-117">说明</span><span class="sxs-lookup"><span data-stu-id="d99fa-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d99fa-118">displayName</span><span class="sxs-lookup"><span data-stu-id="d99fa-118">displayName</span></span>|<span data-ttu-id="d99fa-119">字符串</span><span class="sxs-lookup"><span data-stu-id="d99fa-119">String</span></span>|<span data-ttu-id="d99fa-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d99fa-120">Not yet documented</span></span>|
|<span data-ttu-id="d99fa-121">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="d99fa-121">configurationDeployedUserCount</span></span>|<span data-ttu-id="d99fa-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d99fa-122">Int32</span></span>|<span data-ttu-id="d99fa-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d99fa-123">Not yet documented</span></span>|
|<span data-ttu-id="d99fa-124">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="d99fa-124">lastRefreshTime</span></span>|<span data-ttu-id="d99fa-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d99fa-125">DateTimeOffset</span></span>|<span data-ttu-id="d99fa-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d99fa-126">Not yet documented</span></span>|
|<span data-ttu-id="d99fa-127">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="d99fa-127">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="d99fa-128">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d99fa-128">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="d99fa-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d99fa-129">Not yet documented</span></span>|
|<span data-ttu-id="d99fa-130">id</span><span class="sxs-lookup"><span data-stu-id="d99fa-130">id</span></span>|<span data-ttu-id="d99fa-131">字符串</span><span class="sxs-lookup"><span data-stu-id="d99fa-131">String</span></span>|<span data-ttu-id="d99fa-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d99fa-132">Key of the entity.</span></span>|
|<span data-ttu-id="d99fa-133">version</span><span class="sxs-lookup"><span data-stu-id="d99fa-133">version</span></span>|<span data-ttu-id="d99fa-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d99fa-134">String</span></span>|<span data-ttu-id="d99fa-135">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d99fa-135">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d99fa-136">关系</span><span class="sxs-lookup"><span data-stu-id="d99fa-136">Relationships</span></span>
<span data-ttu-id="d99fa-137">无</span><span class="sxs-lookup"><span data-stu-id="d99fa-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d99fa-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d99fa-138">JSON Representation</span></span>
<span data-ttu-id="d99fa-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d99fa-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "String"
      },
      "configurationAppliedUserCount": 1024
    }
  ],
  "id": "String (identifier)",
  "version": "String"
}
```



