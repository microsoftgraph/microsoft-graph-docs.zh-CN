# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="10df2-101">managedDeviceMobileAppConfigurationUserSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="10df2-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="10df2-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10df2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10df2-103">包含 MDM 移动应用配置用户状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="10df2-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="10df2-104">方法</span><span class="sxs-lookup"><span data-stu-id="10df2-104">Methods</span></span>
|<span data-ttu-id="10df2-105">方法</span><span class="sxs-lookup"><span data-stu-id="10df2-105">Method</span></span>|<span data-ttu-id="10df2-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="10df2-106">Return Type</span></span>|<span data-ttu-id="10df2-107">说明</span><span class="sxs-lookup"><span data-stu-id="10df2-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10df2-108">获取 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="10df2-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="10df2-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="10df2-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="10df2-110">读取 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10df2-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="10df2-111">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="10df2-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="10df2-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="10df2-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="10df2-113">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10df2-113">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10df2-114">属性</span><span class="sxs-lookup"><span data-stu-id="10df2-114">Properties</span></span>
|<span data-ttu-id="10df2-115">属性</span><span class="sxs-lookup"><span data-stu-id="10df2-115">Property</span></span>|<span data-ttu-id="10df2-116">类型</span><span class="sxs-lookup"><span data-stu-id="10df2-116">Type</span></span>|<span data-ttu-id="10df2-117">说明</span><span class="sxs-lookup"><span data-stu-id="10df2-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10df2-118">ID</span><span class="sxs-lookup"><span data-stu-id="10df2-118">id</span></span>|<span data-ttu-id="10df2-119">字符串</span><span class="sxs-lookup"><span data-stu-id="10df2-119">String</span></span>|<span data-ttu-id="10df2-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="10df2-120">Key of the entity.</span></span>|
|<span data-ttu-id="10df2-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="10df2-121">pendingCount</span></span>|<span data-ttu-id="10df2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="10df2-122">Int32</span></span>|<span data-ttu-id="10df2-123">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="10df2-123">Number of pending Users</span></span>|
|<span data-ttu-id="10df2-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="10df2-124">notApplicableCount</span></span>|<span data-ttu-id="10df2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="10df2-125">Int32</span></span>|<span data-ttu-id="10df2-126">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="10df2-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="10df2-127">successCount</span><span class="sxs-lookup"><span data-stu-id="10df2-127">successCount</span></span>|<span data-ttu-id="10df2-128">Int32</span><span class="sxs-lookup"><span data-stu-id="10df2-128">Int32</span></span>|<span data-ttu-id="10df2-129">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="10df2-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="10df2-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="10df2-130">errorCount</span></span>|<span data-ttu-id="10df2-131">Int32</span><span class="sxs-lookup"><span data-stu-id="10df2-131">Int32</span></span>|<span data-ttu-id="10df2-132">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="10df2-132">Number of error Users</span></span>|
|<span data-ttu-id="10df2-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="10df2-133">failedCount</span></span>|<span data-ttu-id="10df2-134">Int32</span><span class="sxs-lookup"><span data-stu-id="10df2-134">Int32</span></span>|<span data-ttu-id="10df2-135">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="10df2-135">Number of failed Users</span></span>|
|<span data-ttu-id="10df2-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="10df2-136">lastUpdateDateTime</span></span>|<span data-ttu-id="10df2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10df2-137">DateTimeOffset</span></span>|<span data-ttu-id="10df2-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="10df2-138">Last update time</span></span>|
|<span data-ttu-id="10df2-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="10df2-139">configurationVersion</span></span>|<span data-ttu-id="10df2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="10df2-140">Int32</span></span>|<span data-ttu-id="10df2-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="10df2-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="10df2-142">关系</span><span class="sxs-lookup"><span data-stu-id="10df2-142">Relationships</span></span>
<span data-ttu-id="10df2-143">无</span><span class="sxs-lookup"><span data-stu-id="10df2-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10df2-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10df2-144">JSON Representation</span></span>
<span data-ttu-id="10df2-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10df2-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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








