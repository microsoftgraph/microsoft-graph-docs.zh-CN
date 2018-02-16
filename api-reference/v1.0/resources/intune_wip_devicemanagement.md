# <a name="devicemanagement-resource-type"></a><span data-ttu-id="22fc6-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="22fc6-101">deviceManagement resource type</span></span>

> <span data-ttu-id="22fc6-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="22fc6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22fc6-103">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="22fc6-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="22fc6-104">方法</span><span class="sxs-lookup"><span data-stu-id="22fc6-104">Methods</span></span>
|<span data-ttu-id="22fc6-105">方法</span><span class="sxs-lookup"><span data-stu-id="22fc6-105">Method</span></span>|<span data-ttu-id="22fc6-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="22fc6-106">Return Type</span></span>|<span data-ttu-id="22fc6-107">说明</span><span class="sxs-lookup"><span data-stu-id="22fc6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22fc6-108">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="22fc6-108">Get deviceManagement</span></span>](../api/intune_wip_devicemanagement_get.md)|[<span data-ttu-id="22fc6-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="22fc6-109">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="22fc6-110">读取 [deviceManagement](../resources/intune_wip_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22fc6-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_wip_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="22fc6-111">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="22fc6-111">Update deviceManagement</span></span>](../api/intune_wip_devicemanagement_update.md)|[<span data-ttu-id="22fc6-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="22fc6-112">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="22fc6-113">更新 [deviceManagement](../resources/intune_wip_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="22fc6-113">Update the properties of a [calendar](../resources/intune_wip_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22fc6-114">属性</span><span class="sxs-lookup"><span data-stu-id="22fc6-114">Properties</span></span>
|<span data-ttu-id="22fc6-115">属性</span><span class="sxs-lookup"><span data-stu-id="22fc6-115">Property</span></span>|<span data-ttu-id="22fc6-116">类型</span><span class="sxs-lookup"><span data-stu-id="22fc6-116">Type</span></span>|<span data-ttu-id="22fc6-117">说明</span><span class="sxs-lookup"><span data-stu-id="22fc6-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22fc6-118">id</span><span class="sxs-lookup"><span data-stu-id="22fc6-118">id</span></span>|<span data-ttu-id="22fc6-119">String</span><span class="sxs-lookup"><span data-stu-id="22fc6-119">String</span></span>|<span data-ttu-id="22fc6-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="22fc6-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="22fc6-121">关系</span><span class="sxs-lookup"><span data-stu-id="22fc6-121">Relationships</span></span>
|<span data-ttu-id="22fc6-122">关系</span><span class="sxs-lookup"><span data-stu-id="22fc6-122">Relationship</span></span>|<span data-ttu-id="22fc6-123">类型</span><span class="sxs-lookup"><span data-stu-id="22fc6-123">Type</span></span>|<span data-ttu-id="22fc6-124">说明</span><span class="sxs-lookup"><span data-stu-id="22fc6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22fc6-125">windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="22fc6-125">windowsInformationProtectionAppLearningSummaries</span></span>|<span data-ttu-id="22fc6-126">[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22fc6-126">[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) collection</span></span>|<span data-ttu-id="22fc6-127">Windows 信息保护应用学习摘要。</span><span class="sxs-lookup"><span data-stu-id="22fc6-127">The windows information protection app learning summaries.</span></span>|
|<span data-ttu-id="22fc6-128">windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="22fc6-128">windowsInformationProtectionNetworkLearningSummaries</span></span>|<span data-ttu-id="22fc6-129">[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22fc6-129">[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) collection</span></span>|<span data-ttu-id="22fc6-130">Windows 信息保护网络学习摘要。</span><span class="sxs-lookup"><span data-stu-id="22fc6-130">The windows information protection network learning summaries.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22fc6-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22fc6-131">JSON Representation</span></span>
<span data-ttu-id="22fc6-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22fc6-132">Here is a JSON representation of the resource.</span></span>
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



