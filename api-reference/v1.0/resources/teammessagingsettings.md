# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="8a726-101">teamMessagingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a726-101">teamMessagingSettings resource type</span></span>



<span data-ttu-id="8a726-102">要配置的消息设置和[团队](team.md)中的提及。</span><span class="sxs-lookup"><span data-stu-id="8a726-102">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8a726-103">属性</span><span class="sxs-lookup"><span data-stu-id="8a726-103">Properties</span></span>
| <span data-ttu-id="8a726-104">属性</span><span class="sxs-lookup"><span data-stu-id="8a726-104">Property</span></span>     | <span data-ttu-id="8a726-105">类型</span><span class="sxs-lookup"><span data-stu-id="8a726-105">Type</span></span>   |<span data-ttu-id="8a726-106">说明</span><span class="sxs-lookup"><span data-stu-id="8a726-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a726-107">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="8a726-107">allowUserEditMessages</span></span>|<span data-ttu-id="8a726-108">布尔</span><span class="sxs-lookup"><span data-stu-id="8a726-108">Boolean</span></span>|<span data-ttu-id="8a726-109">如果设置为 true，则用户可以编辑他们的邮件。</span><span class="sxs-lookup"><span data-stu-id="8a726-109">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="8a726-110">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="8a726-110">allowUserDeleteMessages</span></span>|<span data-ttu-id="8a726-111">布尔</span><span class="sxs-lookup"><span data-stu-id="8a726-111">Boolean</span></span>|<span data-ttu-id="8a726-112">如果设置为 true，则用户可以删除其邮件。</span><span class="sxs-lookup"><span data-stu-id="8a726-112">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="8a726-113">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="8a726-113">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="8a726-114">布尔</span><span class="sxs-lookup"><span data-stu-id="8a726-114">Boolean</span></span>|<span data-ttu-id="8a726-115">如果设置为 true，则所有者可以删除任何消息。</span><span class="sxs-lookup"><span data-stu-id="8a726-115">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="8a726-116">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="8a726-116">allowTeamMentions</span></span>|<span data-ttu-id="8a726-117">布尔</span><span class="sxs-lookup"><span data-stu-id="8a726-117">Boolean</span></span>|<span data-ttu-id="8a726-118">如果设置为 true，允许提及的 @team。</span><span class="sxs-lookup"><span data-stu-id="8a726-118">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="8a726-119">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="8a726-119">allowChannelMentions</span></span>|<span data-ttu-id="8a726-120">布尔</span><span class="sxs-lookup"><span data-stu-id="8a726-120">Boolean</span></span>|<span data-ttu-id="8a726-121">如果设置为 true，允许提及的 @channel。</span><span class="sxs-lookup"><span data-stu-id="8a726-121">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a726-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a726-122">JSON representation</span></span>

<span data-ttu-id="8a726-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a726-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
