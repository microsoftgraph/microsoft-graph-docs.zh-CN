# <a name="rgbcolor-resource-type"></a><span data-ttu-id="7ff10-101">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ff10-101">rgbColor resource type</span></span>

> <span data-ttu-id="7ff10-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ff10-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ff10-103">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="7ff10-103">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="7ff10-104">属性</span><span class="sxs-lookup"><span data-stu-id="7ff10-104">Properties</span></span>
|<span data-ttu-id="7ff10-105">属性</span><span class="sxs-lookup"><span data-stu-id="7ff10-105">Property</span></span>|<span data-ttu-id="7ff10-106">类型</span><span class="sxs-lookup"><span data-stu-id="7ff10-106">Type</span></span>|<span data-ttu-id="7ff10-107">说明</span><span class="sxs-lookup"><span data-stu-id="7ff10-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff10-108">r</span><span class="sxs-lookup"><span data-stu-id="7ff10-108">r</span></span>|<span data-ttu-id="7ff10-109">字节</span><span class="sxs-lookup"><span data-stu-id="7ff10-109">Byte</span></span>|<span data-ttu-id="7ff10-110">红色值</span><span class="sxs-lookup"><span data-stu-id="7ff10-110">Red value</span></span>|
|<span data-ttu-id="7ff10-111">g</span><span class="sxs-lookup"><span data-stu-id="7ff10-111">g</span></span>|<span data-ttu-id="7ff10-112">字节</span><span class="sxs-lookup"><span data-stu-id="7ff10-112">Byte</span></span>|<span data-ttu-id="7ff10-113">绿色值</span><span class="sxs-lookup"><span data-stu-id="7ff10-113">Green value</span></span>|
|<span data-ttu-id="7ff10-114">b</span><span class="sxs-lookup"><span data-stu-id="7ff10-114">b</span></span>|<span data-ttu-id="7ff10-115">字节</span><span class="sxs-lookup"><span data-stu-id="7ff10-115">Byte</span></span>|<span data-ttu-id="7ff10-116">蓝色值</span><span class="sxs-lookup"><span data-stu-id="7ff10-116">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ff10-117">关系</span><span class="sxs-lookup"><span data-stu-id="7ff10-117">Relationships</span></span>
<span data-ttu-id="7ff10-118">无</span><span class="sxs-lookup"><span data-stu-id="7ff10-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ff10-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ff10-119">JSON Representation</span></span>
<span data-ttu-id="7ff10-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ff10-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```



