# <a name="mobileapp-resource-type"></a><span data-ttu-id="d348a-101">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d348a-101">mobileApp resource type</span></span>

> <span data-ttu-id="d348a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d348a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d348a-103">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="d348a-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="d348a-104">方法</span><span class="sxs-lookup"><span data-stu-id="d348a-104">Methods</span></span>
|<span data-ttu-id="d348a-105">方法</span><span class="sxs-lookup"><span data-stu-id="d348a-105">Method</span></span>|<span data-ttu-id="d348a-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="d348a-106">Return Type</span></span>|<span data-ttu-id="d348a-107">说明</span><span class="sxs-lookup"><span data-stu-id="d348a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d348a-108">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="d348a-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="d348a-109">[mobileApp](../resources/intune_apps_mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d348a-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="d348a-110">列出 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d348a-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="d348a-111">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="d348a-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="d348a-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="d348a-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="d348a-113">读取 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d348a-113">Read properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="d348a-114">assign 操作</span><span class="sxs-lookup"><span data-stu-id="d348a-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="d348a-115">无</span><span class="sxs-lookup"><span data-stu-id="d348a-115">None</span></span>|<span data-ttu-id="d348a-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d348a-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d348a-117">属性</span><span class="sxs-lookup"><span data-stu-id="d348a-117">Properties</span></span>
|<span data-ttu-id="d348a-118">属性</span><span class="sxs-lookup"><span data-stu-id="d348a-118">Property</span></span>|<span data-ttu-id="d348a-119">类型</span><span class="sxs-lookup"><span data-stu-id="d348a-119">Type</span></span>|<span data-ttu-id="d348a-120">说明</span><span class="sxs-lookup"><span data-stu-id="d348a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d348a-121">id</span><span class="sxs-lookup"><span data-stu-id="d348a-121">id</span></span>|<span data-ttu-id="d348a-122">String</span><span class="sxs-lookup"><span data-stu-id="d348a-122">String</span></span>|<span data-ttu-id="d348a-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d348a-123">Key of the entity.</span></span>|
|<span data-ttu-id="d348a-124">displayName</span><span class="sxs-lookup"><span data-stu-id="d348a-124">displayName</span></span>|<span data-ttu-id="d348a-125">String</span><span class="sxs-lookup"><span data-stu-id="d348a-125">String</span></span>|<span data-ttu-id="d348a-126">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d348a-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="d348a-127">description</span><span class="sxs-lookup"><span data-stu-id="d348a-127">description</span></span>|<span data-ttu-id="d348a-128">String</span><span class="sxs-lookup"><span data-stu-id="d348a-128">String</span></span>|<span data-ttu-id="d348a-129">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d348a-129">The description of the app.</span></span>|
|<span data-ttu-id="d348a-130">publisher</span><span class="sxs-lookup"><span data-stu-id="d348a-130">publisher</span></span>|<span data-ttu-id="d348a-131">String</span><span class="sxs-lookup"><span data-stu-id="d348a-131">String</span></span>|<span data-ttu-id="d348a-132">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d348a-132">The publisher of the app.</span></span>|
|<span data-ttu-id="d348a-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d348a-133">largeIcon</span></span>|[<span data-ttu-id="d348a-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d348a-134">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="d348a-135">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d348a-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="d348a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d348a-136">createdDateTime</span></span>|<span data-ttu-id="d348a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d348a-137">DateTimeOffset</span></span>|<span data-ttu-id="d348a-138">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d348a-138">The date and time the app was created.</span></span>|
|<span data-ttu-id="d348a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d348a-139">lastModifiedDateTime</span></span>|<span data-ttu-id="d348a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d348a-140">DateTimeOffset</span></span>|<span data-ttu-id="d348a-141">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d348a-141">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="d348a-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d348a-142">isFeatured</span></span>|<span data-ttu-id="d348a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d348a-143">Boolean</span></span>|<span data-ttu-id="d348a-144">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="d348a-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="d348a-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d348a-145">privacyInformationUrl</span></span>|<span data-ttu-id="d348a-146">String</span><span class="sxs-lookup"><span data-stu-id="d348a-146">String</span></span>|<span data-ttu-id="d348a-147">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="d348a-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="d348a-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d348a-148">informationUrl</span></span>|<span data-ttu-id="d348a-149">String</span><span class="sxs-lookup"><span data-stu-id="d348a-149">String</span></span>|<span data-ttu-id="d348a-150">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="d348a-150">The more information Url.</span></span>|
|<span data-ttu-id="d348a-151">owner</span><span class="sxs-lookup"><span data-stu-id="d348a-151">owner</span></span>|<span data-ttu-id="d348a-152">String</span><span class="sxs-lookup"><span data-stu-id="d348a-152">String</span></span>|<span data-ttu-id="d348a-153">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d348a-153">The owner of the app.</span></span>|
|<span data-ttu-id="d348a-154">developer</span><span class="sxs-lookup"><span data-stu-id="d348a-154">developer</span></span>|<span data-ttu-id="d348a-155">String</span><span class="sxs-lookup"><span data-stu-id="d348a-155">String</span></span>|<span data-ttu-id="d348a-156">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d348a-156">The developer of the app.</span></span>|
|<span data-ttu-id="d348a-157">notes</span><span class="sxs-lookup"><span data-stu-id="d348a-157">notes</span></span>|<span data-ttu-id="d348a-158">String</span><span class="sxs-lookup"><span data-stu-id="d348a-158">String</span></span>|<span data-ttu-id="d348a-159">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d348a-159">Notes for the app.</span></span>|
|<span data-ttu-id="d348a-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="d348a-160">publishingState</span></span>|[<span data-ttu-id="d348a-161">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d348a-161">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="d348a-162">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d348a-162">The publishing state for the app.</span></span> <span data-ttu-id="d348a-163">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d348a-163">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d348a-164">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d348a-164">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d348a-165">Relationships</span><span class="sxs-lookup"><span data-stu-id="d348a-165">Relationships</span></span>
|<span data-ttu-id="d348a-166">关系</span><span class="sxs-lookup"><span data-stu-id="d348a-166">Relationship</span></span>|<span data-ttu-id="d348a-167">类型</span><span class="sxs-lookup"><span data-stu-id="d348a-167">Type</span></span>|<span data-ttu-id="d348a-168">说明</span><span class="sxs-lookup"><span data-stu-id="d348a-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d348a-169">categories</span><span class="sxs-lookup"><span data-stu-id="d348a-169">categories</span></span>|<span data-ttu-id="d348a-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d348a-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="d348a-171">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="d348a-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="d348a-172">assignments</span><span class="sxs-lookup"><span data-stu-id="d348a-172">assignments</span></span>|<span data-ttu-id="d348a-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d348a-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="d348a-174">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="d348a-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d348a-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d348a-175">JSON Representation</span></span>
<span data-ttu-id="d348a-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d348a-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```



