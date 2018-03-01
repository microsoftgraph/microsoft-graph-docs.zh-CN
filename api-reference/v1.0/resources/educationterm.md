# <a name="educationterm-resource-type"></a><span data-ttu-id="64e6a-101">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="64e6a-101">educationTerm resource type</span></span>

<span data-ttu-id="64e6a-102">一个学期。</span><span class="sxs-lookup"><span data-stu-id="64e6a-102">A term.</span></span> <span data-ttu-id="64e6a-103">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="64e6a-103">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="64e6a-104">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="64e6a-104">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="64e6a-105">属性</span><span class="sxs-lookup"><span data-stu-id="64e6a-105">Properties</span></span>
| <span data-ttu-id="64e6a-106">属性</span><span class="sxs-lookup"><span data-stu-id="64e6a-106">Property</span></span>     | <span data-ttu-id="64e6a-107">类型</span><span class="sxs-lookup"><span data-stu-id="64e6a-107">Type</span></span>   |<span data-ttu-id="64e6a-108">说明</span><span class="sxs-lookup"><span data-stu-id="64e6a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64e6a-109">displayName</span><span class="sxs-lookup"><span data-stu-id="64e6a-109">displayName</span></span>| <span data-ttu-id="64e6a-110">String</span><span class="sxs-lookup"><span data-stu-id="64e6a-110">String</span></span>| <span data-ttu-id="64e6a-111">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="64e6a-111">The name of the term.</span></span>| 
|<span data-ttu-id="64e6a-112">externalId</span><span class="sxs-lookup"><span data-stu-id="64e6a-112">externalId</span></span>|<span data-ttu-id="64e6a-113">String</span><span class="sxs-lookup"><span data-stu-id="64e6a-113">String</span></span>| <span data-ttu-id="64e6a-114">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="64e6a-114">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="64e6a-115">startDate</span><span class="sxs-lookup"><span data-stu-id="64e6a-115">startDate</span></span>|<span data-ttu-id="64e6a-116">Date</span><span class="sxs-lookup"><span data-stu-id="64e6a-116">Date</span></span>|<span data-ttu-id="64e6a-117">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="64e6a-117">Start of the term.</span></span>|
|<span data-ttu-id="64e6a-118">endDate</span><span class="sxs-lookup"><span data-stu-id="64e6a-118">endDate</span></span>|<span data-ttu-id="64e6a-119">Date</span><span class="sxs-lookup"><span data-stu-id="64e6a-119">Date</span></span>|<span data-ttu-id="64e6a-120">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="64e6a-120">End of the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64e6a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64e6a-121">JSON representation</span></span>

<span data-ttu-id="64e6a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64e6a-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->