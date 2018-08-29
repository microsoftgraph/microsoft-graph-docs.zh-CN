# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="4dc3c-101">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="4dc3c-101">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="4dc3c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4dc3c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dc3c-103">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="4dc3c-103">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="4dc3c-104">属性</span><span class="sxs-lookup"><span data-stu-id="4dc3c-104">Properties</span></span>
|<span data-ttu-id="4dc3c-105">属性</span><span class="sxs-lookup"><span data-stu-id="4dc3c-105">Property</span></span>|<span data-ttu-id="4dc3c-106">类型</span><span class="sxs-lookup"><span data-stu-id="4dc3c-106">Type</span></span>|<span data-ttu-id="4dc3c-107">说明</span><span class="sxs-lookup"><span data-stu-id="4dc3c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc3c-108">displayName</span><span class="sxs-lookup"><span data-stu-id="4dc3c-108">displayName</span></span>|<span data-ttu-id="4dc3c-109">String</span><span class="sxs-lookup"><span data-stu-id="4dc3c-109">String</span></span>|<span data-ttu-id="4dc3c-110">显示名称</span><span class="sxs-lookup"><span data-stu-id="4dc3c-110">Display name</span></span>|
|<span data-ttu-id="4dc3c-111">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="4dc3c-111">proxiedDomains</span></span>|<span data-ttu-id="4dc3c-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4dc3c-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md) collection</span></span>|<span data-ttu-id="4dc3c-113">代理域集合</span><span class="sxs-lookup"><span data-stu-id="4dc3c-113">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dc3c-114">关系</span><span class="sxs-lookup"><span data-stu-id="4dc3c-114">Relationships</span></span>
<span data-ttu-id="4dc3c-115">无</span><span class="sxs-lookup"><span data-stu-id="4dc3c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4dc3c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4dc3c-116">JSON Representation</span></span>
<span data-ttu-id="4dc3c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dc3c-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



