# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="a2bac-101">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2bac-101">mobileAppContent resource type</span></span>

> <span data-ttu-id="a2bac-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a2bac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2bac-103">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="a2bac-103">Contains content properties for a specific app version.</span></span> <span data-ttu-id="a2bac-104">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="a2bac-104">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="a2bac-105">方法</span><span class="sxs-lookup"><span data-stu-id="a2bac-105">Methods</span></span>
|<span data-ttu-id="a2bac-106">方法</span><span class="sxs-lookup"><span data-stu-id="a2bac-106">Method</span></span>|<span data-ttu-id="a2bac-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2bac-107">Return Type</span></span>|<span data-ttu-id="a2bac-108">说明</span><span class="sxs-lookup"><span data-stu-id="a2bac-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2bac-109">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="a2bac-109">List mobileAppContents</span></span>](../api/intune_apps_mobileappcontent_list.md)|<span data-ttu-id="a2bac-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2bac-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) collection</span></span>|<span data-ttu-id="a2bac-111">列出 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2bac-111">List properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="a2bac-112">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a2bac-112">Get mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_get.md)|[<span data-ttu-id="a2bac-113">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a2bac-113">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="a2bac-114">读取 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2bac-114">Read properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a2bac-115">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a2bac-115">Create mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_create.md)|[<span data-ttu-id="a2bac-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a2bac-116">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="a2bac-117">创建新的 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2bac-117">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a2bac-118">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a2bac-118">Delete mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_delete.md)|<span data-ttu-id="a2bac-119">无</span><span class="sxs-lookup"><span data-stu-id="a2bac-119">None</span></span>|<span data-ttu-id="a2bac-120">删除 [mobileAppContent](../resources/intune_apps_mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="a2bac-120">Deletes a [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span></span>|
|[<span data-ttu-id="a2bac-121">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a2bac-121">Update mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_update.md)|[<span data-ttu-id="a2bac-122">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a2bac-122">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="a2bac-123">更新 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2bac-123">Update the properties of a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2bac-124">属性</span><span class="sxs-lookup"><span data-stu-id="a2bac-124">Properties</span></span>
|<span data-ttu-id="a2bac-125">属性</span><span class="sxs-lookup"><span data-stu-id="a2bac-125">Property</span></span>|<span data-ttu-id="a2bac-126">类型</span><span class="sxs-lookup"><span data-stu-id="a2bac-126">Type</span></span>|<span data-ttu-id="a2bac-127">说明</span><span class="sxs-lookup"><span data-stu-id="a2bac-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2bac-128">ID</span><span class="sxs-lookup"><span data-stu-id="a2bac-128">id</span></span>|<span data-ttu-id="a2bac-129">String</span><span class="sxs-lookup"><span data-stu-id="a2bac-129">String</span></span>|<span data-ttu-id="a2bac-130">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="a2bac-130">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2bac-131">关系</span><span class="sxs-lookup"><span data-stu-id="a2bac-131">Relationships</span></span>
|<span data-ttu-id="a2bac-132">关系</span><span class="sxs-lookup"><span data-stu-id="a2bac-132">Relationship</span></span>|<span data-ttu-id="a2bac-133">类型</span><span class="sxs-lookup"><span data-stu-id="a2bac-133">Type</span></span>|<span data-ttu-id="a2bac-134">说明</span><span class="sxs-lookup"><span data-stu-id="a2bac-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2bac-135">files</span><span class="sxs-lookup"><span data-stu-id="a2bac-135">files</span></span>|<span data-ttu-id="a2bac-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2bac-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="a2bac-137">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="a2bac-137">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2bac-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2bac-138">JSON Representation</span></span>
<span data-ttu-id="a2bac-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2bac-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```








