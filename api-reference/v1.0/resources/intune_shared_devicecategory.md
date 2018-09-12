# <a name="devicecategory-resource-type"></a><span data-ttu-id="5612e-101">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="5612e-101">deviceCategory resource type</span></span>

> <span data-ttu-id="5612e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5612e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5612e-103">设备类别提供了整理设备的方法。</span><span class="sxs-lookup"><span data-stu-id="5612e-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="5612e-104">公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。</span><span class="sxs-lookup"><span data-stu-id="5612e-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="5612e-105">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="5612e-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="5612e-106">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="5612e-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="5612e-107">方法</span><span class="sxs-lookup"><span data-stu-id="5612e-107">Methods</span></span>
|<span data-ttu-id="5612e-108">方法</span><span class="sxs-lookup"><span data-stu-id="5612e-108">Method</span></span>|<span data-ttu-id="5612e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5612e-109">Return Type</span></span>|<span data-ttu-id="5612e-110">说明</span><span class="sxs-lookup"><span data-stu-id="5612e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5612e-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5612e-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) objects.</span></span>|
|<span data-ttu-id="5612e-112">[Get deviceCategory](../api/intune_shared_devicecategory_get.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5612e-112">[Get deviceCategory](../api/intune_shared_devicecategory_get.md) object.</span></span>|
|<span data-ttu-id="5612e-113">[Create deviceCategory](../api/intune_shared_devicecategory_create.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5612e-113">Create a new [deviceCategory](../api/intune_shared_devicecategory_create.md) object.</span></span>|
|<span data-ttu-id="5612e-114">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md)。</span><span class="sxs-lookup"><span data-stu-id="5612e-114">Delete deviceCategory</span></span>|
|<span data-ttu-id="5612e-115">[Update deviceCategory](../api/intune_shared_devicecategory_update.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5612e-115">Update the properties of a [deviceCategory](../api/intune_shared_devicecategory_update.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5612e-116">属性</span><span class="sxs-lookup"><span data-stu-id="5612e-116">Properties</span></span>
|<span data-ttu-id="5612e-117">属性</span><span class="sxs-lookup"><span data-stu-id="5612e-117">Property</span></span>|<span data-ttu-id="5612e-118">类型</span><span class="sxs-lookup"><span data-stu-id="5612e-118">Type</span></span>|<span data-ttu-id="5612e-119">说明</span><span class="sxs-lookup"><span data-stu-id="5612e-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5612e-120">ID</span><span class="sxs-lookup"><span data-stu-id="5612e-120">id</span></span>|<span data-ttu-id="5612e-121">字符串</span><span class="sxs-lookup"><span data-stu-id="5612e-121">String</span></span>|<span data-ttu-id="5612e-122">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5612e-122">Unique identifier for the device category.</span></span> <span data-ttu-id="5612e-123">只读。</span><span class="sxs-lookup"><span data-stu-id="5612e-123">Read-only.</span></span>|
|<span data-ttu-id="5612e-124">**起始安排**</span><span class="sxs-lookup"><span data-stu-id="5612e-124">**On-boarding**</span></span>|
|<span data-ttu-id="5612e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="5612e-125">displayName</span></span>|<span data-ttu-id="5612e-126">字符串</span><span class="sxs-lookup"><span data-stu-id="5612e-126">String</span></span>|<span data-ttu-id="5612e-127">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5612e-127">Display name for the device category.</span></span>|
|<span data-ttu-id="5612e-128">说明</span><span class="sxs-lookup"><span data-stu-id="5612e-128">description</span></span>|<span data-ttu-id="5612e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="5612e-129">String</span></span>|<span data-ttu-id="5612e-130">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="5612e-130">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5612e-131">关系</span><span class="sxs-lookup"><span data-stu-id="5612e-131">Relationships</span></span>
<span data-ttu-id="5612e-132">无</span><span class="sxs-lookup"><span data-stu-id="5612e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5612e-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5612e-133">JSON Representation</span></span>
<span data-ttu-id="5612e-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5612e-134">Here is a JSON representation of the resource.</span></span>
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



