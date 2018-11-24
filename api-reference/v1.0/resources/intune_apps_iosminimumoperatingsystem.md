# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="ff19b-101">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff19b-101">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="ff19b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ff19b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff19b-103">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="ff19b-103">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="ff19b-104">属性</span><span class="sxs-lookup"><span data-stu-id="ff19b-104">Properties</span></span>
|<span data-ttu-id="ff19b-105">属性</span><span class="sxs-lookup"><span data-stu-id="ff19b-105">Property</span></span>|<span data-ttu-id="ff19b-106">类型</span><span class="sxs-lookup"><span data-stu-id="ff19b-106">Type</span></span>|<span data-ttu-id="ff19b-107">说明</span><span class="sxs-lookup"><span data-stu-id="ff19b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff19b-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="ff19b-108">v8_0</span></span>|<span data-ttu-id="ff19b-109">布尔值</span><span class="sxs-lookup"><span data-stu-id="ff19b-109">Boolean</span></span>|<span data-ttu-id="ff19b-110">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ff19b-110">Version 8.0 or later.</span></span>|
|<span data-ttu-id="ff19b-111">v9_0</span><span class="sxs-lookup"><span data-stu-id="ff19b-111">v9_0</span></span>|<span data-ttu-id="ff19b-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="ff19b-112">Boolean</span></span>|<span data-ttu-id="ff19b-113">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ff19b-113">Version 9.0 or later.</span></span>|
|<span data-ttu-id="ff19b-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="ff19b-114">v10_0</span></span>|<span data-ttu-id="ff19b-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="ff19b-115">Boolean</span></span>|<span data-ttu-id="ff19b-116">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ff19b-116">Version 10.0 or later.</span></span>|
|<span data-ttu-id="ff19b-117">v11_0</span><span class="sxs-lookup"><span data-stu-id="ff19b-117">v11_0</span></span>|<span data-ttu-id="ff19b-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="ff19b-118">Boolean</span></span>|<span data-ttu-id="ff19b-119">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ff19b-119">Version 11.0 or later.</span></span>|
|<span data-ttu-id="ff19b-120">v12_0</span><span class="sxs-lookup"><span data-stu-id="ff19b-120">v12_0</span></span>|<span data-ttu-id="ff19b-121">布尔</span><span class="sxs-lookup"><span data-stu-id="ff19b-121">Boolean</span></span>|<span data-ttu-id="ff19b-122">12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ff19b-122">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff19b-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="ff19b-123">Relationships</span></span>
<span data-ttu-id="ff19b-124">无</span><span class="sxs-lookup"><span data-stu-id="ff19b-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff19b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff19b-125">JSON Representation</span></span>
<span data-ttu-id="ff19b-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff19b-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



