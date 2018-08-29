# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="9e412-101">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e412-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="9e412-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e412-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e412-103">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="9e412-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="9e412-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e412-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e412-105">属性</span><span class="sxs-lookup"><span data-stu-id="9e412-105">Properties</span></span>
|<span data-ttu-id="9e412-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e412-106">Property</span></span>|<span data-ttu-id="9e412-107">类型</span><span class="sxs-lookup"><span data-stu-id="9e412-107">Type</span></span>|<span data-ttu-id="9e412-108">说明</span><span class="sxs-lookup"><span data-stu-id="9e412-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e412-109">displayName</span><span class="sxs-lookup"><span data-stu-id="9e412-109">displayName</span></span>|<span data-ttu-id="9e412-110">String</span><span class="sxs-lookup"><span data-stu-id="9e412-110">String</span></span>|<span data-ttu-id="9e412-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="9e412-111">Display Name.</span></span> <span data-ttu-id="9e412-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e412-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="9e412-113">description</span><span class="sxs-lookup"><span data-stu-id="9e412-113">description</span></span>|<span data-ttu-id="9e412-114">String</span><span class="sxs-lookup"><span data-stu-id="9e412-114">String</span></span>|<span data-ttu-id="9e412-115">说明。</span><span class="sxs-lookup"><span data-stu-id="9e412-115">Description.</span></span> <span data-ttu-id="9e412-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e412-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="9e412-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="9e412-117">omaUri</span></span>|<span data-ttu-id="9e412-118">String</span><span class="sxs-lookup"><span data-stu-id="9e412-118">String</span></span>|<span data-ttu-id="9e412-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="9e412-119">OMA.</span></span> <span data-ttu-id="9e412-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e412-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="9e412-121">fileName</span><span class="sxs-lookup"><span data-stu-id="9e412-121">fileName</span></span>|<span data-ttu-id="9e412-122">String</span><span class="sxs-lookup"><span data-stu-id="9e412-122">String</span></span>|<span data-ttu-id="9e412-123">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="9e412-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="9e412-124">\*.crt ) 相关联的文件名。</span><span class="sxs-lookup"><span data-stu-id="9e412-124">\*.crt ).</span></span>|
|<span data-ttu-id="9e412-125">值</span><span class="sxs-lookup"><span data-stu-id="9e412-125">value</span></span>|<span data-ttu-id="9e412-126">String</span><span class="sxs-lookup"><span data-stu-id="9e412-126">String</span></span>|<span data-ttu-id="9e412-127">值。</span><span class="sxs-lookup"><span data-stu-id="9e412-127">Value.</span></span> <span data-ttu-id="9e412-128">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="9e412-128">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e412-129">关系</span><span class="sxs-lookup"><span data-stu-id="9e412-129">Relationships</span></span>
<span data-ttu-id="9e412-130">无</span><span class="sxs-lookup"><span data-stu-id="9e412-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e412-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e412-131">JSON Representation</span></span>
<span data-ttu-id="9e412-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e412-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



