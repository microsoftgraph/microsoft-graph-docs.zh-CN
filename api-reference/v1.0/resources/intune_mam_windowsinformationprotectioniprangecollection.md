# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="66fc9-101">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="66fc9-101">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="66fc9-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="66fc9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66fc9-103">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="66fc9-103">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="66fc9-104">属性</span><span class="sxs-lookup"><span data-stu-id="66fc9-104">Properties</span></span>
|<span data-ttu-id="66fc9-105">属性</span><span class="sxs-lookup"><span data-stu-id="66fc9-105">Property</span></span>|<span data-ttu-id="66fc9-106">类型</span><span class="sxs-lookup"><span data-stu-id="66fc9-106">Type</span></span>|<span data-ttu-id="66fc9-107">说明</span><span class="sxs-lookup"><span data-stu-id="66fc9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66fc9-108">displayName</span><span class="sxs-lookup"><span data-stu-id="66fc9-108">displayName</span></span>|<span data-ttu-id="66fc9-109">字符串</span><span class="sxs-lookup"><span data-stu-id="66fc9-109">String</span></span>|<span data-ttu-id="66fc9-110">显示名称</span><span class="sxs-lookup"><span data-stu-id="66fc9-110">Display name</span></span>|
|<span data-ttu-id="66fc9-111">范围</span><span class="sxs-lookup"><span data-stu-id="66fc9-111">ranges</span></span>|<span data-ttu-id="66fc9-112">[ipRange](../resources/intune_mam_iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66fc9-112">[ipRange](../resources/intune_mam_iprange.md) collection</span></span>|<span data-ttu-id="66fc9-113">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="66fc9-113">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="66fc9-114">关系</span><span class="sxs-lookup"><span data-stu-id="66fc9-114">Relationships</span></span>
<span data-ttu-id="66fc9-115">无</span><span class="sxs-lookup"><span data-stu-id="66fc9-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66fc9-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66fc9-116">JSON Representation</span></span>
<span data-ttu-id="66fc9-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66fc9-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```








