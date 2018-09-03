# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="6a776-101">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a776-101">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="6a776-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6a776-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a776-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6a776-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="6a776-104">方法</span><span class="sxs-lookup"><span data-stu-id="6a776-104">Methods</span></span>
|<span data-ttu-id="6a776-105">方法</span><span class="sxs-lookup"><span data-stu-id="6a776-105">Method</span></span>|<span data-ttu-id="6a776-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a776-106">Return Type</span></span>|<span data-ttu-id="6a776-107">说明</span><span class="sxs-lookup"><span data-stu-id="6a776-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a776-108">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="6a776-108">Get deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[<span data-ttu-id="6a776-109">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="6a776-109">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="6a776-110">读取 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a776-110">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="6a776-111">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="6a776-111">Update deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[<span data-ttu-id="6a776-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="6a776-112">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="6a776-113">更新 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a776-113">Update the properties of a [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a776-114">属性</span><span class="sxs-lookup"><span data-stu-id="6a776-114">Properties</span></span>
|<span data-ttu-id="6a776-115">属性</span><span class="sxs-lookup"><span data-stu-id="6a776-115">Property</span></span>|<span data-ttu-id="6a776-116">类型</span><span class="sxs-lookup"><span data-stu-id="6a776-116">Type</span></span>|<span data-ttu-id="6a776-117">说明</span><span class="sxs-lookup"><span data-stu-id="6a776-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a776-118">ID</span><span class="sxs-lookup"><span data-stu-id="6a776-118">id</span></span>|<span data-ttu-id="6a776-119">字符串</span><span class="sxs-lookup"><span data-stu-id="6a776-119">String</span></span>|<span data-ttu-id="6a776-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6a776-120">Key of the entity.</span></span>|
|<span data-ttu-id="6a776-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6a776-121">pendingCount</span></span>|<span data-ttu-id="6a776-122">Int32</span><span class="sxs-lookup"><span data-stu-id="6a776-122">Int32</span></span>|<span data-ttu-id="6a776-123">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="6a776-123">Number of pending Users</span></span>|
|<span data-ttu-id="6a776-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6a776-124">notApplicableCount</span></span>|<span data-ttu-id="6a776-125">Int32</span><span class="sxs-lookup"><span data-stu-id="6a776-125">Int32</span></span>|<span data-ttu-id="6a776-126">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="6a776-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="6a776-127">successCount</span><span class="sxs-lookup"><span data-stu-id="6a776-127">successCount</span></span>|<span data-ttu-id="6a776-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6a776-128">Int32</span></span>|<span data-ttu-id="6a776-129">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="6a776-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="6a776-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="6a776-130">errorCount</span></span>|<span data-ttu-id="6a776-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6a776-131">Int32</span></span>|<span data-ttu-id="6a776-132">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="6a776-132">Number of error Users</span></span>|
|<span data-ttu-id="6a776-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="6a776-133">failedCount</span></span>|<span data-ttu-id="6a776-134">Int32</span><span class="sxs-lookup"><span data-stu-id="6a776-134">Int32</span></span>|<span data-ttu-id="6a776-135">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="6a776-135">Number of failed Users</span></span>|
|<span data-ttu-id="6a776-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6a776-136">lastUpdateDateTime</span></span>|<span data-ttu-id="6a776-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a776-137">DateTimeOffset</span></span>|<span data-ttu-id="6a776-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="6a776-138">Last update time</span></span>|
|<span data-ttu-id="6a776-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6a776-139">configurationVersion</span></span>|<span data-ttu-id="6a776-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6a776-140">Int32</span></span>|<span data-ttu-id="6a776-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="6a776-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a776-142">关系</span><span class="sxs-lookup"><span data-stu-id="6a776-142">Relationships</span></span>
<span data-ttu-id="6a776-143">无</span><span class="sxs-lookup"><span data-stu-id="6a776-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a776-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a776-144">JSON Representation</span></span>
<span data-ttu-id="6a776-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a776-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



