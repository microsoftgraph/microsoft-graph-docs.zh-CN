# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="e1a58-101">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1a58-101">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="e1a58-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1a58-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1a58-103">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="e1a58-103">Desktop App for Windows information protection</span></span>

<span data-ttu-id="e1a58-104">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1a58-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1a58-105">属性</span><span class="sxs-lookup"><span data-stu-id="e1a58-105">Properties</span></span>
|<span data-ttu-id="e1a58-106">属性</span><span class="sxs-lookup"><span data-stu-id="e1a58-106">Property</span></span>|<span data-ttu-id="e1a58-107">类型</span><span class="sxs-lookup"><span data-stu-id="e1a58-107">Type</span></span>|<span data-ttu-id="e1a58-108">说明</span><span class="sxs-lookup"><span data-stu-id="e1a58-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a58-109">displayName</span><span class="sxs-lookup"><span data-stu-id="e1a58-109">displayName</span></span>|<span data-ttu-id="e1a58-110">String</span><span class="sxs-lookup"><span data-stu-id="e1a58-110">String</span></span>|<span data-ttu-id="e1a58-111">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="e1a58-111">App display name.</span></span> <span data-ttu-id="e1a58-112">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1a58-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e1a58-113">description</span><span class="sxs-lookup"><span data-stu-id="e1a58-113">description</span></span>|<span data-ttu-id="e1a58-114">String</span><span class="sxs-lookup"><span data-stu-id="e1a58-114">String</span></span>|<span data-ttu-id="e1a58-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e1a58-115">The app's description.</span></span> <span data-ttu-id="e1a58-116">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1a58-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e1a58-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="e1a58-117">publisherName</span></span>|<span data-ttu-id="e1a58-118">String</span><span class="sxs-lookup"><span data-stu-id="e1a58-118">String</span></span>|<span data-ttu-id="e1a58-119">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="e1a58-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e1a58-120">productName</span><span class="sxs-lookup"><span data-stu-id="e1a58-120">productName</span></span>|<span data-ttu-id="e1a58-121">String</span><span class="sxs-lookup"><span data-stu-id="e1a58-121">String</span></span>|<span data-ttu-id="e1a58-122">产品名称。</span><span class="sxs-lookup"><span data-stu-id="e1a58-122">The product name.</span></span> <span data-ttu-id="e1a58-123">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1a58-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e1a58-124">denied</span><span class="sxs-lookup"><span data-stu-id="e1a58-124">denied</span></span>|<span data-ttu-id="e1a58-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1a58-125">Boolean</span></span>|<span data-ttu-id="e1a58-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="e1a58-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="e1a58-127">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1a58-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e1a58-128">binaryName</span><span class="sxs-lookup"><span data-stu-id="e1a58-128">binaryName</span></span>|<span data-ttu-id="e1a58-129">String</span><span class="sxs-lookup"><span data-stu-id="e1a58-129">String</span></span>|<span data-ttu-id="e1a58-130">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="e1a58-130">The binary name.</span></span>|
|<span data-ttu-id="e1a58-131">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="e1a58-131">binaryVersionLow</span></span>|<span data-ttu-id="e1a58-132">String</span><span class="sxs-lookup"><span data-stu-id="e1a58-132">String</span></span>|<span data-ttu-id="e1a58-133">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="e1a58-133">The lower binary version.</span></span>|
|<span data-ttu-id="e1a58-134">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="e1a58-134">binaryVersionHigh</span></span>|<span data-ttu-id="e1a58-135">String</span><span class="sxs-lookup"><span data-stu-id="e1a58-135">String</span></span>|<span data-ttu-id="e1a58-136">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="e1a58-136">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1a58-137">关系</span><span class="sxs-lookup"><span data-stu-id="e1a58-137">Relationships</span></span>
<span data-ttu-id="e1a58-138">无</span><span class="sxs-lookup"><span data-stu-id="e1a58-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1a58-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1a58-139">JSON Representation</span></span>
<span data-ttu-id="e1a58-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1a58-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



