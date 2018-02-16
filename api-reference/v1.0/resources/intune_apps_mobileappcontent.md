# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="c8323-101">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8323-101">mobileAppContent resource type</span></span>

> <span data-ttu-id="c8323-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c8323-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8323-103">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="c8323-103">Contains content properties for a specific app version.</span></span> <span data-ttu-id="c8323-104">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="c8323-104">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="c8323-105">方法</span><span class="sxs-lookup"><span data-stu-id="c8323-105">Methods</span></span>
|<span data-ttu-id="c8323-106">方法</span><span class="sxs-lookup"><span data-stu-id="c8323-106">Method</span></span>|<span data-ttu-id="c8323-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8323-107">Return Type</span></span>|<span data-ttu-id="c8323-108">说明</span><span class="sxs-lookup"><span data-stu-id="c8323-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8323-109">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="c8323-109">List mobileAppContents</span></span>](../api/intune_apps_mobileappcontent_list.md)|<span data-ttu-id="c8323-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8323-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) collection</span></span>|<span data-ttu-id="c8323-111">列出 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8323-111">List properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="c8323-112">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8323-112">Get mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_get.md)|[<span data-ttu-id="c8323-113">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8323-113">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="c8323-114">读取 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8323-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c8323-115">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8323-115">Create mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_create.md)|[<span data-ttu-id="c8323-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8323-116">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="c8323-117">创建新的 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8323-117">Create a new [plannerBucket](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c8323-118">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8323-118">Delete mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_delete.md)|<span data-ttu-id="c8323-119">无</span><span class="sxs-lookup"><span data-stu-id="c8323-119">None</span></span>|<span data-ttu-id="c8323-120">删除 [mobileAppContent](../resources/intune_apps_mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="c8323-120">Deletes a [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span></span>|
|[<span data-ttu-id="c8323-121">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8323-121">Update mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_update.md)|[<span data-ttu-id="c8323-122">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8323-122">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="c8323-123">更新 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8323-123">Update the properties of a [calendar](../resources/intune_apps_mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8323-124">属性</span><span class="sxs-lookup"><span data-stu-id="c8323-124">Properties</span></span>
|<span data-ttu-id="c8323-125">属性</span><span class="sxs-lookup"><span data-stu-id="c8323-125">Property</span></span>|<span data-ttu-id="c8323-126">类型</span><span class="sxs-lookup"><span data-stu-id="c8323-126">Type</span></span>|<span data-ttu-id="c8323-127">说明</span><span class="sxs-lookup"><span data-stu-id="c8323-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8323-128">id</span><span class="sxs-lookup"><span data-stu-id="c8323-128">id</span></span>|<span data-ttu-id="c8323-129">String</span><span class="sxs-lookup"><span data-stu-id="c8323-129">String</span></span>|<span data-ttu-id="c8323-130">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="c8323-130">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8323-131">关系</span><span class="sxs-lookup"><span data-stu-id="c8323-131">Relationships</span></span>
|<span data-ttu-id="c8323-132">关系</span><span class="sxs-lookup"><span data-stu-id="c8323-132">Relationship</span></span>|<span data-ttu-id="c8323-133">类型</span><span class="sxs-lookup"><span data-stu-id="c8323-133">Type</span></span>|<span data-ttu-id="c8323-134">说明</span><span class="sxs-lookup"><span data-stu-id="c8323-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8323-135">files</span><span class="sxs-lookup"><span data-stu-id="c8323-135">files</span></span>|<span data-ttu-id="c8323-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8323-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="c8323-137">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="c8323-137">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8323-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8323-138">JSON Representation</span></span>
<span data-ttu-id="c8323-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8323-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



