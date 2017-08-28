# <a name="quota-resource-type"></a><span data-ttu-id="4cf54-101">配额资源类型</span><span class="sxs-lookup"><span data-stu-id="4cf54-101">Quota resource type</span></span>

<span data-ttu-id="4cf54-102">**配额**资源提供有关 [驱动器](drive.md) 资源上的空间限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4cf54-102">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cf54-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cf54-103">JSON representation</span></span>

<span data-ttu-id="4cf54-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cf54-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="4cf54-105">属性</span><span class="sxs-lookup"><span data-stu-id="4cf54-105">Properties</span></span>

| <span data-ttu-id="4cf54-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="4cf54-106">Property name</span></span> | <span data-ttu-id="4cf54-107">类型</span><span class="sxs-lookup"><span data-stu-id="4cf54-107">Type</span></span>   | <span data-ttu-id="4cf54-108">说明</span><span class="sxs-lookup"><span data-stu-id="4cf54-108">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="4cf54-109">total</span><span class="sxs-lookup"><span data-stu-id="4cf54-109">total</span></span>         | <span data-ttu-id="4cf54-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4cf54-110">Int64</span></span>  | <span data-ttu-id="4cf54-p101">允许的总存储空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="4cf54-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="4cf54-113">used</span><span class="sxs-lookup"><span data-stu-id="4cf54-113">used</span></span>          | <span data-ttu-id="4cf54-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4cf54-114">Int64</span></span>  | <span data-ttu-id="4cf54-p102">已使用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="4cf54-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="4cf54-117">remaining</span><span class="sxs-lookup"><span data-stu-id="4cf54-117">remaining</span></span>     | <span data-ttu-id="4cf54-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4cf54-118">Int64</span></span>  | <span data-ttu-id="4cf54-p103">达到配额限制之前剩余的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="4cf54-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="4cf54-121">deleted</span><span class="sxs-lookup"><span data-stu-id="4cf54-121">deleted</span></span>       | <span data-ttu-id="4cf54-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4cf54-122">Int64</span></span>  | <span data-ttu-id="4cf54-p104">回收站中的文件占用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="4cf54-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="4cf54-125">state</span><span class="sxs-lookup"><span data-stu-id="4cf54-125">state</span></span>         | <span data-ttu-id="4cf54-126">string</span><span class="sxs-lookup"><span data-stu-id="4cf54-126">string</span></span> | <span data-ttu-id="4cf54-p105">指示存储空间状态的枚举值。只读。</span><span class="sxs-lookup"><span data-stu-id="4cf54-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="4cf54-129">状态枚举</span><span class="sxs-lookup"><span data-stu-id="4cf54-129">State Enumeration</span></span>

| <span data-ttu-id="4cf54-130">值</span><span class="sxs-lookup"><span data-stu-id="4cf54-130">Value</span></span>      | <span data-ttu-id="4cf54-131">说明</span><span class="sxs-lookup"><span data-stu-id="4cf54-131">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="4cf54-132">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="4cf54-132">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="4cf54-133">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="4cf54-133">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="4cf54-134">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="4cf54-134">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="4cf54-p106">使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="4cf54-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "quota resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
