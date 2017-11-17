# <a name="settingvalue-resource-type"></a><span data-ttu-id="69946-101">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="69946-101">settingValue resource type</span></span>

<span data-ttu-id="69946-102">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="69946-102">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="69946-103">属性</span><span class="sxs-lookup"><span data-stu-id="69946-103">Properties</span></span>

| <span data-ttu-id="69946-104">属性</span><span class="sxs-lookup"><span data-stu-id="69946-104">Property</span></span> | <span data-ttu-id="69946-105">类型</span><span class="sxs-lookup"><span data-stu-id="69946-105">Type</span></span> | <span data-ttu-id="69946-106">说明</span><span class="sxs-lookup"><span data-stu-id="69946-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="69946-107">名称</span><span class="sxs-lookup"><span data-stu-id="69946-107">name</span></span>|<span data-ttu-id="69946-108">字符串</span><span class="sxs-lookup"><span data-stu-id="69946-108">String</span></span>| <span data-ttu-id="69946-109">设置的名称（由 [groupSettingTemplate](groupsettingtemplate.md) 定义）。</span><span class="sxs-lookup"><span data-stu-id="69946-109">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="69946-110">value</span><span class="sxs-lookup"><span data-stu-id="69946-110">value</span></span>|<span data-ttu-id="69946-111">字符串</span><span class="sxs-lookup"><span data-stu-id="69946-111">String</span></span>| <span data-ttu-id="69946-112">设置的值。</span><span class="sxs-lookup"><span data-stu-id="69946-112">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="69946-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69946-113">JSON representation</span></span>

<span data-ttu-id="69946-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69946-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->