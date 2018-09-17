# <a name="security-resource-type"></a><span data-ttu-id="9d636-101">安全资源类型</span><span class="sxs-lookup"><span data-stu-id="9d636-101">security resource type</span></span>

<span data-ttu-id="9d636-102">安全资源是安全对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="9d636-102">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="9d636-103">它返回 singleton 安全资源。</span><span class="sxs-lookup"><span data-stu-id="9d636-103">It returns a singleton security resource.</span></span> <span data-ttu-id="9d636-104">它不包含任何可用的属性。</span><span class="sxs-lookup"><span data-stu-id="9d636-104">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="9d636-105">方法</span><span class="sxs-lookup"><span data-stu-id="9d636-105">Methods</span></span>

| <span data-ttu-id="9d636-106">方法</span><span class="sxs-lookup"><span data-stu-id="9d636-106">Method</span></span>       | <span data-ttu-id="9d636-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d636-107">Return Type</span></span> | <span data-ttu-id="9d636-108">说明</span><span class="sxs-lookup"><span data-stu-id="9d636-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9d636-109">列出警报</span><span class="sxs-lookup"><span data-stu-id="9d636-109">List alerts</span></span>](../api/alert_list.md) | <span data-ttu-id="9d636-110">[提示](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d636-110">[alert](alert.md) collection</span></span> | <span data-ttu-id="9d636-111">获取提示对象集合。</span><span class="sxs-lookup"><span data-stu-id="9d636-111">Get a licenseDetails object collection.</span></span> |
| [<span data-ttu-id="9d636-112">获取通知</span><span class="sxs-lookup"><span data-stu-id="9d636-112">get alerts</span></span>](../api/alert_get.md) | <span data-ttu-id="9d636-113">[提示](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d636-113">[alert](alert.md) collection</span></span> | <span data-ttu-id="9d636-114">获取通知对象。</span><span class="sxs-lookup"><span data-stu-id="9d636-114">Get a alert object.</span></span> |
| [<span data-ttu-id="9d636-115">更新通知</span><span class="sxs-lookup"><span data-stu-id="9d636-115">Update alerts</span></span>](../api/alert_update.md) | <span data-ttu-id="9d636-116">[提示](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d636-116">[alert](alert.md) collection</span></span> | <span data-ttu-id="9d636-117">获取通知对象。</span><span class="sxs-lookup"><span data-stu-id="9d636-117">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d636-118">属性</span><span class="sxs-lookup"><span data-stu-id="9d636-118">Properties</span></span>
<span data-ttu-id="9d636-119">无</span><span class="sxs-lookup"><span data-stu-id="9d636-119">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9d636-120">关系</span><span class="sxs-lookup"><span data-stu-id="9d636-120">Relationships</span></span>
| <span data-ttu-id="9d636-121">关系</span><span class="sxs-lookup"><span data-stu-id="9d636-121">Relationship</span></span> | <span data-ttu-id="9d636-122">类型</span><span class="sxs-lookup"><span data-stu-id="9d636-122">Type</span></span>        | <span data-ttu-id="9d636-123">说明</span><span class="sxs-lookup"><span data-stu-id="9d636-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9d636-124">alerts</span><span class="sxs-lookup"><span data-stu-id="9d636-124">alerts</span></span>|<span data-ttu-id="9d636-125">[提示](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d636-125">[alert](alert.md) collection</span></span>| <span data-ttu-id="9d636-p102">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9d636-p102">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9d636-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d636-128">JSON representation</span></span>
<span data-ttu-id="9d636-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d636-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="9d636-130">示例</span><span class="sxs-lookup"><span data-stu-id="9d636-130">Example</span></span>

<span data-ttu-id="9d636-131">**安全**资源可在图表的根目录中使用。</span><span class="sxs-lookup"><span data-stu-id="9d636-131">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->