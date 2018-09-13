# <a name="mobileapp-resource-type"></a><span data-ttu-id="efd6c-101">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="efd6c-101">mobileApp resource type</span></span>

> <span data-ttu-id="efd6c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="efd6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efd6c-103">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="efd6c-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="efd6c-104">方法</span><span class="sxs-lookup"><span data-stu-id="efd6c-104">Methods</span></span>
|<span data-ttu-id="efd6c-105">方法</span><span class="sxs-lookup"><span data-stu-id="efd6c-105">Method</span></span>|<span data-ttu-id="efd6c-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="efd6c-106">Return Type</span></span>|<span data-ttu-id="efd6c-107">说明</span><span class="sxs-lookup"><span data-stu-id="efd6c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="efd6c-108">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="efd6c-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="efd6c-109">[mobileApp](../resources/intune_apps_mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="efd6c-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="efd6c-110">列出 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efd6c-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="efd6c-111">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="efd6c-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="efd6c-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="efd6c-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="efd6c-113">读取 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efd6c-113">Read properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="efd6c-114">assign 操作</span><span class="sxs-lookup"><span data-stu-id="efd6c-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="efd6c-115">无</span><span class="sxs-lookup"><span data-stu-id="efd6c-115">None</span></span>|<span data-ttu-id="efd6c-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="efd6c-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="efd6c-117">属性</span><span class="sxs-lookup"><span data-stu-id="efd6c-117">Properties</span></span>
|<span data-ttu-id="efd6c-118">属性</span><span class="sxs-lookup"><span data-stu-id="efd6c-118">Property</span></span>|<span data-ttu-id="efd6c-119">类型</span><span class="sxs-lookup"><span data-stu-id="efd6c-119">Type</span></span>|<span data-ttu-id="efd6c-120">说明</span><span class="sxs-lookup"><span data-stu-id="efd6c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd6c-121">ID</span><span class="sxs-lookup"><span data-stu-id="efd6c-121">id</span></span>|<span data-ttu-id="efd6c-122">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-122">String</span></span>|<span data-ttu-id="efd6c-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="efd6c-123">Key of the entity.</span></span>|
|<span data-ttu-id="efd6c-124">displayName</span><span class="sxs-lookup"><span data-stu-id="efd6c-124">displayName</span></span>|<span data-ttu-id="efd6c-125">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-125">String</span></span>|<span data-ttu-id="efd6c-126">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="efd6c-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="efd6c-127">description</span><span class="sxs-lookup"><span data-stu-id="efd6c-127">description</span></span>|<span data-ttu-id="efd6c-128">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-128">String</span></span>|<span data-ttu-id="efd6c-129">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="efd6c-129">The description of the app.</span></span>|
|<span data-ttu-id="efd6c-130">publisher</span><span class="sxs-lookup"><span data-stu-id="efd6c-130">publisher</span></span>|<span data-ttu-id="efd6c-131">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-131">String</span></span>|<span data-ttu-id="efd6c-132">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="efd6c-132">The publisher of the app.</span></span>|
|<span data-ttu-id="efd6c-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="efd6c-133">largeIcon</span></span>|[<span data-ttu-id="efd6c-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="efd6c-134">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="efd6c-135">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="efd6c-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="efd6c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efd6c-136">createdDateTime</span></span>|<span data-ttu-id="efd6c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efd6c-137">DateTimeOffset</span></span>|<span data-ttu-id="efd6c-138">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="efd6c-138">The date and time the app was created.</span></span>|
|<span data-ttu-id="efd6c-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efd6c-139">lastModifiedDateTime</span></span>|<span data-ttu-id="efd6c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efd6c-140">DateTimeOffset</span></span>|<span data-ttu-id="efd6c-141">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="efd6c-141">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="efd6c-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="efd6c-142">isFeatured</span></span>|<span data-ttu-id="efd6c-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="efd6c-143">Boolean</span></span>|<span data-ttu-id="efd6c-144">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="efd6c-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="efd6c-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="efd6c-145">privacyInformationUrl</span></span>|<span data-ttu-id="efd6c-146">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-146">String</span></span>|<span data-ttu-id="efd6c-147">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="efd6c-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="efd6c-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="efd6c-148">informationUrl</span></span>|<span data-ttu-id="efd6c-149">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-149">String</span></span>|<span data-ttu-id="efd6c-150">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="efd6c-150">The more information Url.</span></span>|
|<span data-ttu-id="efd6c-151">owner</span><span class="sxs-lookup"><span data-stu-id="efd6c-151">owner</span></span>|<span data-ttu-id="efd6c-152">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-152">String</span></span>|<span data-ttu-id="efd6c-153">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="efd6c-153">The owner of the app.</span></span>|
|<span data-ttu-id="efd6c-154">developer</span><span class="sxs-lookup"><span data-stu-id="efd6c-154">developer</span></span>|<span data-ttu-id="efd6c-155">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-155">String</span></span>|<span data-ttu-id="efd6c-156">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="efd6c-156">The developer of the app.</span></span>|
|<span data-ttu-id="efd6c-157">notes</span><span class="sxs-lookup"><span data-stu-id="efd6c-157">notes</span></span>|<span data-ttu-id="efd6c-158">字符串</span><span class="sxs-lookup"><span data-stu-id="efd6c-158">String</span></span>|<span data-ttu-id="efd6c-159">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="efd6c-159">Notes for the app.</span></span>|
|<span data-ttu-id="efd6c-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="efd6c-160">publishingState</span></span>|[<span data-ttu-id="efd6c-161">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="efd6c-161">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="efd6c-p101">应用的发布状态。除非应用已发布，否则无法分配应用。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="efd6c-p101">The publishing state for the app. The app cannot be assigned unless the app is published. The possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efd6c-165">关系</span><span class="sxs-lookup"><span data-stu-id="efd6c-165">Relationships</span></span>
|<span data-ttu-id="efd6c-166">关系</span><span class="sxs-lookup"><span data-stu-id="efd6c-166">Relationship</span></span>|<span data-ttu-id="efd6c-167">类型</span><span class="sxs-lookup"><span data-stu-id="efd6c-167">Type</span></span>|<span data-ttu-id="efd6c-168">说明</span><span class="sxs-lookup"><span data-stu-id="efd6c-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd6c-169">categories</span><span class="sxs-lookup"><span data-stu-id="efd6c-169">categories</span></span>|<span data-ttu-id="efd6c-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="efd6c-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="efd6c-171">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="efd6c-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="efd6c-172">assignments</span><span class="sxs-lookup"><span data-stu-id="efd6c-172">assignments</span></span>|<span data-ttu-id="efd6c-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="efd6c-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="efd6c-174">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="efd6c-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efd6c-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efd6c-175">JSON Representation</span></span>
<span data-ttu-id="efd6c-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efd6c-176">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}-->
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








