# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="67981-101">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="67981-101">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="67981-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="67981-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67981-103">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="67981-103">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="67981-104">属性</span><span class="sxs-lookup"><span data-stu-id="67981-104">Properties</span></span>
|<span data-ttu-id="67981-105">属性</span><span class="sxs-lookup"><span data-stu-id="67981-105">Property</span></span>|<span data-ttu-id="67981-106">类型</span><span class="sxs-lookup"><span data-stu-id="67981-106">Type</span></span>|<span data-ttu-id="67981-107">说明</span><span class="sxs-lookup"><span data-stu-id="67981-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67981-108">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="67981-108">appConfigKey</span></span>|<span data-ttu-id="67981-109">String</span><span class="sxs-lookup"><span data-stu-id="67981-109">String</span></span>|<span data-ttu-id="67981-110">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="67981-110">app configuration key.</span></span>|
|<span data-ttu-id="67981-111">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="67981-111">appConfigKeyType</span></span>|<span data-ttu-id="67981-112">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="67981-112">mdmAppConfigKeyType</span></span>|<span data-ttu-id="67981-113">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="67981-113">app configuration key type.</span></span> <span data-ttu-id="67981-114">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="67981-114">The possible values are `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`, , , , , , , or .</span></span>|
|<span data-ttu-id="67981-115">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="67981-115">appConfigKeyValue</span></span>|<span data-ttu-id="67981-116">String</span><span class="sxs-lookup"><span data-stu-id="67981-116">String</span></span>|<span data-ttu-id="67981-117">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="67981-117">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67981-118">关系</span><span class="sxs-lookup"><span data-stu-id="67981-118">Relationships</span></span>
<span data-ttu-id="67981-119">无</span><span class="sxs-lookup"><span data-stu-id="67981-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67981-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67981-120">JSON Representation</span></span>
<span data-ttu-id="67981-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67981-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



