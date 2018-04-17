# <a name="devicemanagement-resource-type"></a><span data-ttu-id="3897f-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="3897f-101">deviceManagement resource type</span></span>

> <span data-ttu-id="3897f-102">**重要说明：**Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3897f-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3897f-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3897f-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3897f-104">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3897f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3897f-105">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="3897f-105">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="3897f-106">方法</span><span class="sxs-lookup"><span data-stu-id="3897f-106">Methods</span></span>
|<span data-ttu-id="3897f-107">方法</span><span class="sxs-lookup"><span data-stu-id="3897f-107">Method</span></span>|<span data-ttu-id="3897f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3897f-108">Return Type</span></span>|<span data-ttu-id="3897f-109">说明</span><span class="sxs-lookup"><span data-stu-id="3897f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3897f-110">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3897f-110">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="3897f-111">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3897f-111">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="3897f-112">读取 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3897f-112">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="3897f-113">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3897f-113">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="3897f-114">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3897f-114">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="3897f-115">更新 [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3897f-115">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3897f-116">属性</span><span class="sxs-lookup"><span data-stu-id="3897f-116">Properties</span></span>
|<span data-ttu-id="3897f-117">属性</span><span class="sxs-lookup"><span data-stu-id="3897f-117">Property</span></span>|<span data-ttu-id="3897f-118">类型</span><span class="sxs-lookup"><span data-stu-id="3897f-118">Type</span></span>|<span data-ttu-id="3897f-119">说明</span><span class="sxs-lookup"><span data-stu-id="3897f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3897f-120">id</span><span class="sxs-lookup"><span data-stu-id="3897f-120">id</span></span>|<span data-ttu-id="3897f-121">String</span><span class="sxs-lookup"><span data-stu-id="3897f-121">String</span></span>|<span data-ttu-id="3897f-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3897f-122">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="3897f-123">关系</span><span class="sxs-lookup"><span data-stu-id="3897f-123">Relationships</span></span>
|<span data-ttu-id="3897f-124">关系</span><span class="sxs-lookup"><span data-stu-id="3897f-124">Relationship</span></span>|<span data-ttu-id="3897f-125">类型</span><span class="sxs-lookup"><span data-stu-id="3897f-125">Type</span></span>|<span data-ttu-id="3897f-126">说明</span><span class="sxs-lookup"><span data-stu-id="3897f-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3897f-127">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="3897f-127">troubleshootingEvents</span></span>|<span data-ttu-id="3897f-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3897f-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="3897f-129">租户的故障排除事件列表。</span><span class="sxs-lookup"><span data-stu-id="3897f-129">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3897f-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3897f-130">JSON Representation</span></span>
<span data-ttu-id="3897f-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3897f-131">Here is a JSON representation of the resource.</span></span>
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



