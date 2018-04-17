# <a name="devicemanagement-resource-type"></a><span data-ttu-id="8614b-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="8614b-101">deviceManagement resource type</span></span>

> <span data-ttu-id="8614b-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8614b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8614b-103">deviceManagement 资源表示已在 Intune 中预留的租户的集合设备标识，以及可能分配给支持预注册配置的设备标识的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="8614b-103">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="8614b-104">方法</span><span class="sxs-lookup"><span data-stu-id="8614b-104">Methods</span></span>
|<span data-ttu-id="8614b-105">方法</span><span class="sxs-lookup"><span data-stu-id="8614b-105">Method</span></span>|<span data-ttu-id="8614b-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="8614b-106">Return Type</span></span>|<span data-ttu-id="8614b-107">说明</span><span class="sxs-lookup"><span data-stu-id="8614b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8614b-108">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8614b-108">Get deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_get.md)|[<span data-ttu-id="8614b-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8614b-109">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="8614b-110">读取 [deviceManagement](../resources/intune_enrollment_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8614b-110">Read properties and relationships of the [deviceManagement](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="8614b-111">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8614b-111">Update deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_update.md)|[<span data-ttu-id="8614b-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8614b-112">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="8614b-113">更新 [deviceManagement](../resources/intune_enrollment_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8614b-113">Update the properties of a [deviceManagement](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8614b-114">属性</span><span class="sxs-lookup"><span data-stu-id="8614b-114">Properties</span></span>
|<span data-ttu-id="8614b-115">属性</span><span class="sxs-lookup"><span data-stu-id="8614b-115">Property</span></span>|<span data-ttu-id="8614b-116">类型</span><span class="sxs-lookup"><span data-stu-id="8614b-116">Type</span></span>|<span data-ttu-id="8614b-117">说明</span><span class="sxs-lookup"><span data-stu-id="8614b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8614b-118">id</span><span class="sxs-lookup"><span data-stu-id="8614b-118">id</span></span>|<span data-ttu-id="8614b-119">String</span><span class="sxs-lookup"><span data-stu-id="8614b-119">String</span></span>|<span data-ttu-id="8614b-120">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="8614b-120">The GUID for the object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8614b-121">关系</span><span class="sxs-lookup"><span data-stu-id="8614b-121">Relationships</span></span>
|<span data-ttu-id="8614b-122">关系</span><span class="sxs-lookup"><span data-stu-id="8614b-122">Relationship</span></span>|<span data-ttu-id="8614b-123">类型</span><span class="sxs-lookup"><span data-stu-id="8614b-123">Type</span></span>|<span data-ttu-id="8614b-124">说明</span><span class="sxs-lookup"><span data-stu-id="8614b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8614b-125">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="8614b-125">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="8614b-126">[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8614b-126">[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="8614b-127">导入的 Windows AutoPilot 设备的集合。</span><span class="sxs-lookup"><span data-stu-id="8614b-127">Collection of imported Windows autopilot devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8614b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8614b-128">JSON Representation</span></span>
<span data-ttu-id="8614b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8614b-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



