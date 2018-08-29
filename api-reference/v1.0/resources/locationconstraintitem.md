# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="8240d-101">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="8240d-101">locationConstraintItem resource type</span></span>

<span data-ttu-id="8240d-102">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="8240d-102">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="8240d-103">由 [地点](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="8240d-103">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8240d-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8240d-104">JSON representation</span></span>

<span data-ttu-id="8240d-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8240d-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="8240d-106">属性</span><span class="sxs-lookup"><span data-stu-id="8240d-106">Properties</span></span>
| <span data-ttu-id="8240d-107">属性</span><span class="sxs-lookup"><span data-stu-id="8240d-107">Property</span></span>     | <span data-ttu-id="8240d-108">类型</span><span class="sxs-lookup"><span data-stu-id="8240d-108">Type</span></span>   |<span data-ttu-id="8240d-109">说明</span><span class="sxs-lookup"><span data-stu-id="8240d-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8240d-110">地址</span><span class="sxs-lookup"><span data-stu-id="8240d-110">address</span></span> | [<span data-ttu-id="8240d-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="8240d-111">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="8240d-112">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="8240d-112">The street address of the location.</span></span> |
| <span data-ttu-id="8240d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="8240d-113">displayName</span></span>  | <span data-ttu-id="8240d-114">字符串</span><span class="sxs-lookup"><span data-stu-id="8240d-114">String</span></span> | <span data-ttu-id="8240d-115">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="8240d-115">The name associated with the location.</span></span>                       |
| <span data-ttu-id="8240d-116">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8240d-116">locationEmailAddress</span></span> | <span data-ttu-id="8240d-117">字符串</span><span class="sxs-lookup"><span data-stu-id="8240d-117">String</span></span> | <span data-ttu-id="8240d-118">（可选）与地点相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8240d-118">Optional email address of the location.</span></span> |
| <span data-ttu-id="8240d-119">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="8240d-119">resolveAvailability</span></span> | <span data-ttu-id="8240d-120">布尔</span><span class="sxs-lookup"><span data-stu-id="8240d-120">Boolean</span></span> | <span data-ttu-id="8240d-p101">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user_findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="8240d-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user_findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->