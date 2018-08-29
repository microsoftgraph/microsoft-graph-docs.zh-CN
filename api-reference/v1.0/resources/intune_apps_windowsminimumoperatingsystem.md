# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="368be-101">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="368be-101">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="368be-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="368be-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="368be-103">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="368be-103">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="368be-104">属性</span><span class="sxs-lookup"><span data-stu-id="368be-104">Properties</span></span>
|<span data-ttu-id="368be-105">属性</span><span class="sxs-lookup"><span data-stu-id="368be-105">Property</span></span>|<span data-ttu-id="368be-106">类型</span><span class="sxs-lookup"><span data-stu-id="368be-106">Type</span></span>|<span data-ttu-id="368be-107">说明</span><span class="sxs-lookup"><span data-stu-id="368be-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="368be-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="368be-108">v8_0</span></span>|<span data-ttu-id="368be-109">布尔值</span><span class="sxs-lookup"><span data-stu-id="368be-109">Boolean</span></span>|<span data-ttu-id="368be-110">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="368be-110">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="368be-111">v8_1</span><span class="sxs-lookup"><span data-stu-id="368be-111">v8_1</span></span>|<span data-ttu-id="368be-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="368be-112">Boolean</span></span>|<span data-ttu-id="368be-113">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="368be-113">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="368be-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="368be-114">v10_0</span></span>|<span data-ttu-id="368be-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="368be-115">Boolean</span></span>|<span data-ttu-id="368be-116">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="368be-116">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="368be-117">关系</span><span class="sxs-lookup"><span data-stu-id="368be-117">Relationships</span></span>
<span data-ttu-id="368be-118">无</span><span class="sxs-lookup"><span data-stu-id="368be-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="368be-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="368be-119">JSON Representation</span></span>
<span data-ttu-id="368be-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="368be-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



