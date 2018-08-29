# <a name="profilephoto-resource-type"></a><span data-ttu-id="9ce6e-101">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ce6e-101">profilePhoto resource type</span></span>
<span data-ttu-id="9ce6e-p101">从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-p101">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="9ce6e-104">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-104">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="9ce6e-105">方法</span><span class="sxs-lookup"><span data-stu-id="9ce6e-105">Methods</span></span>

| <span data-ttu-id="9ce6e-106">方法</span><span class="sxs-lookup"><span data-stu-id="9ce6e-106">Method</span></span>       | <span data-ttu-id="9ce6e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ce6e-107">Return Type</span></span>  |<span data-ttu-id="9ce6e-108">说明</span><span class="sxs-lookup"><span data-stu-id="9ce6e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ce6e-109">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9ce6e-109">Get profilePhoto</span></span>](../api/profilephoto_get.md) | [<span data-ttu-id="9ce6e-110">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9ce6e-110">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="9ce6e-111">获取指定的 **profilePhoto** 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-111">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="9ce6e-112">更新</span><span class="sxs-lookup"><span data-stu-id="9ce6e-112">Update</span></span>](../api/profilephoto_update.md) | [<span data-ttu-id="9ce6e-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9ce6e-113">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="9ce6e-p102">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-p102">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ce6e-117">属性</span><span class="sxs-lookup"><span data-stu-id="9ce6e-117">Properties</span></span>
| <span data-ttu-id="9ce6e-118">属性</span><span class="sxs-lookup"><span data-stu-id="9ce6e-118">Property</span></span>     | <span data-ttu-id="9ce6e-119">类型</span><span class="sxs-lookup"><span data-stu-id="9ce6e-119">Type</span></span>   |<span data-ttu-id="9ce6e-120">说明</span><span class="sxs-lookup"><span data-stu-id="9ce6e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ce6e-121">id</span><span class="sxs-lookup"><span data-stu-id="9ce6e-121">id</span></span>|<span data-ttu-id="9ce6e-122">string</span><span class="sxs-lookup"><span data-stu-id="9ce6e-122">string</span></span>|<span data-ttu-id="9ce6e-123">只读。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-123">Read-only.</span></span>|
|<span data-ttu-id="9ce6e-124">height</span><span class="sxs-lookup"><span data-stu-id="9ce6e-124">height</span></span>|<span data-ttu-id="9ce6e-125">int32</span><span class="sxs-lookup"><span data-stu-id="9ce6e-125">int32</span></span>|<span data-ttu-id="9ce6e-p103">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-p103">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="9ce6e-128">width</span><span class="sxs-lookup"><span data-stu-id="9ce6e-128">width</span></span>|<span data-ttu-id="9ce6e-129">int32</span><span class="sxs-lookup"><span data-stu-id="9ce6e-129">int32</span></span>|<span data-ttu-id="9ce6e-p104">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-p104">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ce6e-132">Relationships</span><span class="sxs-lookup"><span data-stu-id="9ce6e-132">Relationships</span></span>
<span data-ttu-id="9ce6e-133">无</span><span class="sxs-lookup"><span data-stu-id="9ce6e-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9ce6e-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ce6e-134">JSON representation</span></span>

<span data-ttu-id="9ce6e-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ce6e-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
