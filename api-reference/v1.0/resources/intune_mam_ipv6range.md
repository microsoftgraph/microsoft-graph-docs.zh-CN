# <a name="ipv6range-resource-type"></a><span data-ttu-id="bfb45-101">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfb45-101">iPv6Range resource type</span></span>

> <span data-ttu-id="bfb45-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bfb45-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfb45-103">IPV6 范围</span><span class="sxs-lookup"><span data-stu-id="bfb45-103">IP V6 range</span></span>

<span data-ttu-id="bfb45-104">继承自 [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="bfb45-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bfb45-105">属性</span><span class="sxs-lookup"><span data-stu-id="bfb45-105">Properties</span></span>
|<span data-ttu-id="bfb45-106">属性</span><span class="sxs-lookup"><span data-stu-id="bfb45-106">Property</span></span>|<span data-ttu-id="bfb45-107">类型</span><span class="sxs-lookup"><span data-stu-id="bfb45-107">Type</span></span>|<span data-ttu-id="bfb45-108">说明</span><span class="sxs-lookup"><span data-stu-id="bfb45-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfb45-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="bfb45-109">lowerAddress</span></span>|<span data-ttu-id="bfb45-110">String</span><span class="sxs-lookup"><span data-stu-id="bfb45-110">String</span></span>|<span data-ttu-id="bfb45-111">IP 地址下限</span><span class="sxs-lookup"><span data-stu-id="bfb45-111">Lower IP Address</span></span>|
|<span data-ttu-id="bfb45-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="bfb45-112">upperAddress</span></span>|<span data-ttu-id="bfb45-113">String</span><span class="sxs-lookup"><span data-stu-id="bfb45-113">String</span></span>|<span data-ttu-id="bfb45-114">IP 地址上限</span><span class="sxs-lookup"><span data-stu-id="bfb45-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfb45-115">关系</span><span class="sxs-lookup"><span data-stu-id="bfb45-115">Relationships</span></span>
<span data-ttu-id="bfb45-116">无</span><span class="sxs-lookup"><span data-stu-id="bfb45-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bfb45-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfb45-117">JSON Representation</span></span>
<span data-ttu-id="bfb45-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfb45-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



