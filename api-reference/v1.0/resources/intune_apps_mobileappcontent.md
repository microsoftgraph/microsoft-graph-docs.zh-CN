# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="ccb3b-101">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ccb3b-101">mobileAppContent resource type</span></span>

> <span data-ttu-id="ccb3b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ccb3b-103">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-103">Contains content properties for a specific app version.</span></span> <span data-ttu-id="ccb3b-104">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-104">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="ccb3b-105">方法</span><span class="sxs-lookup"><span data-stu-id="ccb3b-105">Methods</span></span>
|<span data-ttu-id="ccb3b-106">方法</span><span class="sxs-lookup"><span data-stu-id="ccb3b-106">Method</span></span>|<span data-ttu-id="ccb3b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ccb3b-107">Return Type</span></span>|<span data-ttu-id="ccb3b-108">说明</span><span class="sxs-lookup"><span data-stu-id="ccb3b-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ccb3b-109">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="ccb3b-109">List mobileAppContents</span></span>](../api/intune_apps_mobileappcontent_list.md)|<span data-ttu-id="ccb3b-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccb3b-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) collection</span></span>|<span data-ttu-id="ccb3b-111">列出 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-111">List properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="ccb3b-112">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccb3b-112">Get mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_get.md)|[<span data-ttu-id="ccb3b-113">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccb3b-113">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="ccb3b-114">读取 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-114">Read properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ccb3b-115">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccb3b-115">Create mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_create.md)|[<span data-ttu-id="ccb3b-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccb3b-116">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="ccb3b-117">创建新的 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-117">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ccb3b-118">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccb3b-118">Delete mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_delete.md)|<span data-ttu-id="ccb3b-119">无</span><span class="sxs-lookup"><span data-stu-id="ccb3b-119">None</span></span>|<span data-ttu-id="ccb3b-120">删除 [mobileAppContent](../resources/intune_apps_mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-120">Deletes a [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span></span>|
|[<span data-ttu-id="ccb3b-121">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccb3b-121">Update mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_update.md)|[<span data-ttu-id="ccb3b-122">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccb3b-122">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="ccb3b-123">更新 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-123">Update the properties of a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ccb3b-124">属性</span><span class="sxs-lookup"><span data-stu-id="ccb3b-124">Properties</span></span>
|<span data-ttu-id="ccb3b-125">属性</span><span class="sxs-lookup"><span data-stu-id="ccb3b-125">Property</span></span>|<span data-ttu-id="ccb3b-126">类型</span><span class="sxs-lookup"><span data-stu-id="ccb3b-126">Type</span></span>|<span data-ttu-id="ccb3b-127">说明</span><span class="sxs-lookup"><span data-stu-id="ccb3b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccb3b-128">id</span><span class="sxs-lookup"><span data-stu-id="ccb3b-128">id</span></span>|<span data-ttu-id="ccb3b-129">String</span><span class="sxs-lookup"><span data-stu-id="ccb3b-129">String</span></span>|<span data-ttu-id="ccb3b-130">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-130">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccb3b-131">关系</span><span class="sxs-lookup"><span data-stu-id="ccb3b-131">Relationships</span></span>
|<span data-ttu-id="ccb3b-132">关系</span><span class="sxs-lookup"><span data-stu-id="ccb3b-132">Relationship</span></span>|<span data-ttu-id="ccb3b-133">类型</span><span class="sxs-lookup"><span data-stu-id="ccb3b-133">Type</span></span>|<span data-ttu-id="ccb3b-134">说明</span><span class="sxs-lookup"><span data-stu-id="ccb3b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccb3b-135">files</span><span class="sxs-lookup"><span data-stu-id="ccb3b-135">files</span></span>|<span data-ttu-id="ccb3b-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccb3b-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="ccb3b-137">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-137">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ccb3b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ccb3b-138">JSON Representation</span></span>
<span data-ttu-id="ccb3b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccb3b-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mobileAppContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



