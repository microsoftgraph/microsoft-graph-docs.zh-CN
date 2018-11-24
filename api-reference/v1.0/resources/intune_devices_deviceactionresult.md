# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="20301-101">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="20301-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="20301-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="20301-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20301-103">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="20301-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="20301-104">属性</span><span class="sxs-lookup"><span data-stu-id="20301-104">Properties</span></span>
|<span data-ttu-id="20301-105">属性</span><span class="sxs-lookup"><span data-stu-id="20301-105">Property</span></span>|<span data-ttu-id="20301-106">类型</span><span class="sxs-lookup"><span data-stu-id="20301-106">Type</span></span>|<span data-ttu-id="20301-107">说明</span><span class="sxs-lookup"><span data-stu-id="20301-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20301-108">actionName</span><span class="sxs-lookup"><span data-stu-id="20301-108">actionName</span></span>|<span data-ttu-id="20301-109">String</span><span class="sxs-lookup"><span data-stu-id="20301-109">String</span></span>|<span data-ttu-id="20301-110">操作名</span><span class="sxs-lookup"><span data-stu-id="20301-110">Action name</span></span>|
|<span data-ttu-id="20301-111">actionState</span><span class="sxs-lookup"><span data-stu-id="20301-111">actionState</span></span>|[<span data-ttu-id="20301-112">actionState</span><span class="sxs-lookup"><span data-stu-id="20301-112">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="20301-113">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="20301-113">State of the action.</span></span> <span data-ttu-id="20301-114">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="20301-114">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="20301-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="20301-115">startDateTime</span></span>|<span data-ttu-id="20301-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20301-116">DateTimeOffset</span></span>|<span data-ttu-id="20301-117">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="20301-117">Time the action was initiated</span></span>|
|<span data-ttu-id="20301-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="20301-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="20301-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20301-119">DateTimeOffset</span></span>|<span data-ttu-id="20301-120">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="20301-120">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="20301-121">关系</span><span class="sxs-lookup"><span data-stu-id="20301-121">Relationships</span></span>
<span data-ttu-id="20301-122">无</span><span class="sxs-lookup"><span data-stu-id="20301-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20301-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20301-123">JSON Representation</span></span>
<span data-ttu-id="20301-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20301-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



