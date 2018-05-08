# <a name="outlookuser-resource-type"></a><span data-ttu-id="23b76-101">outlookUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="23b76-101">outlookUser resource type</span></span>


<span data-ttu-id="23b76-102">表示用户可用的 Outlook 服务。</span><span class="sxs-lookup"><span data-stu-id="23b76-102">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="23b76-103">方法</span><span class="sxs-lookup"><span data-stu-id="23b76-103">Methods</span></span>

| <span data-ttu-id="23b76-104">方法</span><span class="sxs-lookup"><span data-stu-id="23b76-104">Method</span></span>           | <span data-ttu-id="23b76-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="23b76-105">Return Type</span></span>    |<span data-ttu-id="23b76-106">说明</span><span class="sxs-lookup"><span data-stu-id="23b76-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23b76-107">Create category</span><span class="sxs-lookup"><span data-stu-id="23b76-107">Create category</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="23b76-108">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="23b76-108">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="23b76-109">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="23b76-109">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="23b76-110">List categories</span><span class="sxs-lookup"><span data-stu-id="23b76-110">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="23b76-111">[outlookCategory](outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23b76-111">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="23b76-112">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="23b76-112">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="23b76-113">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="23b76-113">supportedLanguages</span></span>](../api/outlookuser_supportedlanguages.md) | <span data-ttu-id="23b76-114">[localeInfo](localeinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23b76-114">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="23b76-115">获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="23b76-115">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="23b76-116">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="23b76-116">supportedTimeZones</span></span>](../api/outlookuser_supportedtimezones.md) | <span data-ttu-id="23b76-117">[timeZoneInformation](timezoneinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23b76-117">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="23b76-118">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="23b76-118">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="23b76-119">属性</span><span class="sxs-lookup"><span data-stu-id="23b76-119">Properties</span></span>
<span data-ttu-id="23b76-120">无</span><span class="sxs-lookup"><span data-stu-id="23b76-120">None</span></span>

## <a name="relationships"></a><span data-ttu-id="23b76-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="23b76-121">Relationships</span></span>
| <span data-ttu-id="23b76-122">关系</span><span class="sxs-lookup"><span data-stu-id="23b76-122">Relationship</span></span> | <span data-ttu-id="23b76-123">类型</span><span class="sxs-lookup"><span data-stu-id="23b76-123">Type</span></span>   |<span data-ttu-id="23b76-124">说明</span><span class="sxs-lookup"><span data-stu-id="23b76-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23b76-125">masterCategories</span><span class="sxs-lookup"><span data-stu-id="23b76-125">masterCategories</span></span>|<span data-ttu-id="23b76-126">[outlookCategory](../resources/outlookCategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23b76-126">[outlookCategory](../resources/outlookCategory.md) collection</span></span>| <span data-ttu-id="23b76-127">为用户定义的类别列表。</span><span class="sxs-lookup"><span data-stu-id="23b76-127">A list of categories defined for the user.</span></span> | 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->