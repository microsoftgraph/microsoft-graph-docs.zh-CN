# <a name="ipv4range-resource-type"></a><span data-ttu-id="49610-101">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="49610-101">iPv4Range resource type</span></span>

> <span data-ttu-id="49610-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49610-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49610-103">IP V4 范围</span><span class="sxs-lookup"><span data-stu-id="49610-103">IP V4 range</span></span>

<span data-ttu-id="49610-104">继承自 [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="49610-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49610-105">属性</span><span class="sxs-lookup"><span data-stu-id="49610-105">Properties</span></span>
|<span data-ttu-id="49610-106">属性</span><span class="sxs-lookup"><span data-stu-id="49610-106">Property</span></span>|<span data-ttu-id="49610-107">类型</span><span class="sxs-lookup"><span data-stu-id="49610-107">Type</span></span>|<span data-ttu-id="49610-108">说明</span><span class="sxs-lookup"><span data-stu-id="49610-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49610-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="49610-109">lowerAddress</span></span>|<span data-ttu-id="49610-110">String</span><span class="sxs-lookup"><span data-stu-id="49610-110">String</span></span>|<span data-ttu-id="49610-111">IP 地址下限</span><span class="sxs-lookup"><span data-stu-id="49610-111">Lower IP Address</span></span>|
|<span data-ttu-id="49610-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="49610-112">upperAddress</span></span>|<span data-ttu-id="49610-113">String</span><span class="sxs-lookup"><span data-stu-id="49610-113">String</span></span>|<span data-ttu-id="49610-114">IP 地址上限</span><span class="sxs-lookup"><span data-stu-id="49610-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="49610-115">关系</span><span class="sxs-lookup"><span data-stu-id="49610-115">Relationships</span></span>
<span data-ttu-id="49610-116">无</span><span class="sxs-lookup"><span data-stu-id="49610-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49610-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49610-117">JSON Representation</span></span>
<span data-ttu-id="49610-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49610-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



