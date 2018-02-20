# <a name="devicecategory-resource-type"></a><span data-ttu-id="b351e-101">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="b351e-101">deviceCategory resource type</span></span>

> <span data-ttu-id="b351e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b351e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b351e-103">设备类别提供了整理设备的方法。</span><span class="sxs-lookup"><span data-stu-id="b351e-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="b351e-104">公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。</span><span class="sxs-lookup"><span data-stu-id="b351e-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="b351e-105">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="b351e-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="b351e-106">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="b351e-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>
## <a name="methods"></a><span data-ttu-id="b351e-107">方法</span><span class="sxs-lookup"><span data-stu-id="b351e-107">Methods</span></span>
|<span data-ttu-id="b351e-108">方法</span><span class="sxs-lookup"><span data-stu-id="b351e-108">Method</span></span>|<span data-ttu-id="b351e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b351e-109">Return Type</span></span>|<span data-ttu-id="b351e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b351e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b351e-111">List deviceCategories</span><span class="sxs-lookup"><span data-stu-id="b351e-111">List deviceCategories</span></span>](../api/intune_onboarding_devicecategory_list.md)|<span data-ttu-id="b351e-112">[deviceCategory](../resources/intune_onboarding_devicecategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b351e-112">[deviceCategory](../resources/intune_onboarding_devicecategory.md) collection</span></span>|<span data-ttu-id="b351e-113">列出 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b351e-113">List properties and relationships of the [deviceCategory](../resources/intune_onboarding_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="b351e-114">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b351e-114">Get deviceCategory</span></span>](../api/intune_onboarding_devicecategory_get.md)|[<span data-ttu-id="b351e-115">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b351e-115">deviceCategory</span></span>](../resources/intune_onboarding_devicecategory.md)|<span data-ttu-id="b351e-116">读取 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b351e-116">Read properties and relationships of [plannerPlanDetails](../resources/intune_onboarding_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b351e-117">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b351e-117">Create deviceCategory</span></span>](../api/intune_onboarding_devicecategory_create.md)|[<span data-ttu-id="b351e-118">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b351e-118">deviceCategory</span></span>](../resources/intune_onboarding_devicecategory.md)|<span data-ttu-id="b351e-119">创建新的 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b351e-119">Create a new [plannerBucket](../resources/intune_onboarding_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b351e-120">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b351e-120">Delete deviceCategory</span></span>](../api/intune_onboarding_devicecategory_delete.md)|<span data-ttu-id="b351e-121">无</span><span class="sxs-lookup"><span data-stu-id="b351e-121">None</span></span>|<span data-ttu-id="b351e-122">删除 [deviceCategory](../resources/intune_onboarding_devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="b351e-122">Deletes a [deviceCategory](../resources/intune_onboarding_devicecategory.md).</span></span>|
|[<span data-ttu-id="b351e-123">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b351e-123">Update deviceCategory</span></span>](../api/intune_onboarding_devicecategory_update.md)|[<span data-ttu-id="b351e-124">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b351e-124">deviceCategory</span></span>](../resources/intune_onboarding_devicecategory.md)|<span data-ttu-id="b351e-125">更新 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b351e-125">Update the properties of a [calendar](../resources/intune_onboarding_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b351e-126">属性</span><span class="sxs-lookup"><span data-stu-id="b351e-126">Properties</span></span>
|<span data-ttu-id="b351e-127">属性</span><span class="sxs-lookup"><span data-stu-id="b351e-127">Property</span></span>|<span data-ttu-id="b351e-128">类型</span><span class="sxs-lookup"><span data-stu-id="b351e-128">Type</span></span>|<span data-ttu-id="b351e-129">说明</span><span class="sxs-lookup"><span data-stu-id="b351e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b351e-130">id</span><span class="sxs-lookup"><span data-stu-id="b351e-130">id</span></span>|<span data-ttu-id="b351e-131">String</span><span class="sxs-lookup"><span data-stu-id="b351e-131">String</span></span>|<span data-ttu-id="b351e-132">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b351e-132">Unique identifier for the device category.</span></span> <span data-ttu-id="b351e-133">只读。</span><span class="sxs-lookup"><span data-stu-id="b351e-133">Read-only.</span></span>|
|<span data-ttu-id="b351e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b351e-134">displayName</span></span>|<span data-ttu-id="b351e-135">String</span><span class="sxs-lookup"><span data-stu-id="b351e-135">String</span></span>|<span data-ttu-id="b351e-136">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b351e-136">Display name for the device category.</span></span>|
|<span data-ttu-id="b351e-137">description</span><span class="sxs-lookup"><span data-stu-id="b351e-137">description</span></span>|<span data-ttu-id="b351e-138">String</span><span class="sxs-lookup"><span data-stu-id="b351e-138">String</span></span>|<span data-ttu-id="b351e-139">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="b351e-139">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b351e-140">关系</span><span class="sxs-lookup"><span data-stu-id="b351e-140">Relationships</span></span>
<span data-ttu-id="b351e-141">无</span><span class="sxs-lookup"><span data-stu-id="b351e-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b351e-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b351e-142">JSON Representation</span></span>
<span data-ttu-id="b351e-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b351e-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



