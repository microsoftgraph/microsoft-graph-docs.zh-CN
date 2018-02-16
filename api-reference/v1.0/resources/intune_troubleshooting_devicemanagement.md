# <a name="devicemanagement-resource-type"></a><span data-ttu-id="1f2d4-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f2d4-101">deviceManagement resource type</span></span>

> <span data-ttu-id="1f2d4-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f2d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f2d4-103">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="1f2d4-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="1f2d4-104">方法</span><span class="sxs-lookup"><span data-stu-id="1f2d4-104">Methods</span></span>
|<span data-ttu-id="1f2d4-105">方法</span><span class="sxs-lookup"><span data-stu-id="1f2d4-105">Method</span></span>|<span data-ttu-id="1f2d4-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="1f2d4-106">Return Type</span></span>|<span data-ttu-id="1f2d4-107">说明</span><span class="sxs-lookup"><span data-stu-id="1f2d4-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f2d4-108">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1f2d4-108">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="1f2d4-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1f2d4-109">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="1f2d4-110">读取 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f2d4-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="1f2d4-111">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1f2d4-111">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="1f2d4-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1f2d4-112">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="1f2d4-113">更新 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f2d4-113">Update the properties of a [calendar](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f2d4-114">属性</span><span class="sxs-lookup"><span data-stu-id="1f2d4-114">Properties</span></span>
|<span data-ttu-id="1f2d4-115">属性</span><span class="sxs-lookup"><span data-stu-id="1f2d4-115">Property</span></span>|<span data-ttu-id="1f2d4-116">类型</span><span class="sxs-lookup"><span data-stu-id="1f2d4-116">Type</span></span>|<span data-ttu-id="1f2d4-117">说明</span><span class="sxs-lookup"><span data-stu-id="1f2d4-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f2d4-118">id</span><span class="sxs-lookup"><span data-stu-id="1f2d4-118">id</span></span>|<span data-ttu-id="1f2d4-119">String</span><span class="sxs-lookup"><span data-stu-id="1f2d4-119">String</span></span>|<span data-ttu-id="1f2d4-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1f2d4-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f2d4-121">关系</span><span class="sxs-lookup"><span data-stu-id="1f2d4-121">Relationships</span></span>
|<span data-ttu-id="1f2d4-122">关系</span><span class="sxs-lookup"><span data-stu-id="1f2d4-122">Relationship</span></span>|<span data-ttu-id="1f2d4-123">类型</span><span class="sxs-lookup"><span data-stu-id="1f2d4-123">Type</span></span>|<span data-ttu-id="1f2d4-124">说明</span><span class="sxs-lookup"><span data-stu-id="1f2d4-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f2d4-125">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="1f2d4-125">troubleshootingEvents</span></span>|<span data-ttu-id="1f2d4-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1f2d4-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="1f2d4-127">租户的故障排除事件列表。</span><span class="sxs-lookup"><span data-stu-id="1f2d4-127">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f2d4-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f2d4-128">JSON Representation</span></span>
<span data-ttu-id="1f2d4-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f2d4-129">Here is a JSON representation of the resource.</span></span>
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



