# <a name="person-resource-type"></a><span data-ttu-id="7a53a-101">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a53a-101">person resource type</span></span>

<span data-ttu-id="7a53a-p101">邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。</span><span class="sxs-lookup"><span data-stu-id="7a53a-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="7a53a-104">方法</span><span class="sxs-lookup"><span data-stu-id="7a53a-104">Methods</span></span>

| <span data-ttu-id="7a53a-105">方法</span><span class="sxs-lookup"><span data-stu-id="7a53a-105">Method</span></span> | <span data-ttu-id="7a53a-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a53a-106">Return Type</span></span> | <span data-ttu-id="7a53a-107">说明</span><span class="sxs-lookup"><span data-stu-id="7a53a-107">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a53a-108">List people</span><span class="sxs-lookup"><span data-stu-id="7a53a-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="7a53a-109">**person**</span><span class="sxs-lookup"><span data-stu-id="7a53a-109">**person**</span></span> |<span data-ttu-id="7a53a-110">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="7a53a-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="7a53a-111">属性</span><span class="sxs-lookup"><span data-stu-id="7a53a-111">Properties</span></span>

| <span data-ttu-id="7a53a-112">属性</span><span class="sxs-lookup"><span data-stu-id="7a53a-112">Property</span></span> | <span data-ttu-id="7a53a-113">类型</span><span class="sxs-lookup"><span data-stu-id="7a53a-113">Type</span></span> | <span data-ttu-id="7a53a-114">说明</span><span class="sxs-lookup"><span data-stu-id="7a53a-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7a53a-115">birthday</span><span class="sxs-lookup"><span data-stu-id="7a53a-115">birthday</span></span>|<span data-ttu-id="7a53a-116">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-116">String</span></span>|<span data-ttu-id="7a53a-117">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="7a53a-117">The person's birthday.</span></span>|
|<span data-ttu-id="7a53a-118">companyName</span><span class="sxs-lookup"><span data-stu-id="7a53a-118">companyName</span></span>|<span data-ttu-id="7a53a-119">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-119">String</span></span>|<span data-ttu-id="7a53a-120">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="7a53a-120">The name of the person's company.</span></span>|
|<span data-ttu-id="7a53a-121">department</span><span class="sxs-lookup"><span data-stu-id="7a53a-121">department</span></span>|<span data-ttu-id="7a53a-122">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-122">String</span></span>|<span data-ttu-id="7a53a-123">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="7a53a-123">The person's department.</span></span>|
|<span data-ttu-id="7a53a-124">displayName</span><span class="sxs-lookup"><span data-stu-id="7a53a-124">displayName</span></span>|<span data-ttu-id="7a53a-125">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-125">String</span></span>|<span data-ttu-id="7a53a-126">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7a53a-126">The person's display name.</span></span>|
|<span data-ttu-id="7a53a-127">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="7a53a-127">scoredEmailAddresses</span></span>|<span data-ttu-id="7a53a-128">[scoredEmailAddress](scoredemailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a53a-128">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="7a53a-129">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7a53a-129">The person's email addresses.</span></span>|
|<span data-ttu-id="7a53a-130">givenName</span><span class="sxs-lookup"><span data-stu-id="7a53a-130">givenName</span></span>|<span data-ttu-id="7a53a-131">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-131">String</span></span>|<span data-ttu-id="7a53a-132">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="7a53a-132">The person's given name.</span></span>|
|<span data-ttu-id="7a53a-133">id</span><span class="sxs-lookup"><span data-stu-id="7a53a-133">id</span></span>|<span data-ttu-id="7a53a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7a53a-134">String</span></span>|<span data-ttu-id="7a53a-p102">人员的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7a53a-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="7a53a-137">imAddress</span><span class="sxs-lookup"><span data-stu-id="7a53a-137">imAddress</span></span>|<span data-ttu-id="7a53a-138">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-138">String</span></span>|<span data-ttu-id="7a53a-p103">用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。</span><span class="sxs-lookup"><span data-stu-id="7a53a-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="7a53a-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="7a53a-141">isFavorite</span></span>|<span data-ttu-id="7a53a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a53a-142">Boolean</span></span>|<span data-ttu-id="7a53a-143">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="7a53a-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="7a53a-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="7a53a-144">jobTitle</span></span>|<span data-ttu-id="7a53a-145">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-145">String</span></span>|<span data-ttu-id="7a53a-146">人员的职务。</span><span class="sxs-lookup"><span data-stu-id="7a53a-146">The person's job title.</span></span>|
|<span data-ttu-id="7a53a-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="7a53a-147">officeLocation</span></span>|<span data-ttu-id="7a53a-148">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-148">String</span></span>|<span data-ttu-id="7a53a-149">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="7a53a-149">The location of the person's office.</span></span>|
|<span data-ttu-id="7a53a-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="7a53a-150">personNotes</span></span>|<span data-ttu-id="7a53a-151">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-151">String</span></span>|<span data-ttu-id="7a53a-152">用户对此人员所做的自由格式备注。</span><span class="sxs-lookup"><span data-stu-id="7a53a-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="7a53a-153">personType</span><span class="sxs-lookup"><span data-stu-id="7a53a-153">personType</span></span>|[<span data-ttu-id="7a53a-154">personType</span><span class="sxs-lookup"><span data-stu-id="7a53a-154">personType</span></span>](persontype.md) |<span data-ttu-id="7a53a-155">人员类型。</span><span class="sxs-lookup"><span data-stu-id="7a53a-155">The type of person.</span></span>|
|<span data-ttu-id="7a53a-156">phones</span><span class="sxs-lookup"><span data-stu-id="7a53a-156">phones</span></span>|<span data-ttu-id="7a53a-157">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a53a-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="7a53a-158">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="7a53a-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="7a53a-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="7a53a-159">postalAddresses</span></span>|<span data-ttu-id="7a53a-160">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a53a-160">[location](location.md) collection</span></span>|<span data-ttu-id="7a53a-161">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="7a53a-161">The person's addresses.</span></span>|
|<span data-ttu-id="7a53a-162">profession</span><span class="sxs-lookup"><span data-stu-id="7a53a-162">profession</span></span>|<span data-ttu-id="7a53a-163">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-163">String</span></span>|<span data-ttu-id="7a53a-164">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="7a53a-164">The person's profession.</span></span>|
|<span data-ttu-id="7a53a-165">surname</span><span class="sxs-lookup"><span data-stu-id="7a53a-165">surname</span></span>|<span data-ttu-id="7a53a-166">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-166">String</span></span>|<span data-ttu-id="7a53a-167">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="7a53a-167">The person's surname.</span></span>|
|<span data-ttu-id="7a53a-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a53a-168">userPrincipalName</span></span>|<span data-ttu-id="7a53a-169">字符串</span><span class="sxs-lookup"><span data-stu-id="7a53a-169">String</span></span>|<span data-ttu-id="7a53a-p104">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="7a53a-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="7a53a-174">websites</span><span class="sxs-lookup"><span data-stu-id="7a53a-174">websites</span></span>|<span data-ttu-id="7a53a-175">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a53a-175">[website](website.md) collection</span></span>|<span data-ttu-id="7a53a-176">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="7a53a-176">The person's websites.</span></span>|
|<span data-ttu-id="7a53a-177">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="7a53a-177">yomiCompany</span></span>|<span data-ttu-id="7a53a-178">String</span><span class="sxs-lookup"><span data-stu-id="7a53a-178">String</span></span>|<span data-ttu-id="7a53a-179">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="7a53a-179">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a53a-180">Relationships</span><span class="sxs-lookup"><span data-stu-id="7a53a-180">Relationships</span></span>

<span data-ttu-id="7a53a-181">无。</span><span class="sxs-lookup"><span data-stu-id="7a53a-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a53a-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a53a-182">JSON representation</span></span>

<span data-ttu-id="7a53a-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a53a-183">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
