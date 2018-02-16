# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="d48bc-101">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d48bc-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="d48bc-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d48bc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d48bc-103">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="d48bc-103">Windows Defender last scan result</span></span>

<span data-ttu-id="d48bc-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d48bc-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d48bc-105">属性</span><span class="sxs-lookup"><span data-stu-id="d48bc-105">Properties</span></span>
|<span data-ttu-id="d48bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="d48bc-106">Property</span></span>|<span data-ttu-id="d48bc-107">类型</span><span class="sxs-lookup"><span data-stu-id="d48bc-107">Type</span></span>|<span data-ttu-id="d48bc-108">说明</span><span class="sxs-lookup"><span data-stu-id="d48bc-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d48bc-109">actionName</span><span class="sxs-lookup"><span data-stu-id="d48bc-109">ActionName</span></span>|<span data-ttu-id="d48bc-110">String</span><span class="sxs-lookup"><span data-stu-id="d48bc-110">String</span></span>|<span data-ttu-id="d48bc-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d48bc-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="d48bc-112">actionState</span><span class="sxs-lookup"><span data-stu-id="d48bc-112">actionState</span></span>|<span data-ttu-id="d48bc-113">String</span><span class="sxs-lookup"><span data-stu-id="d48bc-113">String</span></span>|<span data-ttu-id="d48bc-114">操作状态 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md) 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d48bc-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d48bc-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d48bc-115">startDateTime</span></span>|<span data-ttu-id="d48bc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d48bc-116">DateTimeOffset</span></span>|<span data-ttu-id="d48bc-117">操作启动的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d48bc-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="d48bc-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d48bc-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="d48bc-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d48bc-119">DateTimeOffset</span></span>|<span data-ttu-id="d48bc-120">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d48bc-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="d48bc-121">scanType</span><span class="sxs-lookup"><span data-stu-id="d48bc-121">scanType</span></span>|<span data-ttu-id="d48bc-122">String</span><span class="sxs-lookup"><span data-stu-id="d48bc-122">String</span></span>|<span data-ttu-id="d48bc-123">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="d48bc-123">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="d48bc-124">关系</span><span class="sxs-lookup"><span data-stu-id="d48bc-124">Relationships</span></span>
<span data-ttu-id="d48bc-125">无</span><span class="sxs-lookup"><span data-stu-id="d48bc-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d48bc-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d48bc-126">JSON Representation</span></span>
<span data-ttu-id="d48bc-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d48bc-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



