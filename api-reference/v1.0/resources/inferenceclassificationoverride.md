# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="72f83-101">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="72f83-101">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="72f83-102">表示来自特定发件人的传入邮件始终应如何分类的用户的替代。</span><span class="sxs-lookup"><span data-stu-id="72f83-102">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="72f83-103">方法</span><span class="sxs-lookup"><span data-stu-id="72f83-103">Methods</span></span>

| <span data-ttu-id="72f83-104">方法</span><span class="sxs-lookup"><span data-stu-id="72f83-104">Method</span></span>           | <span data-ttu-id="72f83-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="72f83-105">Return Type</span></span>    |<span data-ttu-id="72f83-106">说明</span><span class="sxs-lookup"><span data-stu-id="72f83-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72f83-107">更新</span><span class="sxs-lookup"><span data-stu-id="72f83-107">Update</span></span>](../api/inferenceclassificationoverride_update.md) | [<span data-ttu-id="72f83-108">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="72f83-108">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="72f83-109">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="72f83-109">Change the **classifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="72f83-110">删除</span><span class="sxs-lookup"><span data-stu-id="72f83-110">Delete</span></span>](../api/inferenceclassificationoverride_delete.md) | <span data-ttu-id="72f83-111">无</span><span class="sxs-lookup"><span data-stu-id="72f83-111">None</span></span> |<span data-ttu-id="72f83-112">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="72f83-112">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="72f83-113">属性</span><span class="sxs-lookup"><span data-stu-id="72f83-113">Properties</span></span>
| <span data-ttu-id="72f83-114">属性</span><span class="sxs-lookup"><span data-stu-id="72f83-114">Property</span></span>     | <span data-ttu-id="72f83-115">类型</span><span class="sxs-lookup"><span data-stu-id="72f83-115">Type</span></span>   |<span data-ttu-id="72f83-116">说明</span><span class="sxs-lookup"><span data-stu-id="72f83-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72f83-117">classifyAs</span><span class="sxs-lookup"><span data-stu-id="72f83-117">classifyAs</span></span>|<span data-ttu-id="72f83-118">InferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="72f83-118">InferenceClassificationType</span></span>| <span data-ttu-id="72f83-119">指定来自特定发件人的传入邮件始终应如何分类。</span><span class="sxs-lookup"><span data-stu-id="72f83-119">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: , .</span></span> <span data-ttu-id="72f83-120">可取值为：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="72f83-120">The possible values are:</span></span>|
|<span data-ttu-id="72f83-121">id</span><span class="sxs-lookup"><span data-stu-id="72f83-121">id</span></span>|<span data-ttu-id="72f83-122">string</span><span class="sxs-lookup"><span data-stu-id="72f83-122">string</span></span>| <span data-ttu-id="72f83-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="72f83-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="72f83-125">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="72f83-125">senderEmailAddress</span></span>|[<span data-ttu-id="72f83-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="72f83-126">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="72f83-127">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="72f83-127">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72f83-128">关系</span><span class="sxs-lookup"><span data-stu-id="72f83-128">Relationships</span></span>
<span data-ttu-id="72f83-129">无</span><span class="sxs-lookup"><span data-stu-id="72f83-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="72f83-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72f83-130">JSON representation</span></span>

<span data-ttu-id="72f83-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72f83-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->