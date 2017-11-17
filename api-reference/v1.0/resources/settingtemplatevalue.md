# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="2479f-101">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="2479f-101">settingTemplateValue resource type</span></span>

<span data-ttu-id="2479f-102">如果该设置未被实例化，则表示单独的模板设置定义，包括设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="2479f-102">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="2479f-103">属性</span><span class="sxs-lookup"><span data-stu-id="2479f-103">Properties</span></span>

| <span data-ttu-id="2479f-104">属性</span><span class="sxs-lookup"><span data-stu-id="2479f-104">Property</span></span> | <span data-ttu-id="2479f-105">类型</span><span class="sxs-lookup"><span data-stu-id="2479f-105">Type</span></span> | <span data-ttu-id="2479f-106">说明</span><span class="sxs-lookup"><span data-stu-id="2479f-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2479f-107">defaultValue</span><span class="sxs-lookup"><span data-stu-id="2479f-107">DefaultValue</span></span>|<span data-ttu-id="2479f-108">字符串</span><span class="sxs-lookup"><span data-stu-id="2479f-108">String</span></span>| <span data-ttu-id="2479f-109">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="2479f-109">Default value for the setting.</span></span> |
|<span data-ttu-id="2479f-110">description</span><span class="sxs-lookup"><span data-stu-id="2479f-110">description</span></span>|<span data-ttu-id="2479f-111">字符串</span><span class="sxs-lookup"><span data-stu-id="2479f-111">String</span></span>| <span data-ttu-id="2479f-112">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="2479f-112">Description of the component.</span></span> |
|<span data-ttu-id="2479f-113">name</span><span class="sxs-lookup"><span data-stu-id="2479f-113">name</span></span>|<span data-ttu-id="2479f-114">字符串</span><span class="sxs-lookup"><span data-stu-id="2479f-114">String</span></span>| <span data-ttu-id="2479f-115">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="2479f-115">Name of the setting.</span></span> |
|<span data-ttu-id="2479f-116">type</span><span class="sxs-lookup"><span data-stu-id="2479f-116">type</span></span>|<span data-ttu-id="2479f-117">字符串</span><span class="sxs-lookup"><span data-stu-id="2479f-117">String</span></span>| <span data-ttu-id="2479f-118">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="2479f-118">Key of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="2479f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2479f-119">JSON representation</span></span>

<span data-ttu-id="2479f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2479f-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->