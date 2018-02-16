# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="5f45f-101">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f45f-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="5f45f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5f45f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f45f-103">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="5f45f-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="5f45f-104">属性</span><span class="sxs-lookup"><span data-stu-id="5f45f-104">Properties</span></span>
|<span data-ttu-id="5f45f-105">属性</span><span class="sxs-lookup"><span data-stu-id="5f45f-105">Property</span></span>|<span data-ttu-id="5f45f-106">类型</span><span class="sxs-lookup"><span data-stu-id="5f45f-106">Type</span></span>|<span data-ttu-id="5f45f-107">说明</span><span class="sxs-lookup"><span data-stu-id="5f45f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f45f-108">actionName</span><span class="sxs-lookup"><span data-stu-id="5f45f-108">ActionName</span></span>|<span data-ttu-id="5f45f-109">String</span><span class="sxs-lookup"><span data-stu-id="5f45f-109">String</span></span>|<span data-ttu-id="5f45f-110">操作名</span><span class="sxs-lookup"><span data-stu-id="5f45f-110">Action name</span></span>|
|<span data-ttu-id="5f45f-111">actionState</span><span class="sxs-lookup"><span data-stu-id="5f45f-111">actionState</span></span>|<span data-ttu-id="5f45f-112">String</span><span class="sxs-lookup"><span data-stu-id="5f45f-112">String</span></span>|<span data-ttu-id="5f45f-113">操作状态的可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="5f45f-113">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5f45f-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5f45f-114">startDateTime</span></span>|<span data-ttu-id="5f45f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f45f-115">DateTimeOffset</span></span>|<span data-ttu-id="5f45f-116">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="5f45f-116">Time the action was initiated</span></span>|
|<span data-ttu-id="5f45f-117">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f45f-117">lastUpdatedDateTime</span></span>|<span data-ttu-id="5f45f-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f45f-118">DateTimeOffset</span></span>|<span data-ttu-id="5f45f-119">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="5f45f-119">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f45f-120">关系</span><span class="sxs-lookup"><span data-stu-id="5f45f-120">Relationships</span></span>
<span data-ttu-id="5f45f-121">无</span><span class="sxs-lookup"><span data-stu-id="5f45f-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f45f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f45f-122">JSON Representation</span></span>
<span data-ttu-id="5f45f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f45f-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



