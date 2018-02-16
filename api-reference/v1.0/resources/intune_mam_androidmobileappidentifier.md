# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="33cba-101">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="33cba-101">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="33cba-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="33cba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33cba-103">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="33cba-103">The identifier for an Android app.</span></span>

<span data-ttu-id="33cba-104">继承自 [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="33cba-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33cba-105">属性</span><span class="sxs-lookup"><span data-stu-id="33cba-105">Properties</span></span>
|<span data-ttu-id="33cba-106">属性</span><span class="sxs-lookup"><span data-stu-id="33cba-106">Property</span></span>|<span data-ttu-id="33cba-107">类型</span><span class="sxs-lookup"><span data-stu-id="33cba-107">Type</span></span>|<span data-ttu-id="33cba-108">说明</span><span class="sxs-lookup"><span data-stu-id="33cba-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33cba-109">packageId</span><span class="sxs-lookup"><span data-stu-id="33cba-109">PackageId</span></span>|<span data-ttu-id="33cba-110">String</span><span class="sxs-lookup"><span data-stu-id="33cba-110">String</span></span>|<span data-ttu-id="33cba-111">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="33cba-111">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33cba-112">关系</span><span class="sxs-lookup"><span data-stu-id="33cba-112">Relationships</span></span>
<span data-ttu-id="33cba-113">无</span><span class="sxs-lookup"><span data-stu-id="33cba-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33cba-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33cba-114">JSON Representation</span></span>
<span data-ttu-id="33cba-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33cba-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



