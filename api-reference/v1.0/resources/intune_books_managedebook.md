# <a name="managedebook-resource-type"></a><span data-ttu-id="f1611-101">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1611-101">managedEBook resource type</span></span>

> <span data-ttu-id="f1611-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1611-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1611-103">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="f1611-103">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="f1611-104">方法</span><span class="sxs-lookup"><span data-stu-id="f1611-104">Methods</span></span>
|<span data-ttu-id="f1611-105">方法</span><span class="sxs-lookup"><span data-stu-id="f1611-105">Method</span></span>|<span data-ttu-id="f1611-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1611-106">Return Type</span></span>|<span data-ttu-id="f1611-107">说明</span><span class="sxs-lookup"><span data-stu-id="f1611-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f1611-108">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="f1611-108">List managedEBooks</span></span>](../api/intune_books_managedebook_list.md)|<span data-ttu-id="f1611-109">[managedEBook](../resources/intune_books_managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1611-109">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="f1611-110">列出 [managedEBook](../resources/intune_books_managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1611-110">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>|
|[<span data-ttu-id="f1611-111">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="f1611-111">Get managedEBook</span></span>](../api/intune_books_managedebook_get.md)|[<span data-ttu-id="f1611-112">managedEBook</span><span class="sxs-lookup"><span data-stu-id="f1611-112">managedEBook</span></span>](../resources/intune_books_managedebook.md)|<span data-ttu-id="f1611-113">读取 [managedEBook](../resources/intune_books_managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1611-113">Read properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) object.</span></span>|
|[<span data-ttu-id="f1611-114">assign 操作</span><span class="sxs-lookup"><span data-stu-id="f1611-114">assign action</span></span>](../api/intune_books_managedebook_assign.md)|<span data-ttu-id="f1611-115">无</span><span class="sxs-lookup"><span data-stu-id="f1611-115">None</span></span>|<span data-ttu-id="f1611-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f1611-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f1611-117">属性</span><span class="sxs-lookup"><span data-stu-id="f1611-117">Properties</span></span>
|<span data-ttu-id="f1611-118">属性</span><span class="sxs-lookup"><span data-stu-id="f1611-118">Property</span></span>|<span data-ttu-id="f1611-119">类型</span><span class="sxs-lookup"><span data-stu-id="f1611-119">Type</span></span>|<span data-ttu-id="f1611-120">说明</span><span class="sxs-lookup"><span data-stu-id="f1611-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1611-121">id</span><span class="sxs-lookup"><span data-stu-id="f1611-121">id</span></span>|<span data-ttu-id="f1611-122">String</span><span class="sxs-lookup"><span data-stu-id="f1611-122">String</span></span>|<span data-ttu-id="f1611-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1611-123">Key of the entity.</span></span>|
|<span data-ttu-id="f1611-124">displayName</span><span class="sxs-lookup"><span data-stu-id="f1611-124">displayName</span></span>|<span data-ttu-id="f1611-125">String</span><span class="sxs-lookup"><span data-stu-id="f1611-125">String</span></span>|<span data-ttu-id="f1611-126">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="f1611-126">Name of the eBook.</span></span>|
|<span data-ttu-id="f1611-127">description</span><span class="sxs-lookup"><span data-stu-id="f1611-127">description</span></span>|<span data-ttu-id="f1611-128">String</span><span class="sxs-lookup"><span data-stu-id="f1611-128">String</span></span>|<span data-ttu-id="f1611-129">说明。</span><span class="sxs-lookup"><span data-stu-id="f1611-129">Description.</span></span>|
|<span data-ttu-id="f1611-130">publisher</span><span class="sxs-lookup"><span data-stu-id="f1611-130">publisher</span></span>|<span data-ttu-id="f1611-131">String</span><span class="sxs-lookup"><span data-stu-id="f1611-131">String</span></span>|<span data-ttu-id="f1611-132">发布者。</span><span class="sxs-lookup"><span data-stu-id="f1611-132">Publisher.</span></span>|
|<span data-ttu-id="f1611-133">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1611-133">publishedDateTime</span></span>|<span data-ttu-id="f1611-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1611-134">DateTimeOffset</span></span>|<span data-ttu-id="f1611-135">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f1611-135">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="f1611-136">largeCover</span><span class="sxs-lookup"><span data-stu-id="f1611-136">largeCover</span></span>|[<span data-ttu-id="f1611-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f1611-137">mimeContent</span></span>](../resources/intune_books_mimecontent.md)|<span data-ttu-id="f1611-138">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="f1611-138">Book cover.</span></span>|
|<span data-ttu-id="f1611-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1611-139">createdDateTime</span></span>|<span data-ttu-id="f1611-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1611-140">DateTimeOffset</span></span>|<span data-ttu-id="f1611-141">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f1611-141">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="f1611-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1611-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f1611-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1611-143">DateTimeOffset</span></span>|<span data-ttu-id="f1611-144">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f1611-144">The date and time when teh eBook was last modified.</span></span>|
|<span data-ttu-id="f1611-145">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f1611-145">informationUrl</span></span>|<span data-ttu-id="f1611-146">String</span><span class="sxs-lookup"><span data-stu-id="f1611-146">String</span></span>|<span data-ttu-id="f1611-147">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f1611-147">The more information Url.</span></span>|
|<span data-ttu-id="f1611-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f1611-148">privacyInformationUrl</span></span>|<span data-ttu-id="f1611-149">String</span><span class="sxs-lookup"><span data-stu-id="f1611-149">String</span></span>|<span data-ttu-id="f1611-150">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f1611-150">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1611-151">关系</span><span class="sxs-lookup"><span data-stu-id="f1611-151">Relationships</span></span>
|<span data-ttu-id="f1611-152">关系</span><span class="sxs-lookup"><span data-stu-id="f1611-152">Relationship</span></span>|<span data-ttu-id="f1611-153">类型</span><span class="sxs-lookup"><span data-stu-id="f1611-153">Type</span></span>|<span data-ttu-id="f1611-154">说明</span><span class="sxs-lookup"><span data-stu-id="f1611-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1611-155">assignments</span><span class="sxs-lookup"><span data-stu-id="f1611-155">assignments</span></span>|<span data-ttu-id="f1611-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1611-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="f1611-157">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="f1611-157">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="f1611-158">installSummary</span><span class="sxs-lookup"><span data-stu-id="f1611-158">installSummary</span></span>|[<span data-ttu-id="f1611-159">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f1611-159">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="f1611-160">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="f1611-160">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="f1611-161">deviceStates</span><span class="sxs-lookup"><span data-stu-id="f1611-161">deviceStates</span></span>|<span data-ttu-id="f1611-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1611-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="f1611-163">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="f1611-163">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="f1611-164">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="f1611-164">userStateSummary</span></span>|<span data-ttu-id="f1611-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1611-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="f1611-166">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="f1611-166">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1611-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1611-167">JSON Representation</span></span>
<span data-ttu-id="f1611-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1611-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



