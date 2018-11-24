# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="1adf0-101">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="1adf0-101">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="1adf0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1adf0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1adf0-103">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="1adf0-103">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="1adf0-104">属性</span><span class="sxs-lookup"><span data-stu-id="1adf0-104">Properties</span></span>
|<span data-ttu-id="1adf0-105">属性</span><span class="sxs-lookup"><span data-stu-id="1adf0-105">Property</span></span>|<span data-ttu-id="1adf0-106">类型</span><span class="sxs-lookup"><span data-stu-id="1adf0-106">Type</span></span>|<span data-ttu-id="1adf0-107">说明</span><span class="sxs-lookup"><span data-stu-id="1adf0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1adf0-108">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="1adf0-108">appConfigKey</span></span>|<span data-ttu-id="1adf0-109">String</span><span class="sxs-lookup"><span data-stu-id="1adf0-109">String</span></span>|<span data-ttu-id="1adf0-110">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="1adf0-110">app configuration key.</span></span>|
|<span data-ttu-id="1adf0-111">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="1adf0-111">appConfigKeyType</span></span>|[<span data-ttu-id="1adf0-112">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="1adf0-112">mdmAppConfigKeyType</span></span>](../resources/intune_apps_mdmappconfigkeytype.md)|<span data-ttu-id="1adf0-113">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="1adf0-113">app configuration key type.</span></span> <span data-ttu-id="1adf0-114">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="1adf0-114">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="1adf0-115">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="1adf0-115">appConfigKeyValue</span></span>|<span data-ttu-id="1adf0-116">String</span><span class="sxs-lookup"><span data-stu-id="1adf0-116">String</span></span>|<span data-ttu-id="1adf0-117">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="1adf0-117">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1adf0-118">关系</span><span class="sxs-lookup"><span data-stu-id="1adf0-118">Relationships</span></span>
<span data-ttu-id="1adf0-119">无</span><span class="sxs-lookup"><span data-stu-id="1adf0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1adf0-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1adf0-120">JSON Representation</span></span>
<span data-ttu-id="1adf0-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1adf0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



