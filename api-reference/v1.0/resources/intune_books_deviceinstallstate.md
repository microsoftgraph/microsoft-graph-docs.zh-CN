# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="715ac-101">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="715ac-101">deviceInstallState resource type</span></span>

> <span data-ttu-id="715ac-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="715ac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="715ac-103">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="715ac-103">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="715ac-104">方法</span><span class="sxs-lookup"><span data-stu-id="715ac-104">Methods</span></span>
|<span data-ttu-id="715ac-105">方法</span><span class="sxs-lookup"><span data-stu-id="715ac-105">Method</span></span>|<span data-ttu-id="715ac-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="715ac-106">Return Type</span></span>|<span data-ttu-id="715ac-107">说明</span><span class="sxs-lookup"><span data-stu-id="715ac-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="715ac-108">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="715ac-108">List deviceInstallStates</span></span>](../api/intune_books_deviceinstallstate_list.md)|<span data-ttu-id="715ac-109">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="715ac-109">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="715ac-110">列出 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="715ac-110">List properties and relationships of the [deviceInstallState](../resources/intune_books_deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="715ac-111">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="715ac-111">Get deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_get.md)|[<span data-ttu-id="715ac-112">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="715ac-112">deviceInstallState</span></span>](../resources/intune_books_deviceinstallstate.md)|<span data-ttu-id="715ac-113">读取 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="715ac-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_books_deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="715ac-114">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="715ac-114">Create deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_create.md)|[<span data-ttu-id="715ac-115">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="715ac-115">deviceInstallState</span></span>](../resources/intune_books_deviceinstallstate.md)|<span data-ttu-id="715ac-116">创建新的 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="715ac-116">Create a new [plannerBucket](../resources/intune_books_deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="715ac-117">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="715ac-117">Delete deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_delete.md)|<span data-ttu-id="715ac-118">无</span><span class="sxs-lookup"><span data-stu-id="715ac-118">None</span></span>|<span data-ttu-id="715ac-119">删除 [deviceInstallState](../resources/intune_books_deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="715ac-119">Deletes a [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="715ac-120">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="715ac-120">Update deviceInstallState</span></span>](../api/intune_books_deviceinstallstate_update.md)|[<span data-ttu-id="715ac-121">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="715ac-121">deviceInstallState</span></span>](../resources/intune_books_deviceinstallstate.md)|<span data-ttu-id="715ac-122">更新 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="715ac-122">Update the properties of a [calendar](../resources/intune_books_deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="715ac-123">属性</span><span class="sxs-lookup"><span data-stu-id="715ac-123">Properties</span></span>
|<span data-ttu-id="715ac-124">属性</span><span class="sxs-lookup"><span data-stu-id="715ac-124">Property</span></span>|<span data-ttu-id="715ac-125">类型</span><span class="sxs-lookup"><span data-stu-id="715ac-125">Type</span></span>|<span data-ttu-id="715ac-126">说明</span><span class="sxs-lookup"><span data-stu-id="715ac-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="715ac-127">id</span><span class="sxs-lookup"><span data-stu-id="715ac-127">id</span></span>|<span data-ttu-id="715ac-128">String</span><span class="sxs-lookup"><span data-stu-id="715ac-128">String</span></span>|<span data-ttu-id="715ac-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="715ac-129">Key of the setting.</span></span>|
|<span data-ttu-id="715ac-130">deviceName</span><span class="sxs-lookup"><span data-stu-id="715ac-130">deviceName</span></span>|<span data-ttu-id="715ac-131">String</span><span class="sxs-lookup"><span data-stu-id="715ac-131">String</span></span>|<span data-ttu-id="715ac-132">设备名称。</span><span class="sxs-lookup"><span data-stu-id="715ac-132">Device name.</span></span>|
|<span data-ttu-id="715ac-133">deviceId</span><span class="sxs-lookup"><span data-stu-id="715ac-133">deviceId</span></span>|<span data-ttu-id="715ac-134">String</span><span class="sxs-lookup"><span data-stu-id="715ac-134">String</span></span>|<span data-ttu-id="715ac-135">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="715ac-135">Device Id.</span></span>|
|<span data-ttu-id="715ac-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="715ac-136">lastSyncDateTime</span></span>|<span data-ttu-id="715ac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="715ac-137">DateTimeOffset</span></span>|<span data-ttu-id="715ac-138">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="715ac-138">Last sync date and time.</span></span>|
|<span data-ttu-id="715ac-139">installState</span><span class="sxs-lookup"><span data-stu-id="715ac-139">installState</span></span>|<span data-ttu-id="715ac-140">String</span><span class="sxs-lookup"><span data-stu-id="715ac-140">String</span></span>|<span data-ttu-id="715ac-141">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="715ac-141">The install state of the eBook.</span></span> <span data-ttu-id="715ac-142">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="715ac-142">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="715ac-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="715ac-143">errorCode</span></span>|<span data-ttu-id="715ac-144">String</span><span class="sxs-lookup"><span data-stu-id="715ac-144">String</span></span>|<span data-ttu-id="715ac-145">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="715ac-145">The error code for install failures.</span></span>|
|<span data-ttu-id="715ac-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="715ac-146">osVersion</span></span>|<span data-ttu-id="715ac-147">String</span><span class="sxs-lookup"><span data-stu-id="715ac-147">String</span></span>|<span data-ttu-id="715ac-148">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="715ac-148">OS Version.</span></span>|
|<span data-ttu-id="715ac-149">osDescription</span><span class="sxs-lookup"><span data-stu-id="715ac-149">osDescription</span></span>|<span data-ttu-id="715ac-150">String</span><span class="sxs-lookup"><span data-stu-id="715ac-150">String</span></span>|<span data-ttu-id="715ac-151">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="715ac-151">OS Description.</span></span>|
|<span data-ttu-id="715ac-152">userName</span><span class="sxs-lookup"><span data-stu-id="715ac-152">UserName</span></span>|<span data-ttu-id="715ac-153">String</span><span class="sxs-lookup"><span data-stu-id="715ac-153">String</span></span>|<span data-ttu-id="715ac-154">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="715ac-154">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="715ac-155">关系</span><span class="sxs-lookup"><span data-stu-id="715ac-155">Relationships</span></span>
<span data-ttu-id="715ac-156">无</span><span class="sxs-lookup"><span data-stu-id="715ac-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="715ac-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="715ac-157">JSON Representation</span></span>
<span data-ttu-id="715ac-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="715ac-158">Here is a JSON representation of the resource.</span></span>
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



