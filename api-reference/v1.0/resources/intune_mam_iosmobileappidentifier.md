# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="3232a-101">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="3232a-101">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="3232a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3232a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3232a-103">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="3232a-103">The identifier for an iOS app.</span></span>

<span data-ttu-id="3232a-104">继承自 [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="3232a-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3232a-105">属性</span><span class="sxs-lookup"><span data-stu-id="3232a-105">Properties</span></span>
|<span data-ttu-id="3232a-106">属性</span><span class="sxs-lookup"><span data-stu-id="3232a-106">Property</span></span>|<span data-ttu-id="3232a-107">类型</span><span class="sxs-lookup"><span data-stu-id="3232a-107">Type</span></span>|<span data-ttu-id="3232a-108">说明</span><span class="sxs-lookup"><span data-stu-id="3232a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3232a-109">bundleId</span><span class="sxs-lookup"><span data-stu-id="3232a-109">bundleId</span></span>|<span data-ttu-id="3232a-110">String</span><span class="sxs-lookup"><span data-stu-id="3232a-110">String</span></span>|<span data-ttu-id="3232a-111">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="3232a-111">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3232a-112">关系</span><span class="sxs-lookup"><span data-stu-id="3232a-112">Relationships</span></span>
<span data-ttu-id="3232a-113">无</span><span class="sxs-lookup"><span data-stu-id="3232a-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3232a-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3232a-114">JSON Representation</span></span>
<span data-ttu-id="3232a-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3232a-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppIdentifier",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



