# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="967df-101">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="967df-101">WorksheetProtection resource type</span></span>

<span data-ttu-id="967df-102">表示对 sheet 对象的保护。</span><span class="sxs-lookup"><span data-stu-id="967df-102">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="967df-103">方法</span><span class="sxs-lookup"><span data-stu-id="967df-103">Methods</span></span>

| <span data-ttu-id="967df-104">方法</span><span class="sxs-lookup"><span data-stu-id="967df-104">Method</span></span>           | <span data-ttu-id="967df-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="967df-105">Return Type</span></span>    |<span data-ttu-id="967df-106">说明</span><span class="sxs-lookup"><span data-stu-id="967df-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="967df-107">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="967df-107">Get WorksheetProtection</span></span>](../api/worksheetprotection_get.md) | [<span data-ttu-id="967df-108">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="967df-108">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="967df-109">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="967df-109">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="967df-110">Protect</span><span class="sxs-lookup"><span data-stu-id="967df-110">Protect</span></span>](../api/worksheetprotection_protect.md)|<span data-ttu-id="967df-111">无</span><span class="sxs-lookup"><span data-stu-id="967df-111">None</span></span>|<span data-ttu-id="967df-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="967df-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="967df-114">Unprotect</span><span class="sxs-lookup"><span data-stu-id="967df-114">Unprotect</span></span>](../api/worksheetprotection_unprotect.md)|<span data-ttu-id="967df-115">无</span><span class="sxs-lookup"><span data-stu-id="967df-115">None</span></span>|<span data-ttu-id="967df-116">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="967df-116">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="967df-117">属性</span><span class="sxs-lookup"><span data-stu-id="967df-117">Properties</span></span>
| <span data-ttu-id="967df-118">属性</span><span class="sxs-lookup"><span data-stu-id="967df-118">Property</span></span>     | <span data-ttu-id="967df-119">类型</span><span class="sxs-lookup"><span data-stu-id="967df-119">Type</span></span>   |<span data-ttu-id="967df-120">说明</span><span class="sxs-lookup"><span data-stu-id="967df-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="967df-121">options</span><span class="sxs-lookup"><span data-stu-id="967df-121">options</span></span>|[<span data-ttu-id="967df-122">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="967df-122">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="967df-p102">工作表保护选项。只读。</span><span class="sxs-lookup"><span data-stu-id="967df-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="967df-125">protected</span><span class="sxs-lookup"><span data-stu-id="967df-125">protected</span></span>|<span data-ttu-id="967df-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="967df-126">boolean</span></span>|<span data-ttu-id="967df-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="967df-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="967df-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="967df-129">JSON representation</span></span>

<span data-ttu-id="967df-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="967df-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->