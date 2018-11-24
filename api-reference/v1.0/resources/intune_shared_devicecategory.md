# <a name="devicecategory-resource-type"></a><span data-ttu-id="270df-101">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="270df-101">deviceCategory resource type</span></span>

> <span data-ttu-id="270df-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="270df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="270df-103">设备类别提供了整理设备的方法。</span><span class="sxs-lookup"><span data-stu-id="270df-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="270df-104">公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。</span><span class="sxs-lookup"><span data-stu-id="270df-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="270df-105">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="270df-105"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="270df-106">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="270df-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="270df-107">方法</span><span class="sxs-lookup"><span data-stu-id="270df-107">Methods</span></span>
|<span data-ttu-id="270df-108">方法</span><span class="sxs-lookup"><span data-stu-id="270df-108">Method</span></span>|<span data-ttu-id="270df-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="270df-109">Return Type</span></span>|<span data-ttu-id="270df-110">说明</span><span class="sxs-lookup"><span data-stu-id="270df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270df-111">[列表 deviceCategories](../api/intune_shared_devicecategory_list.md)集合</span><span class="sxs-lookup"><span data-stu-id="270df-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) collection</span></span>|<span data-ttu-id="270df-112">列出 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="270df-112">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="270df-113">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="270df-113">Get deviceCategory</span></span>](../api/intune_shared_devicecategory_get.md)|<span data-ttu-id="270df-114">读取 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="270df-114">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="270df-115">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="270df-115">Create deviceCategory</span></span>](../api/intune_shared_devicecategory_create.md)|<span data-ttu-id="270df-116">创建新的 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="270df-116">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|<span data-ttu-id="270df-117">[删除 deviceCategory](../api/intune_shared_devicecategory_delete.md)。</span><span class="sxs-lookup"><span data-stu-id="270df-117">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md).</span></span>|
|[<span data-ttu-id="270df-118">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="270df-118">Update deviceCategory</span></span>](../api/intune_shared_devicecategory_update.md)|<span data-ttu-id="270df-119">更新 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="270df-119">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="270df-120">属性</span><span class="sxs-lookup"><span data-stu-id="270df-120">Properties</span></span>
|<span data-ttu-id="270df-121">属性</span><span class="sxs-lookup"><span data-stu-id="270df-121">Property</span></span>|<span data-ttu-id="270df-122">类型</span><span class="sxs-lookup"><span data-stu-id="270df-122">Type</span></span>|<span data-ttu-id="270df-123">说明</span><span class="sxs-lookup"><span data-stu-id="270df-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270df-124">id</span><span class="sxs-lookup"><span data-stu-id="270df-124">id</span></span>|<span data-ttu-id="270df-125">String</span><span class="sxs-lookup"><span data-stu-id="270df-125">String</span></span>|<span data-ttu-id="270df-126">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="270df-126">Unique identifier for the device category.</span></span> <span data-ttu-id="270df-127">只读。</span><span class="sxs-lookup"><span data-stu-id="270df-127">Read-only.</span></span>|
|<span data-ttu-id="270df-128">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="270df-128">**Onboarding**</span></span>|
|<span data-ttu-id="270df-129">displayName</span><span class="sxs-lookup"><span data-stu-id="270df-129">displayName</span></span>|<span data-ttu-id="270df-130">String</span><span class="sxs-lookup"><span data-stu-id="270df-130">String</span></span>|<span data-ttu-id="270df-131">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="270df-131">Display name for the device category.</span></span>|
|<span data-ttu-id="270df-132">description</span><span class="sxs-lookup"><span data-stu-id="270df-132">description</span></span>|<span data-ttu-id="270df-133">String</span><span class="sxs-lookup"><span data-stu-id="270df-133">String</span></span>|<span data-ttu-id="270df-134">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="270df-134">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="270df-135">关系</span><span class="sxs-lookup"><span data-stu-id="270df-135">Relationships</span></span>
<span data-ttu-id="270df-136">无</span><span class="sxs-lookup"><span data-stu-id="270df-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="270df-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="270df-137">JSON Representation</span></span>
<span data-ttu-id="270df-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="270df-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



