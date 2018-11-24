# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="5b327-101">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b327-101">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="5b327-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b327-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b327-103">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="5b327-103">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="5b327-104">属性</span><span class="sxs-lookup"><span data-stu-id="5b327-104">Properties</span></span>
|<span data-ttu-id="5b327-105">属性</span><span class="sxs-lookup"><span data-stu-id="5b327-105">Property</span></span>|<span data-ttu-id="5b327-106">类型</span><span class="sxs-lookup"><span data-stu-id="5b327-106">Type</span></span>|<span data-ttu-id="5b327-107">说明</span><span class="sxs-lookup"><span data-stu-id="5b327-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b327-108">managedApps</span><span class="sxs-lookup"><span data-stu-id="5b327-108">managedApps</span></span>|<span data-ttu-id="5b327-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b327-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="5b327-110">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="5b327-110">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="5b327-111">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5b327-111">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5b327-112">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="5b327-112">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="5b327-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b327-113">Boolean</span></span>|<span data-ttu-id="5b327-114">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="5b327-114">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="5b327-115">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="5b327-115">cellularDataBlocked</span></span>|<span data-ttu-id="5b327-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b327-116">Boolean</span></span>|<span data-ttu-id="5b327-117">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="5b327-117">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b327-118">关系</span><span class="sxs-lookup"><span data-stu-id="5b327-118">Relationships</span></span>
<span data-ttu-id="5b327-119">无</span><span class="sxs-lookup"><span data-stu-id="5b327-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b327-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b327-120">JSON Representation</span></span>
<span data-ttu-id="5b327-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b327-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



