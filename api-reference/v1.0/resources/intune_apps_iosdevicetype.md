# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="1fe65-101">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fe65-101">iosDeviceType resource type</span></span>

> <span data-ttu-id="1fe65-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1fe65-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fe65-103">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="1fe65-103">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="1fe65-104">属性</span><span class="sxs-lookup"><span data-stu-id="1fe65-104">Properties</span></span>
|<span data-ttu-id="1fe65-105">属性</span><span class="sxs-lookup"><span data-stu-id="1fe65-105">Property</span></span>|<span data-ttu-id="1fe65-106">类型</span><span class="sxs-lookup"><span data-stu-id="1fe65-106">Type</span></span>|<span data-ttu-id="1fe65-107">说明</span><span class="sxs-lookup"><span data-stu-id="1fe65-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fe65-108">iPad</span><span class="sxs-lookup"><span data-stu-id="1fe65-108">iPad</span></span>|<span data-ttu-id="1fe65-109">布尔值</span><span class="sxs-lookup"><span data-stu-id="1fe65-109">Boolean</span></span>|<span data-ttu-id="1fe65-110">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="1fe65-110">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="1fe65-111">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="1fe65-111">iPhoneAndIPod</span></span>|<span data-ttu-id="1fe65-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="1fe65-112">Boolean</span></span>|<span data-ttu-id="1fe65-113">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="1fe65-113">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fe65-114">关系</span><span class="sxs-lookup"><span data-stu-id="1fe65-114">Relationships</span></span>
<span data-ttu-id="1fe65-115">无</span><span class="sxs-lookup"><span data-stu-id="1fe65-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1fe65-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fe65-116">JSON Representation</span></span>
<span data-ttu-id="1fe65-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fe65-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```








