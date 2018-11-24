# <a name="proxieddomain-resource-type"></a><span data-ttu-id="868a2-101">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="868a2-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="868a2-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="868a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="868a2-103">代理域</span><span class="sxs-lookup"><span data-stu-id="868a2-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="868a2-104">属性</span><span class="sxs-lookup"><span data-stu-id="868a2-104">Properties</span></span>
|<span data-ttu-id="868a2-105">属性</span><span class="sxs-lookup"><span data-stu-id="868a2-105">Property</span></span>|<span data-ttu-id="868a2-106">类型</span><span class="sxs-lookup"><span data-stu-id="868a2-106">Type</span></span>|<span data-ttu-id="868a2-107">说明</span><span class="sxs-lookup"><span data-stu-id="868a2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="868a2-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="868a2-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="868a2-109">String</span><span class="sxs-lookup"><span data-stu-id="868a2-109">String</span></span>|<span data-ttu-id="868a2-110">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="868a2-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="868a2-111">代理</span><span class="sxs-lookup"><span data-stu-id="868a2-111">proxy</span></span>|<span data-ttu-id="868a2-112">String</span><span class="sxs-lookup"><span data-stu-id="868a2-112">String</span></span>|<span data-ttu-id="868a2-113">代理 IP</span><span class="sxs-lookup"><span data-stu-id="868a2-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="868a2-114">关系</span><span class="sxs-lookup"><span data-stu-id="868a2-114">Relationships</span></span>
<span data-ttu-id="868a2-115">无</span><span class="sxs-lookup"><span data-stu-id="868a2-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="868a2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="868a2-116">JSON Representation</span></span>
<span data-ttu-id="868a2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="868a2-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



