# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="7d3a6-101">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d3a6-101">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="7d3a6-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d3a6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d3a6-103">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="7d3a6-103">Store App for Windows information protection</span></span>

<span data-ttu-id="7d3a6-104">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3a6-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d3a6-105">属性</span><span class="sxs-lookup"><span data-stu-id="7d3a6-105">Properties</span></span>
|<span data-ttu-id="7d3a6-106">属性</span><span class="sxs-lookup"><span data-stu-id="7d3a6-106">Property</span></span>|<span data-ttu-id="7d3a6-107">类型</span><span class="sxs-lookup"><span data-stu-id="7d3a6-107">Type</span></span>|<span data-ttu-id="7d3a6-108">说明</span><span class="sxs-lookup"><span data-stu-id="7d3a6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d3a6-109">displayName</span><span class="sxs-lookup"><span data-stu-id="7d3a6-109">displayName</span></span>|<span data-ttu-id="7d3a6-110">String</span><span class="sxs-lookup"><span data-stu-id="7d3a6-110">String</span></span>|<span data-ttu-id="7d3a6-111">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="7d3a6-111">App display name.</span></span> <span data-ttu-id="7d3a6-112">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3a6-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7d3a6-113">description</span><span class="sxs-lookup"><span data-stu-id="7d3a6-113">description</span></span>|<span data-ttu-id="7d3a6-114">String</span><span class="sxs-lookup"><span data-stu-id="7d3a6-114">String</span></span>|<span data-ttu-id="7d3a6-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="7d3a6-115">The app's description.</span></span> <span data-ttu-id="7d3a6-116">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3a6-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7d3a6-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="7d3a6-117">publisherName</span></span>|<span data-ttu-id="7d3a6-118">String</span><span class="sxs-lookup"><span data-stu-id="7d3a6-118">String</span></span>|<span data-ttu-id="7d3a6-119">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="7d3a6-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7d3a6-120">productName</span><span class="sxs-lookup"><span data-stu-id="7d3a6-120">productName</span></span>|<span data-ttu-id="7d3a6-121">String</span><span class="sxs-lookup"><span data-stu-id="7d3a6-121">String</span></span>|<span data-ttu-id="7d3a6-122">产品名称。</span><span class="sxs-lookup"><span data-stu-id="7d3a6-122">The product name.</span></span> <span data-ttu-id="7d3a6-123">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3a6-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7d3a6-124">denied</span><span class="sxs-lookup"><span data-stu-id="7d3a6-124">Permission denied</span></span>|<span data-ttu-id="7d3a6-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="7d3a6-125">Boolean</span></span>|<span data-ttu-id="7d3a6-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="7d3a6-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="7d3a6-127">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3a6-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d3a6-128">关系</span><span class="sxs-lookup"><span data-stu-id="7d3a6-128">Relationships</span></span>
<span data-ttu-id="7d3a6-129">无</span><span class="sxs-lookup"><span data-stu-id="7d3a6-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d3a6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d3a6-130">JSON Representation</span></span>
<span data-ttu-id="7d3a6-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d3a6-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



