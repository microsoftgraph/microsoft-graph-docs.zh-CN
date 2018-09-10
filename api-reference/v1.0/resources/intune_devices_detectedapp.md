# <a name="detectedapp-resource-type"></a><span data-ttu-id="513a4-101">detectedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="513a4-101">detectedApp resource type</span></span>

> <span data-ttu-id="513a4-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="513a4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="513a4-103">托管设备上安装的托管或未托管应用。</span><span class="sxs-lookup"><span data-stu-id="513a4-103">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="513a4-104">未托管应用仅出现在标记为公司所有的设备上。</span><span class="sxs-lookup"><span data-stu-id="513a4-104">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="513a4-105">方法</span><span class="sxs-lookup"><span data-stu-id="513a4-105">Methods</span></span>
|<span data-ttu-id="513a4-106">方法</span><span class="sxs-lookup"><span data-stu-id="513a4-106">Method</span></span>|<span data-ttu-id="513a4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="513a4-107">Return Type</span></span>|<span data-ttu-id="513a4-108">说明</span><span class="sxs-lookup"><span data-stu-id="513a4-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="513a4-109">List detectedApps</span><span class="sxs-lookup"><span data-stu-id="513a4-109">List detectedApps</span></span>](../api/intune_devices_detectedapp_list.md)|<span data-ttu-id="513a4-110">[detectedApp](../resources/intune_devices_detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="513a4-110">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="513a4-111">列出 [detectedApp](../resources/intune_devices_detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="513a4-111">List properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="513a4-112">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="513a4-112">Get detectedApp</span></span>](../api/intune_devices_detectedapp_get.md)|[<span data-ttu-id="513a4-113">detectedApp</span><span class="sxs-lookup"><span data-stu-id="513a4-113">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="513a4-114">读取 [detectedApp](../resources/intune_devices_detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="513a4-114">Read properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="513a4-115">Create detectedApp</span><span class="sxs-lookup"><span data-stu-id="513a4-115">Create detectedApp</span></span>](../api/intune_devices_detectedapp_create.md)|[<span data-ttu-id="513a4-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="513a4-116">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="513a4-117">创建新的 [detectedApp](../resources/intune_devices_detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="513a4-117">Create a new [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="513a4-118">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="513a4-118">Delete detectedApp</span></span>](../api/intune_devices_detectedapp_delete.md)|<span data-ttu-id="513a4-119">无</span><span class="sxs-lookup"><span data-stu-id="513a4-119">None</span></span>|<span data-ttu-id="513a4-120">删除 [detectedApp](../resources/intune_devices_detectedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="513a4-120">Deletes a [detectedApp](../resources/intune_devices_detectedapp.md).</span></span>|
|[<span data-ttu-id="513a4-121">Update detectedApp</span><span class="sxs-lookup"><span data-stu-id="513a4-121">Update detectedApp</span></span>](../api/intune_devices_detectedapp_update.md)|[<span data-ttu-id="513a4-122">detectedApp</span><span class="sxs-lookup"><span data-stu-id="513a4-122">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="513a4-123">更新 [detectedApp](../resources/intune_devices_detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="513a4-123">Update the properties of a [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="513a4-124">属性</span><span class="sxs-lookup"><span data-stu-id="513a4-124">Properties</span></span>
|<span data-ttu-id="513a4-125">属性</span><span class="sxs-lookup"><span data-stu-id="513a4-125">Property</span></span>|<span data-ttu-id="513a4-126">类型</span><span class="sxs-lookup"><span data-stu-id="513a4-126">Type</span></span>|<span data-ttu-id="513a4-127">说明</span><span class="sxs-lookup"><span data-stu-id="513a4-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="513a4-128">ID</span><span class="sxs-lookup"><span data-stu-id="513a4-128">id</span></span>|<span data-ttu-id="513a4-129">String</span><span class="sxs-lookup"><span data-stu-id="513a4-129">String</span></span>|<span data-ttu-id="513a4-130">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="513a4-130">The unique Identifier for the detected application.</span></span> <span data-ttu-id="513a4-131">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="513a4-131">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="513a4-132">只读。</span><span class="sxs-lookup"><span data-stu-id="513a4-132">Read-only.</span></span>|
|<span data-ttu-id="513a4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="513a4-133">displayName</span></span>|<span data-ttu-id="513a4-134">String</span><span class="sxs-lookup"><span data-stu-id="513a4-134">String</span></span>|<span data-ttu-id="513a4-135">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="513a4-135">Name of the discovered application.</span></span> <span data-ttu-id="513a4-136">只读</span><span class="sxs-lookup"><span data-stu-id="513a4-136">Read-only</span></span>|
|<span data-ttu-id="513a4-137">version</span><span class="sxs-lookup"><span data-stu-id="513a4-137">version</span></span>|<span data-ttu-id="513a4-138">String</span><span class="sxs-lookup"><span data-stu-id="513a4-138">String</span></span>|<span data-ttu-id="513a4-139">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="513a4-139">Version of the discovered application.</span></span> <span data-ttu-id="513a4-140">只读</span><span class="sxs-lookup"><span data-stu-id="513a4-140">Read-only</span></span>|
|<span data-ttu-id="513a4-141">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="513a4-141">sizeInByte</span></span>|<span data-ttu-id="513a4-142">Int64</span><span class="sxs-lookup"><span data-stu-id="513a4-142">Int64</span></span>|<span data-ttu-id="513a4-143">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="513a4-143">Discovered application size in bytes.</span></span> <span data-ttu-id="513a4-144">只读</span><span class="sxs-lookup"><span data-stu-id="513a4-144">Read-only</span></span>|
|<span data-ttu-id="513a4-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="513a4-145">deviceCount</span></span>|<span data-ttu-id="513a4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="513a4-146">Int32</span></span>|<span data-ttu-id="513a4-147">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="513a4-147">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="513a4-148">关系</span><span class="sxs-lookup"><span data-stu-id="513a4-148">Relationships</span></span>
|<span data-ttu-id="513a4-149">关系</span><span class="sxs-lookup"><span data-stu-id="513a4-149">Relationship</span></span>|<span data-ttu-id="513a4-150">类型</span><span class="sxs-lookup"><span data-stu-id="513a4-150">Type</span></span>|<span data-ttu-id="513a4-151">说明</span><span class="sxs-lookup"><span data-stu-id="513a4-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="513a4-152">managedDevices</span><span class="sxs-lookup"><span data-stu-id="513a4-152">managedDevices</span></span>|<span data-ttu-id="513a4-153">[managedDevice](../resources/intune_devices_manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="513a4-153">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="513a4-154">已安装发现的应用程序的设备</span><span class="sxs-lookup"><span data-stu-id="513a4-154">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="513a4-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="513a4-155">JSON Representation</span></span>
<span data-ttu-id="513a4-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="513a4-156">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```








