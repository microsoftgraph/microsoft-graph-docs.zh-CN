# <a name="devicecategory-resource-type"></a><span data-ttu-id="1b1c5-101">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b1c5-101">deviceCategory resource type</span></span>

> <span data-ttu-id="1b1c5-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1b1c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b1c5-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b1c5-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="1b1c5-104">方法</span><span class="sxs-lookup"><span data-stu-id="1b1c5-104">Methods</span></span>
|<span data-ttu-id="1b1c5-105">方法</span><span class="sxs-lookup"><span data-stu-id="1b1c5-105">Method</span></span>|<span data-ttu-id="1b1c5-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b1c5-106">Return Type</span></span>|<span data-ttu-id="1b1c5-107">说明</span><span class="sxs-lookup"><span data-stu-id="1b1c5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b1c5-108">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1b1c5-108">Get deviceCategory</span></span>](../api/intune_devices_devicecategory_get.md)|[<span data-ttu-id="1b1c5-109">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1b1c5-109">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="1b1c5-110">读取 [deviceCategory](../resources/intune_devices_devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b1c5-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_devices_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="1b1c5-111">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1b1c5-111">Update deviceCategory</span></span>](../api/intune_devices_devicecategory_update.md)|[<span data-ttu-id="1b1c5-112">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1b1c5-112">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="1b1c5-113">更新 [deviceCategory](../resources/intune_devices_devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b1c5-113">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b1c5-114">属性</span><span class="sxs-lookup"><span data-stu-id="1b1c5-114">Properties</span></span>
|<span data-ttu-id="1b1c5-115">属性</span><span class="sxs-lookup"><span data-stu-id="1b1c5-115">Property</span></span>|<span data-ttu-id="1b1c5-116">类型</span><span class="sxs-lookup"><span data-stu-id="1b1c5-116">Type</span></span>|<span data-ttu-id="1b1c5-117">说明</span><span class="sxs-lookup"><span data-stu-id="1b1c5-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b1c5-118">id</span><span class="sxs-lookup"><span data-stu-id="1b1c5-118">id</span></span>|<span data-ttu-id="1b1c5-119">String</span><span class="sxs-lookup"><span data-stu-id="1b1c5-119">String</span></span>|<span data-ttu-id="1b1c5-120">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1b1c5-120">Unique identifier for the device category.</span></span> <span data-ttu-id="1b1c5-121">只读。</span><span class="sxs-lookup"><span data-stu-id="1b1c5-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b1c5-122">关系</span><span class="sxs-lookup"><span data-stu-id="1b1c5-122">Relationships</span></span>
<span data-ttu-id="1b1c5-123">无</span><span class="sxs-lookup"><span data-stu-id="1b1c5-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b1c5-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b1c5-124">JSON Representation</span></span>
<span data-ttu-id="1b1c5-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b1c5-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```



