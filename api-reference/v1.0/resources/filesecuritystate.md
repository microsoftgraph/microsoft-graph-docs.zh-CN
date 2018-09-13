# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="c46c4-101">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c46c4-101">fileSecurityState resource type</span></span>

<span data-ttu-id="c46c4-102">包含有关与通知相关的文件（非进程）的信息。</span><span class="sxs-lookup"><span data-stu-id="c46c4-102">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="c46c4-103">属性</span><span class="sxs-lookup"><span data-stu-id="c46c4-103">Properties</span></span>

| <span data-ttu-id="c46c4-104">属性</span><span class="sxs-lookup"><span data-stu-id="c46c4-104">Property</span></span>   | <span data-ttu-id="c46c4-105">类型</span><span class="sxs-lookup"><span data-stu-id="c46c4-105">Type</span></span>|<span data-ttu-id="c46c4-106">说明</span><span class="sxs-lookup"><span data-stu-id="c46c4-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c46c4-107">fileHash</span><span class="sxs-lookup"><span data-stu-id="c46c4-107">fileHash</span></span>|[<span data-ttu-id="c46c4-108">fileHash</span><span class="sxs-lookup"><span data-stu-id="c46c4-108">fileHash</span></span>](filehash.md)|<span data-ttu-id="c46c4-109">包含文件哈希 （加密和位置敏感）的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="c46c4-109">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="c46c4-110">name</span><span class="sxs-lookup"><span data-stu-id="c46c4-110">name</span></span>|<span data-ttu-id="c46c4-111">字符串</span><span class="sxs-lookup"><span data-stu-id="c46c4-111">String</span></span>|<span data-ttu-id="c46c4-112">文件名 （无路径）。</span><span class="sxs-lookup"><span data-stu-id="c46c4-112">File name (without path).</span></span>|
|<span data-ttu-id="c46c4-113">path</span><span class="sxs-lookup"><span data-stu-id="c46c4-113">path</span></span>|<span data-ttu-id="c46c4-114">字符串</span><span class="sxs-lookup"><span data-stu-id="c46c4-114">String</span></span>|<span data-ttu-id="c46c4-115">文件/图片文件的完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="c46c4-115">Full file path of the stencil file</span></span>|
|<span data-ttu-id="c46c4-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="c46c4-116">riskScore</span></span>|<span data-ttu-id="c46c4-117">字符串</span><span class="sxs-lookup"><span data-stu-id="c46c4-117">String</span></span>|<span data-ttu-id="c46c4-118">提供程序生成/计算的通知文件风险评分。</span><span class="sxs-lookup"><span data-stu-id="c46c4-118">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="c46c4-119">建议值的范围为 0-1，相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="c46c4-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c46c4-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c46c4-120">JSON representation</span></span>

<span data-ttu-id="c46c4-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c46c4-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->