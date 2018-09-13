# <a name="filehash-resource-type"></a><span data-ttu-id="337a6-101">fileHash 资源类型</span><span class="sxs-lookup"><span data-stu-id="337a6-101">fileHash resource type</span></span>

<span data-ttu-id="337a6-102">包含有关文件哈希（加密和位置）的有状态信息。</span><span class="sxs-lookup"><span data-stu-id="337a6-102">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="337a6-103">属性</span><span class="sxs-lookup"><span data-stu-id="337a6-103">Properties</span></span>

| <span data-ttu-id="337a6-104">属性</span><span class="sxs-lookup"><span data-stu-id="337a6-104">Property</span></span>     | <span data-ttu-id="337a6-105">类型</span><span class="sxs-lookup"><span data-stu-id="337a6-105">Type</span></span>        | <span data-ttu-id="337a6-106">说明</span><span class="sxs-lookup"><span data-stu-id="337a6-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="337a6-107">hashType</span><span class="sxs-lookup"><span data-stu-id="337a6-107">hashType</span></span>|<span data-ttu-id="337a6-108">fileHashType</span><span class="sxs-lookup"><span data-stu-id="337a6-108">fileHashType</span></span>|<span data-ttu-id="337a6-109">文件哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="337a6-109">File hash type.</span></span> <span data-ttu-id="337a6-110">可能的值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256`。</span><span class="sxs-lookup"><span data-stu-id="337a6-110">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="337a6-111">hashValue</span><span class="sxs-lookup"><span data-stu-id="337a6-111">hashValue</span></span>|<span data-ttu-id="337a6-112">字符串</span><span class="sxs-lookup"><span data-stu-id="337a6-112">String</span></span>|<span data-ttu-id="337a6-113">文件哈希值。</span><span class="sxs-lookup"><span data-stu-id="337a6-113">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="337a6-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="337a6-114">JSON representation</span></span>

<span data-ttu-id="337a6-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="337a6-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->