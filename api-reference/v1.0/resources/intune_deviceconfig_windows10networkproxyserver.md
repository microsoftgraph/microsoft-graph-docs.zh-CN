# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="abc99-101">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="abc99-101">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="abc99-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="abc99-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abc99-103">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="abc99-103">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="abc99-104">属性</span><span class="sxs-lookup"><span data-stu-id="abc99-104">Properties</span></span>
|<span data-ttu-id="abc99-105">属性</span><span class="sxs-lookup"><span data-stu-id="abc99-105">Property</span></span>|<span data-ttu-id="abc99-106">类型</span><span class="sxs-lookup"><span data-stu-id="abc99-106">Type</span></span>|<span data-ttu-id="abc99-107">说明</span><span class="sxs-lookup"><span data-stu-id="abc99-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abc99-108">address</span><span class="sxs-lookup"><span data-stu-id="abc99-108">address</span></span>|<span data-ttu-id="abc99-109">String</span><span class="sxs-lookup"><span data-stu-id="abc99-109">String</span></span>|<span data-ttu-id="abc99-110">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="abc99-110">Address to the proxy server.</span></span> <span data-ttu-id="abc99-111">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="abc99-111">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="abc99-112">exceptions</span><span class="sxs-lookup"><span data-stu-id="abc99-112">exceptions</span></span>|<span data-ttu-id="abc99-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="abc99-113">String collection</span></span>|<span data-ttu-id="abc99-114">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="abc99-114">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="abc99-115">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="abc99-115">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="abc99-116">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="abc99-116">useForLocalAddresses</span></span>|<span data-ttu-id="abc99-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="abc99-117">Boolean</span></span>|<span data-ttu-id="abc99-118">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="abc99-118">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abc99-119">关系</span><span class="sxs-lookup"><span data-stu-id="abc99-119">Relationships</span></span>
<span data-ttu-id="abc99-120">无</span><span class="sxs-lookup"><span data-stu-id="abc99-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abc99-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abc99-121">JSON Representation</span></span>
<span data-ttu-id="abc99-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abc99-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



