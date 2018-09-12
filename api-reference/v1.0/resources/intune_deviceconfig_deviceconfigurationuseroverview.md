# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="fcc7e-101">deviceConfigurationUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcc7e-101">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="fcc7e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fcc7e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcc7e-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fcc7e-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="fcc7e-104">方法</span><span class="sxs-lookup"><span data-stu-id="fcc7e-104">Methods</span></span>
|<span data-ttu-id="fcc7e-105">方法</span><span class="sxs-lookup"><span data-stu-id="fcc7e-105">Method</span></span>|<span data-ttu-id="fcc7e-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="fcc7e-106">Return Type</span></span>|<span data-ttu-id="fcc7e-107">说明</span><span class="sxs-lookup"><span data-stu-id="fcc7e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fcc7e-108">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="fcc7e-108">Get deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[<span data-ttu-id="fcc7e-109">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="fcc7e-109">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="fcc7e-110">读取 [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fcc7e-110">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="fcc7e-111">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="fcc7e-111">Update deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_update.md)|[<span data-ttu-id="fcc7e-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="fcc7e-112">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="fcc7e-113">更新 [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fcc7e-113">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fcc7e-114">属性</span><span class="sxs-lookup"><span data-stu-id="fcc7e-114">Properties</span></span>
|<span data-ttu-id="fcc7e-115">属性</span><span class="sxs-lookup"><span data-stu-id="fcc7e-115">Property</span></span>|<span data-ttu-id="fcc7e-116">类型</span><span class="sxs-lookup"><span data-stu-id="fcc7e-116">Type</span></span>|<span data-ttu-id="fcc7e-117">说明</span><span class="sxs-lookup"><span data-stu-id="fcc7e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc7e-118">ID</span><span class="sxs-lookup"><span data-stu-id="fcc7e-118">id</span></span>|<span data-ttu-id="fcc7e-119">字符串</span><span class="sxs-lookup"><span data-stu-id="fcc7e-119">String</span></span>|<span data-ttu-id="fcc7e-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fcc7e-120">Key of the entity.</span></span>|
|<span data-ttu-id="fcc7e-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="fcc7e-121">pendingCount</span></span>|<span data-ttu-id="fcc7e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc7e-122">Int32</span></span>|<span data-ttu-id="fcc7e-123">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="fcc7e-123">Number of pending Users</span></span>|
|<span data-ttu-id="fcc7e-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="fcc7e-124">notApplicableCount</span></span>|<span data-ttu-id="fcc7e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc7e-125">Int32</span></span>|<span data-ttu-id="fcc7e-126">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="fcc7e-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="fcc7e-127">successCount</span><span class="sxs-lookup"><span data-stu-id="fcc7e-127">successCount</span></span>|<span data-ttu-id="fcc7e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc7e-128">Int32</span></span>|<span data-ttu-id="fcc7e-129">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="fcc7e-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="fcc7e-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="fcc7e-130">errorCount</span></span>|<span data-ttu-id="fcc7e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc7e-131">Int32</span></span>|<span data-ttu-id="fcc7e-132">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="fcc7e-132">Number of error Users</span></span>|
|<span data-ttu-id="fcc7e-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="fcc7e-133">failedCount</span></span>|<span data-ttu-id="fcc7e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc7e-134">Int32</span></span>|<span data-ttu-id="fcc7e-135">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="fcc7e-135">Number of failed Users</span></span>|
|<span data-ttu-id="fcc7e-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc7e-136">lastUpdateDateTime</span></span>|<span data-ttu-id="fcc7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcc7e-137">DateTimeOffset</span></span>|<span data-ttu-id="fcc7e-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="fcc7e-138">Last update time</span></span>|
|<span data-ttu-id="fcc7e-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="fcc7e-139">configurationVersion</span></span>|<span data-ttu-id="fcc7e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc7e-140">Int32</span></span>|<span data-ttu-id="fcc7e-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="fcc7e-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcc7e-142">关系</span><span class="sxs-lookup"><span data-stu-id="fcc7e-142">Relationships</span></span>
<span data-ttu-id="fcc7e-143">无</span><span class="sxs-lookup"><span data-stu-id="fcc7e-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fcc7e-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcc7e-144">JSON Representation</span></span>
<span data-ttu-id="fcc7e-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcc7e-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}-->
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








