# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="f2bff-101">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2bff-101">deviceInstallState resource type</span></span>

> <span data-ttu-id="f2bff-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f2bff-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2bff-103">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="f2bff-103">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="f2bff-104">方法</span><span class="sxs-lookup"><span data-stu-id="f2bff-104">Methods</span></span>
|<span data-ttu-id="f2bff-105">方法</span><span class="sxs-lookup"><span data-stu-id="f2bff-105">Method</span></span>|<span data-ttu-id="f2bff-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2bff-106">Return Type</span></span>|<span data-ttu-id="f2bff-107">说明</span><span class="sxs-lookup"><span data-stu-id="f2bff-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2bff-108">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="f2bff-108">List deviceInstallStates</span></span>](../api/intune_books_deviceinstallstate_list.md)|<span data-ttu-id="f2bff-109">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2bff-109">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="f2bff-110">列出 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2bff-110">List properties and relationships of the [deviceInstallState](../resources/intune_books_deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="f2bff-111">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f2bff-111">Get deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_get.md)|[<span data-ttu-id="f2bff-112">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f2bff-112">deviceInstallState</span></span>](../resources/intune_books_deviceinstallstate.md)|<span data-ttu-id="f2bff-113">读取 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2bff-113">Read properties and relationships of the [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="f2bff-114">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f2bff-114">Create deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_create.md)|[<span data-ttu-id="f2bff-115">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f2bff-115">deviceInstallState</span></span>](../resources/intune_books_deviceinstallstate.md)|<span data-ttu-id="f2bff-116">创建新的 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2bff-116">Create a new [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="f2bff-117">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f2bff-117">Delete deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_delete.md)|<span data-ttu-id="f2bff-118">无</span><span class="sxs-lookup"><span data-stu-id="f2bff-118">None</span></span>|<span data-ttu-id="f2bff-119">删除 [deviceInstallState](../resources/intune_books_deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="f2bff-119">Deletes a [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="f2bff-120">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f2bff-120">Update deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_update.md)|[<span data-ttu-id="f2bff-121">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f2bff-121">deviceInstallState</span></span>](../resources/intune_books_deviceinstallstate.md)|<span data-ttu-id="f2bff-122">更新 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2bff-122">Update the properties of a [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2bff-123">属性</span><span class="sxs-lookup"><span data-stu-id="f2bff-123">Properties</span></span>
|<span data-ttu-id="f2bff-124">属性</span><span class="sxs-lookup"><span data-stu-id="f2bff-124">Property</span></span>|<span data-ttu-id="f2bff-125">类型</span><span class="sxs-lookup"><span data-stu-id="f2bff-125">Type</span></span>|<span data-ttu-id="f2bff-126">说明</span><span class="sxs-lookup"><span data-stu-id="f2bff-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2bff-127">id</span><span class="sxs-lookup"><span data-stu-id="f2bff-127">id</span></span>|<span data-ttu-id="f2bff-128">String</span><span class="sxs-lookup"><span data-stu-id="f2bff-128">String</span></span>|<span data-ttu-id="f2bff-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f2bff-129">Key of the entity.</span></span>|
|<span data-ttu-id="f2bff-130">deviceName</span><span class="sxs-lookup"><span data-stu-id="f2bff-130">deviceName</span></span>|<span data-ttu-id="f2bff-131">String</span><span class="sxs-lookup"><span data-stu-id="f2bff-131">String</span></span>|<span data-ttu-id="f2bff-132">设备名称。</span><span class="sxs-lookup"><span data-stu-id="f2bff-132">Device name.</span></span>|
|<span data-ttu-id="f2bff-133">deviceId</span><span class="sxs-lookup"><span data-stu-id="f2bff-133">deviceId</span></span>|<span data-ttu-id="f2bff-134">String</span><span class="sxs-lookup"><span data-stu-id="f2bff-134">String</span></span>|<span data-ttu-id="f2bff-135">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="f2bff-135">Device Id.</span></span>|
|<span data-ttu-id="f2bff-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f2bff-136">lastSyncDateTime</span></span>|<span data-ttu-id="f2bff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2bff-137">DateTimeOffset</span></span>|<span data-ttu-id="f2bff-138">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f2bff-138">Last sync date and time.</span></span>|
|<span data-ttu-id="f2bff-139">installState</span><span class="sxs-lookup"><span data-stu-id="f2bff-139">installState</span></span>|[<span data-ttu-id="f2bff-140">installState</span><span class="sxs-lookup"><span data-stu-id="f2bff-140">installState</span></span>](../resources/intune_books_installstate.md)|<span data-ttu-id="f2bff-141">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="f2bff-141">The install state of the eBook.</span></span> <span data-ttu-id="f2bff-142">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="f2bff-142">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="f2bff-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="f2bff-143">errorCode</span></span>|<span data-ttu-id="f2bff-144">String</span><span class="sxs-lookup"><span data-stu-id="f2bff-144">String</span></span>|<span data-ttu-id="f2bff-145">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="f2bff-145">The error code for install failures.</span></span>|
|<span data-ttu-id="f2bff-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="f2bff-146">osVersion</span></span>|<span data-ttu-id="f2bff-147">String</span><span class="sxs-lookup"><span data-stu-id="f2bff-147">String</span></span>|<span data-ttu-id="f2bff-148">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f2bff-148">OS Version.</span></span>|
|<span data-ttu-id="f2bff-149">osDescription</span><span class="sxs-lookup"><span data-stu-id="f2bff-149">osDescription</span></span>|<span data-ttu-id="f2bff-150">String</span><span class="sxs-lookup"><span data-stu-id="f2bff-150">String</span></span>|<span data-ttu-id="f2bff-151">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="f2bff-151">OS Description.</span></span>|
|<span data-ttu-id="f2bff-152">userName</span><span class="sxs-lookup"><span data-stu-id="f2bff-152">userName</span></span>|<span data-ttu-id="f2bff-153">String</span><span class="sxs-lookup"><span data-stu-id="f2bff-153">String</span></span>|<span data-ttu-id="f2bff-154">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="f2bff-154">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2bff-155">关系</span><span class="sxs-lookup"><span data-stu-id="f2bff-155">Relationships</span></span>
<span data-ttu-id="f2bff-156">无</span><span class="sxs-lookup"><span data-stu-id="f2bff-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2bff-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2bff-157">JSON Representation</span></span>
<span data-ttu-id="f2bff-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2bff-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



