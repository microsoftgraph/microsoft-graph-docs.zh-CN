# <a name="manageddevice-resource-type"></a><span data-ttu-id="6041c-101">managedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="6041c-101">managedDevice resource type</span></span>

> <span data-ttu-id="6041c-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6041c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6041c-103">通过 Intune 托管或预注册的设备</span><span class="sxs-lookup"><span data-stu-id="6041c-103">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="6041c-104">方法</span><span class="sxs-lookup"><span data-stu-id="6041c-104">Methods</span></span>
|<span data-ttu-id="6041c-105">方法</span><span class="sxs-lookup"><span data-stu-id="6041c-105">Method</span></span>|<span data-ttu-id="6041c-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="6041c-106">Return Type</span></span>|<span data-ttu-id="6041c-107">说明</span><span class="sxs-lookup"><span data-stu-id="6041c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6041c-108">列出 managedDevices</span><span class="sxs-lookup"><span data-stu-id="6041c-108">List managedDevices</span></span>](../api/intune_deviceconfig_manageddevice_list.md)|<span data-ttu-id="6041c-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6041c-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) collection</span></span>|<span data-ttu-id="6041c-110">列出 [managedDevice](../resources/intune_deviceconfig_manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6041c-110">List properties and relationships of the [managedDevice](../resources/intune_deviceconfig_manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="6041c-111">获取 managedDevice</span><span class="sxs-lookup"><span data-stu-id="6041c-111">Get managedDevice</span></span>](../api/intune_deviceconfig_manageddevice_get.md)|[<span data-ttu-id="6041c-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="6041c-112">managedDevice</span></span>](../resources/intune_deviceconfig_manageddevice.md)|<span data-ttu-id="6041c-113">读取 [managedDevice](../resources/intune_deviceconfig_manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6041c-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_manageddevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6041c-114">属性</span><span class="sxs-lookup"><span data-stu-id="6041c-114">Properties</span></span>
|<span data-ttu-id="6041c-115">属性</span><span class="sxs-lookup"><span data-stu-id="6041c-115">Property</span></span>|<span data-ttu-id="6041c-116">类型</span><span class="sxs-lookup"><span data-stu-id="6041c-116">Type</span></span>|<span data-ttu-id="6041c-117">说明</span><span class="sxs-lookup"><span data-stu-id="6041c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6041c-118">id</span><span class="sxs-lookup"><span data-stu-id="6041c-118">id</span></span>|<span data-ttu-id="6041c-119">String</span><span class="sxs-lookup"><span data-stu-id="6041c-119">String</span></span>|<span data-ttu-id="6041c-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6041c-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="6041c-121">关系</span><span class="sxs-lookup"><span data-stu-id="6041c-121">Relationships</span></span>
|<span data-ttu-id="6041c-122">关系</span><span class="sxs-lookup"><span data-stu-id="6041c-122">Relationship</span></span>|<span data-ttu-id="6041c-123">类型</span><span class="sxs-lookup"><span data-stu-id="6041c-123">Type</span></span>|<span data-ttu-id="6041c-124">说明</span><span class="sxs-lookup"><span data-stu-id="6041c-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6041c-125">deviceConfigurationStates</span><span class="sxs-lookup"><span data-stu-id="6041c-125">deviceConfigurationStates</span></span>|<span data-ttu-id="6041c-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6041c-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) collection</span></span>|<span data-ttu-id="6041c-127">此设备的设备配置状态。</span><span class="sxs-lookup"><span data-stu-id="6041c-127">Device configuration states for this device.</span></span>|
|<span data-ttu-id="6041c-128">deviceCompliancePolicyStates</span><span class="sxs-lookup"><span data-stu-id="6041c-128">deviceCompliancePolicyStates</span></span>|<span data-ttu-id="6041c-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6041c-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) collection</span></span>|<span data-ttu-id="6041c-130">此设备的设备合规性策略状态。</span><span class="sxs-lookup"><span data-stu-id="6041c-130">Device compliance policy states for this device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6041c-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6041c-131">JSON Representation</span></span>
<span data-ttu-id="6041c-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6041c-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



