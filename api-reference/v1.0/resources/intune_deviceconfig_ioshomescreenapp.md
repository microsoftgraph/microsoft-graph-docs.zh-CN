# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="51115-101">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="51115-101">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="51115-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="51115-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51115-103">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="51115-103">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="51115-104">继承自 [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="51115-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="51115-105">属性</span><span class="sxs-lookup"><span data-stu-id="51115-105">Properties</span></span>
|<span data-ttu-id="51115-106">属性</span><span class="sxs-lookup"><span data-stu-id="51115-106">Property</span></span>|<span data-ttu-id="51115-107">类型</span><span class="sxs-lookup"><span data-stu-id="51115-107">Type</span></span>|<span data-ttu-id="51115-108">说明</span><span class="sxs-lookup"><span data-stu-id="51115-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51115-109">displayName</span><span class="sxs-lookup"><span data-stu-id="51115-109">displayName</span></span>|<span data-ttu-id="51115-110">String</span><span class="sxs-lookup"><span data-stu-id="51115-110">String</span></span>|<span data-ttu-id="51115-111">继承自 [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="51115-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="51115-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="51115-112">bundleID</span></span>|<span data-ttu-id="51115-113">String</span><span class="sxs-lookup"><span data-stu-id="51115-113">String</span></span>|<span data-ttu-id="51115-114">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="51115-114">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="51115-115">关系</span><span class="sxs-lookup"><span data-stu-id="51115-115">Relationships</span></span>
<span data-ttu-id="51115-116">无</span><span class="sxs-lookup"><span data-stu-id="51115-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51115-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51115-117">JSON Representation</span></span>
<span data-ttu-id="51115-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51115-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.iosHomeScreenItem",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



