# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="6b9cf-101">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b9cf-101">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="6b9cf-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b9cf-103">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="6b9cf-103">Desktop App for Windows information protection</span></span>

<span data-ttu-id="6b9cf-104">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b9cf-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b9cf-105">属性</span><span class="sxs-lookup"><span data-stu-id="6b9cf-105">Properties</span></span>
|<span data-ttu-id="6b9cf-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b9cf-106">Property</span></span>|<span data-ttu-id="6b9cf-107">类型</span><span class="sxs-lookup"><span data-stu-id="6b9cf-107">Type</span></span>|<span data-ttu-id="6b9cf-108">说明</span><span class="sxs-lookup"><span data-stu-id="6b9cf-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9cf-109">displayName</span><span class="sxs-lookup"><span data-stu-id="6b9cf-109">displayName</span></span>|<span data-ttu-id="6b9cf-110">String</span><span class="sxs-lookup"><span data-stu-id="6b9cf-110">String</span></span>|<span data-ttu-id="6b9cf-111">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-111">App display name.</span></span> <span data-ttu-id="6b9cf-112">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b9cf-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6b9cf-113">description</span><span class="sxs-lookup"><span data-stu-id="6b9cf-113">description</span></span>|<span data-ttu-id="6b9cf-114">String</span><span class="sxs-lookup"><span data-stu-id="6b9cf-114">String</span></span>|<span data-ttu-id="6b9cf-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-115">The app's description.</span></span> <span data-ttu-id="6b9cf-116">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b9cf-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6b9cf-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="6b9cf-117">publisherName</span></span>|<span data-ttu-id="6b9cf-118">String</span><span class="sxs-lookup"><span data-stu-id="6b9cf-118">String</span></span>|<span data-ttu-id="6b9cf-119">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="6b9cf-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6b9cf-120">productName</span><span class="sxs-lookup"><span data-stu-id="6b9cf-120">productName</span></span>|<span data-ttu-id="6b9cf-121">String</span><span class="sxs-lookup"><span data-stu-id="6b9cf-121">String</span></span>|<span data-ttu-id="6b9cf-122">产品名称。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-122">The product name.</span></span> <span data-ttu-id="6b9cf-123">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b9cf-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6b9cf-124">denied</span><span class="sxs-lookup"><span data-stu-id="6b9cf-124">Permission denied</span></span>|<span data-ttu-id="6b9cf-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b9cf-125">Boolean</span></span>|<span data-ttu-id="6b9cf-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="6b9cf-127">继承自 [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b9cf-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6b9cf-128">binaryName</span><span class="sxs-lookup"><span data-stu-id="6b9cf-128">binaryName</span></span>|<span data-ttu-id="6b9cf-129">String</span><span class="sxs-lookup"><span data-stu-id="6b9cf-129">String</span></span>|<span data-ttu-id="6b9cf-130">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-130">The binary name.</span></span>|
|<span data-ttu-id="6b9cf-131">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="6b9cf-131">binaryVersionLow</span></span>|<span data-ttu-id="6b9cf-132">String</span><span class="sxs-lookup"><span data-stu-id="6b9cf-132">String</span></span>|<span data-ttu-id="6b9cf-133">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-133">The lower binary version.</span></span>|
|<span data-ttu-id="6b9cf-134">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="6b9cf-134">binaryVersionHigh</span></span>|<span data-ttu-id="6b9cf-135">String</span><span class="sxs-lookup"><span data-stu-id="6b9cf-135">String</span></span>|<span data-ttu-id="6b9cf-136">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-136">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b9cf-137">关系</span><span class="sxs-lookup"><span data-stu-id="6b9cf-137">Relationships</span></span>
<span data-ttu-id="6b9cf-138">无</span><span class="sxs-lookup"><span data-stu-id="6b9cf-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b9cf-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b9cf-139">JSON Representation</span></span>
<span data-ttu-id="6b9cf-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b9cf-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



