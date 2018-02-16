# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="c6c99-101">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6c99-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="c6c99-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6c99-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6c99-103">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="c6c99-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="c6c99-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6c99-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6c99-105">属性</span><span class="sxs-lookup"><span data-stu-id="c6c99-105">Properties</span></span>
|<span data-ttu-id="c6c99-106">属性</span><span class="sxs-lookup"><span data-stu-id="c6c99-106">Property</span></span>|<span data-ttu-id="c6c99-107">类型</span><span class="sxs-lookup"><span data-stu-id="c6c99-107">Type</span></span>|<span data-ttu-id="c6c99-108">说明</span><span class="sxs-lookup"><span data-stu-id="c6c99-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6c99-109">displayName</span><span class="sxs-lookup"><span data-stu-id="c6c99-109">displayName</span></span>|<span data-ttu-id="c6c99-110">String</span><span class="sxs-lookup"><span data-stu-id="c6c99-110">String</span></span>|<span data-ttu-id="c6c99-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c6c99-111">Display Name</span></span> <span data-ttu-id="c6c99-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6c99-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c6c99-113">description</span><span class="sxs-lookup"><span data-stu-id="c6c99-113">description</span></span>|<span data-ttu-id="c6c99-114">String</span><span class="sxs-lookup"><span data-stu-id="c6c99-114">String</span></span>|<span data-ttu-id="c6c99-115">说明。</span><span class="sxs-lookup"><span data-stu-id="c6c99-115">Description.</span></span> <span data-ttu-id="c6c99-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6c99-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c6c99-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="c6c99-117">omaUri</span></span>|<span data-ttu-id="c6c99-118">String</span><span class="sxs-lookup"><span data-stu-id="c6c99-118">String</span></span>|<span data-ttu-id="c6c99-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="c6c99-119">OMA.</span></span> <span data-ttu-id="c6c99-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6c99-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c6c99-121">fileName</span><span class="sxs-lookup"><span data-stu-id="c6c99-121">fileName</span></span>|<span data-ttu-id="c6c99-122">String</span><span class="sxs-lookup"><span data-stu-id="c6c99-122">String</span></span>|<span data-ttu-id="c6c99-123">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="c6c99-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="c6c99-124">\*.crt ) 相关联的文件名。</span><span class="sxs-lookup"><span data-stu-id="c6c99-124">\*.crt ).</span></span>|
|<span data-ttu-id="c6c99-125">值</span><span class="sxs-lookup"><span data-stu-id="c6c99-125">value</span></span>|<span data-ttu-id="c6c99-126">String</span><span class="sxs-lookup"><span data-stu-id="c6c99-126">String</span></span>|<span data-ttu-id="c6c99-127">值。</span><span class="sxs-lookup"><span data-stu-id="c6c99-127">Value.</span></span> <span data-ttu-id="c6c99-128">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="c6c99-128">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6c99-129">关系</span><span class="sxs-lookup"><span data-stu-id="c6c99-129">Relationships</span></span>
<span data-ttu-id="c6c99-130">无</span><span class="sxs-lookup"><span data-stu-id="c6c99-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6c99-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6c99-131">JSON Representation</span></span>
<span data-ttu-id="c6c99-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6c99-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
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



