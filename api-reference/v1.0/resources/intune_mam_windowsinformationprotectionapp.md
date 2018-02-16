# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="8150a-101">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="8150a-101">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="8150a-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8150a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8150a-103">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="8150a-103">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="8150a-104">属性</span><span class="sxs-lookup"><span data-stu-id="8150a-104">Properties</span></span>
|<span data-ttu-id="8150a-105">属性</span><span class="sxs-lookup"><span data-stu-id="8150a-105">Property</span></span>|<span data-ttu-id="8150a-106">类型</span><span class="sxs-lookup"><span data-stu-id="8150a-106">Type</span></span>|<span data-ttu-id="8150a-107">说明</span><span class="sxs-lookup"><span data-stu-id="8150a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8150a-108">displayName</span><span class="sxs-lookup"><span data-stu-id="8150a-108">displayName</span></span>|<span data-ttu-id="8150a-109">String</span><span class="sxs-lookup"><span data-stu-id="8150a-109">String</span></span>|<span data-ttu-id="8150a-110">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="8150a-110">App display name.</span></span>|
|<span data-ttu-id="8150a-111">description</span><span class="sxs-lookup"><span data-stu-id="8150a-111">description</span></span>|<span data-ttu-id="8150a-112">String</span><span class="sxs-lookup"><span data-stu-id="8150a-112">String</span></span>|<span data-ttu-id="8150a-113">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="8150a-113">The app's description.</span></span>|
|<span data-ttu-id="8150a-114">publisherName</span><span class="sxs-lookup"><span data-stu-id="8150a-114">publisherName</span></span>|<span data-ttu-id="8150a-115">String</span><span class="sxs-lookup"><span data-stu-id="8150a-115">String</span></span>|<span data-ttu-id="8150a-116">发布者名称</span><span class="sxs-lookup"><span data-stu-id="8150a-116">The publisher name</span></span>|
|<span data-ttu-id="8150a-117">productName</span><span class="sxs-lookup"><span data-stu-id="8150a-117">productName</span></span>|<span data-ttu-id="8150a-118">String</span><span class="sxs-lookup"><span data-stu-id="8150a-118">String</span></span>|<span data-ttu-id="8150a-119">产品名称。</span><span class="sxs-lookup"><span data-stu-id="8150a-119">The product name.</span></span>|
|<span data-ttu-id="8150a-120">denied</span><span class="sxs-lookup"><span data-stu-id="8150a-120">Permission denied</span></span>|<span data-ttu-id="8150a-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="8150a-121">Boolean</span></span>|<span data-ttu-id="8150a-122">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="8150a-122">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8150a-123">关系</span><span class="sxs-lookup"><span data-stu-id="8150a-123">Relationships</span></span>
<span data-ttu-id="8150a-124">无</span><span class="sxs-lookup"><span data-stu-id="8150a-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8150a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8150a-125">JSON Representation</span></span>
<span data-ttu-id="8150a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8150a-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



