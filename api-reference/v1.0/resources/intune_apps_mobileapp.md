# <a name="mobileapp-resource-type"></a><span data-ttu-id="73023-101">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="73023-101">mobileApp resource type</span></span>

> <span data-ttu-id="73023-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73023-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73023-103">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="73023-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="73023-104">方法</span><span class="sxs-lookup"><span data-stu-id="73023-104">Methods</span></span>
|<span data-ttu-id="73023-105">方法</span><span class="sxs-lookup"><span data-stu-id="73023-105">Method</span></span>|<span data-ttu-id="73023-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="73023-106">Return Type</span></span>|<span data-ttu-id="73023-107">说明</span><span class="sxs-lookup"><span data-stu-id="73023-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73023-108">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="73023-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="73023-109">[mobileApp](../resources/intune_apps_mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73023-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="73023-110">列出 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73023-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="73023-111">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="73023-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="73023-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="73023-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="73023-113">读取 [mobileApp](../resources/intune_apps_mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73023-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="73023-114">assign 操作</span><span class="sxs-lookup"><span data-stu-id="73023-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="73023-115">无</span><span class="sxs-lookup"><span data-stu-id="73023-115">None</span></span>|<span data-ttu-id="73023-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="73023-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="73023-117">属性</span><span class="sxs-lookup"><span data-stu-id="73023-117">Properties</span></span>
|<span data-ttu-id="73023-118">属性</span><span class="sxs-lookup"><span data-stu-id="73023-118">Property</span></span>|<span data-ttu-id="73023-119">类型</span><span class="sxs-lookup"><span data-stu-id="73023-119">Type</span></span>|<span data-ttu-id="73023-120">说明</span><span class="sxs-lookup"><span data-stu-id="73023-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73023-121">id</span><span class="sxs-lookup"><span data-stu-id="73023-121">id</span></span>|<span data-ttu-id="73023-122">String</span><span class="sxs-lookup"><span data-stu-id="73023-122">String</span></span>|<span data-ttu-id="73023-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73023-123">Key of the setting.</span></span>|
|<span data-ttu-id="73023-124">displayName</span><span class="sxs-lookup"><span data-stu-id="73023-124">displayName</span></span>|<span data-ttu-id="73023-125">String</span><span class="sxs-lookup"><span data-stu-id="73023-125">String</span></span>|<span data-ttu-id="73023-126">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="73023-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="73023-127">description</span><span class="sxs-lookup"><span data-stu-id="73023-127">description</span></span>|<span data-ttu-id="73023-128">String</span><span class="sxs-lookup"><span data-stu-id="73023-128">String</span></span>|<span data-ttu-id="73023-129">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="73023-129">The description of the app.</span></span>|
|<span data-ttu-id="73023-130">publisher</span><span class="sxs-lookup"><span data-stu-id="73023-130">Publisher</span></span>|<span data-ttu-id="73023-131">String</span><span class="sxs-lookup"><span data-stu-id="73023-131">String</span></span>|<span data-ttu-id="73023-132">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="73023-132">The name of the app.</span></span>|
|<span data-ttu-id="73023-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73023-133">largeIcon</span></span>|[<span data-ttu-id="73023-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73023-134">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="73023-135">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="73023-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="73023-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73023-136">createdDateTime</span></span>|<span data-ttu-id="73023-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73023-137">DateTimeOffset</span></span>|<span data-ttu-id="73023-138">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73023-138">The date and time when the page was created.</span></span>|
|<span data-ttu-id="73023-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73023-139">lastModifiedDateTime</span></span>|<span data-ttu-id="73023-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73023-140">DateTimeOffset</span></span>|<span data-ttu-id="73023-141">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73023-141">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="73023-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73023-142">isFeatured</span></span>|<span data-ttu-id="73023-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="73023-143">Boolean</span></span>|<span data-ttu-id="73023-144">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="73023-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="73023-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73023-145">privacyInformationUrl</span></span>|<span data-ttu-id="73023-146">String</span><span class="sxs-lookup"><span data-stu-id="73023-146">String</span></span>|<span data-ttu-id="73023-147">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="73023-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="73023-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73023-148">informationUrl</span></span>|<span data-ttu-id="73023-149">String</span><span class="sxs-lookup"><span data-stu-id="73023-149">String</span></span>|<span data-ttu-id="73023-150">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="73023-150">The more information Url.</span></span>|
|<span data-ttu-id="73023-151">owner</span><span class="sxs-lookup"><span data-stu-id="73023-151">owner</span></span>|<span data-ttu-id="73023-152">String</span><span class="sxs-lookup"><span data-stu-id="73023-152">String</span></span>|<span data-ttu-id="73023-153">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="73023-153">The owner of the timesheet.</span></span>|
|<span data-ttu-id="73023-154">developer</span><span class="sxs-lookup"><span data-stu-id="73023-154">developer</span></span>|<span data-ttu-id="73023-155">String</span><span class="sxs-lookup"><span data-stu-id="73023-155">String</span></span>|<span data-ttu-id="73023-156">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="73023-156">The name of the app.</span></span>|
|<span data-ttu-id="73023-157">notes</span><span class="sxs-lookup"><span data-stu-id="73023-157">notes</span></span>|<span data-ttu-id="73023-158">String</span><span class="sxs-lookup"><span data-stu-id="73023-158">String</span></span>|<span data-ttu-id="73023-159">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="73023-159">Notes for the app.</span></span>|
|<span data-ttu-id="73023-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="73023-160">publishingState</span></span>|<span data-ttu-id="73023-161">String</span><span class="sxs-lookup"><span data-stu-id="73023-161">String</span></span>|<span data-ttu-id="73023-162">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="73023-162">The publishing state for the app.</span></span> <span data-ttu-id="73023-163">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="73023-163">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73023-164">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="73023-164">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73023-165">Relationships</span><span class="sxs-lookup"><span data-stu-id="73023-165">Relationships</span></span>
|<span data-ttu-id="73023-166">关系</span><span class="sxs-lookup"><span data-stu-id="73023-166">Relationship</span></span>|<span data-ttu-id="73023-167">类型</span><span class="sxs-lookup"><span data-stu-id="73023-167">Type</span></span>|<span data-ttu-id="73023-168">说明</span><span class="sxs-lookup"><span data-stu-id="73023-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73023-169">categories</span><span class="sxs-lookup"><span data-stu-id="73023-169">categories</span></span>|<span data-ttu-id="73023-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73023-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="73023-171">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="73023-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="73023-172">assignments</span><span class="sxs-lookup"><span data-stu-id="73023-172">assignments</span></span>|<span data-ttu-id="73023-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73023-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="73023-174">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="73023-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73023-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73023-175">JSON Representation</span></span>
<span data-ttu-id="73023-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73023-176">Here is a JSON representation of the resource.</span></span>
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



