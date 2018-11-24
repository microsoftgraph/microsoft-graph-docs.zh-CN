# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="4aeff-101">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="4aeff-101">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="4aeff-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4aeff-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4aeff-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4aeff-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="4aeff-104">方法</span><span class="sxs-lookup"><span data-stu-id="4aeff-104">Methods</span></span>
|<span data-ttu-id="4aeff-105">方法</span><span class="sxs-lookup"><span data-stu-id="4aeff-105">Method</span></span>|<span data-ttu-id="4aeff-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="4aeff-106">Return Type</span></span>|<span data-ttu-id="4aeff-107">说明</span><span class="sxs-lookup"><span data-stu-id="4aeff-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4aeff-108">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4aeff-108">Get deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[<span data-ttu-id="4aeff-109">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4aeff-109">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="4aeff-110">读取 [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4aeff-110">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="4aeff-111">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4aeff-111">Update deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_update.md)|[<span data-ttu-id="4aeff-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4aeff-112">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="4aeff-113">更新 [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4aeff-113">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4aeff-114">属性</span><span class="sxs-lookup"><span data-stu-id="4aeff-114">Properties</span></span>
|<span data-ttu-id="4aeff-115">属性</span><span class="sxs-lookup"><span data-stu-id="4aeff-115">Property</span></span>|<span data-ttu-id="4aeff-116">类型</span><span class="sxs-lookup"><span data-stu-id="4aeff-116">Type</span></span>|<span data-ttu-id="4aeff-117">说明</span><span class="sxs-lookup"><span data-stu-id="4aeff-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4aeff-118">id</span><span class="sxs-lookup"><span data-stu-id="4aeff-118">id</span></span>|<span data-ttu-id="4aeff-119">String</span><span class="sxs-lookup"><span data-stu-id="4aeff-119">String</span></span>|<span data-ttu-id="4aeff-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4aeff-120">Key of the entity.</span></span>|
|<span data-ttu-id="4aeff-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4aeff-121">pendingCount</span></span>|<span data-ttu-id="4aeff-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4aeff-122">Int32</span></span>|<span data-ttu-id="4aeff-123">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="4aeff-123">Number of pending Users</span></span>|
|<span data-ttu-id="4aeff-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4aeff-124">notApplicableCount</span></span>|<span data-ttu-id="4aeff-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4aeff-125">Int32</span></span>|<span data-ttu-id="4aeff-126">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="4aeff-126">Number of not applicable users</span></span>|
|<span data-ttu-id="4aeff-127">successCount</span><span class="sxs-lookup"><span data-stu-id="4aeff-127">successCount</span></span>|<span data-ttu-id="4aeff-128">Int32</span><span class="sxs-lookup"><span data-stu-id="4aeff-128">Int32</span></span>|<span data-ttu-id="4aeff-129">成功的用户数量</span><span class="sxs-lookup"><span data-stu-id="4aeff-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="4aeff-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="4aeff-130">errorCount</span></span>|<span data-ttu-id="4aeff-131">Int32</span><span class="sxs-lookup"><span data-stu-id="4aeff-131">Int32</span></span>|<span data-ttu-id="4aeff-132">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="4aeff-132">Number of error Users</span></span>|
|<span data-ttu-id="4aeff-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="4aeff-133">failedCount</span></span>|<span data-ttu-id="4aeff-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4aeff-134">Int32</span></span>|<span data-ttu-id="4aeff-135">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="4aeff-135">Number of failed Users</span></span>|
|<span data-ttu-id="4aeff-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4aeff-136">lastUpdateDateTime</span></span>|<span data-ttu-id="4aeff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4aeff-137">DateTimeOffset</span></span>|<span data-ttu-id="4aeff-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="4aeff-138">Last update time</span></span>|
|<span data-ttu-id="4aeff-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4aeff-139">configurationVersion</span></span>|<span data-ttu-id="4aeff-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4aeff-140">Int32</span></span>|<span data-ttu-id="4aeff-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="4aeff-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="4aeff-142">关系</span><span class="sxs-lookup"><span data-stu-id="4aeff-142">Relationships</span></span>
<span data-ttu-id="4aeff-143">无</span><span class="sxs-lookup"><span data-stu-id="4aeff-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4aeff-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4aeff-144">JSON Representation</span></span>
<span data-ttu-id="4aeff-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4aeff-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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



