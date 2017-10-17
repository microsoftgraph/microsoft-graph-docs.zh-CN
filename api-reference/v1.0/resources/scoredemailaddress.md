# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="ba16f-101">scoredEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba16f-101">scoredEmailAddress resource type</span></span>

<span data-ttu-id="ba16f-102">表示经过评分的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ba16f-102">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="ba16f-103">属性</span><span class="sxs-lookup"><span data-stu-id="ba16f-103">Properties</span></span>
| <span data-ttu-id="ba16f-104">属性</span><span class="sxs-lookup"><span data-stu-id="ba16f-104">Property</span></span>     | <span data-ttu-id="ba16f-105">类型</span><span class="sxs-lookup"><span data-stu-id="ba16f-105">Type</span></span>   |<span data-ttu-id="ba16f-106">说明</span><span class="sxs-lookup"><span data-stu-id="ba16f-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba16f-107">address</span><span class="sxs-lookup"><span data-stu-id="ba16f-107">address</span></span>|<span data-ttu-id="ba16f-108">string</span><span class="sxs-lookup"><span data-stu-id="ba16f-108">string</span></span>|<span data-ttu-id="ba16f-109">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ba16f-109">The email address.</span></span>|
|<span data-ttu-id="ba16f-110">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="ba16f-110">relevanceScore</span></span>|<span data-ttu-id="ba16f-111">double</span><span class="sxs-lookup"><span data-stu-id="ba16f-111">double</span></span>|<span data-ttu-id="ba16f-p101">电子邮件地址的相关性评分。相关性评分用作排序关键字，与其他返回的结果相关。相关性评分值越高，对应结果的相关性越高。相关性由用户的通信和协作模式及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="ba16f-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba16f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba16f-116">JSON representation</span></span>

<span data-ttu-id="ba16f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba16f-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
