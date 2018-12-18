---
title: person 资源类型
description: 有关跨邮件、 联系人和社交网络从个人信息的聚合。 人员可以是本地联系人、 社交网络的联系人，贵组织的目录和 （如电子邮件和 Skype） 最近通信的人员。
author: simonhult
ms.openlocfilehash: eccd5da56806b6608f5610579c61a171713990b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308552"
---
# <a name="person-resource-type"></a><span data-ttu-id="c3fc0-104">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3fc0-104">person resource type</span></span>

> <span data-ttu-id="c3fc0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3fc0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3fc0-107">有关跨邮件、 联系人和社交网络从个人信息的聚合。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-107">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="c3fc0-108">人员可以是本地联系人、 社交网络的联系人，贵组织的目录和 （如电子邮件和 Skype） 最近通信的人员。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-108">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="c3fc0-109">方法</span><span class="sxs-lookup"><span data-stu-id="c3fc0-109">Methods</span></span>

| <span data-ttu-id="c3fc0-110">方法</span><span class="sxs-lookup"><span data-stu-id="c3fc0-110">Method</span></span> | <span data-ttu-id="c3fc0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3fc0-111">Return Type</span></span> | <span data-ttu-id="c3fc0-112">说明</span><span class="sxs-lookup"><span data-stu-id="c3fc0-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3fc0-113">List people</span><span class="sxs-lookup"><span data-stu-id="c3fc0-113">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="c3fc0-114">**person**</span><span class="sxs-lookup"><span data-stu-id="c3fc0-114">**person**</span></span> |<span data-ttu-id="c3fc0-115">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-115">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="c3fc0-116">属性</span><span class="sxs-lookup"><span data-stu-id="c3fc0-116">Properties</span></span>

| <span data-ttu-id="c3fc0-117">属性</span><span class="sxs-lookup"><span data-stu-id="c3fc0-117">Property</span></span> | <span data-ttu-id="c3fc0-118">类型</span><span class="sxs-lookup"><span data-stu-id="c3fc0-118">Type</span></span> | <span data-ttu-id="c3fc0-119">说明</span><span class="sxs-lookup"><span data-stu-id="c3fc0-119">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c3fc0-120">birthday</span><span class="sxs-lookup"><span data-stu-id="c3fc0-120">birthday</span></span>|<span data-ttu-id="c3fc0-121">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-121">string</span></span>|<span data-ttu-id="c3fc0-122">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-122">The person's birthday.</span></span>|
|<span data-ttu-id="c3fc0-123">companyName</span><span class="sxs-lookup"><span data-stu-id="c3fc0-123">companyName</span></span>|<span data-ttu-id="c3fc0-124">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-124">string</span></span>|<span data-ttu-id="c3fc0-125">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-125">The name of the person's company.</span></span>|
|<span data-ttu-id="c3fc0-126">department</span><span class="sxs-lookup"><span data-stu-id="c3fc0-126">department</span></span>|<span data-ttu-id="c3fc0-127">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-127">string</span></span>|<span data-ttu-id="c3fc0-128">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-128">The person's department.</span></span>|
|<span data-ttu-id="c3fc0-129">displayName</span><span class="sxs-lookup"><span data-stu-id="c3fc0-129">displayName</span></span>|<span data-ttu-id="c3fc0-130">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-130">string</span></span>|<span data-ttu-id="c3fc0-131">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-131">The person's display name.</span></span>|
|<span data-ttu-id="c3fc0-132">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="c3fc0-132">emailAddresses</span></span>|<span data-ttu-id="c3fc0-133">[rankedEmailAddress](rankedemailaddress.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3fc0-133">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="c3fc0-134">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-134">The person's email addresses.</span></span>|
|<span data-ttu-id="c3fc0-135">givenName</span><span class="sxs-lookup"><span data-stu-id="c3fc0-135">givenName</span></span>|<span data-ttu-id="c3fc0-136">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-136">string</span></span>|<span data-ttu-id="c3fc0-137">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-137">The person's given name.</span></span>|
|<span data-ttu-id="c3fc0-138">id</span><span class="sxs-lookup"><span data-stu-id="c3fc0-138">id</span></span>|<span data-ttu-id="c3fc0-139">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-139">string</span></span>|<span data-ttu-id="c3fc0-p104">人员的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-p104">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="c3fc0-142">isFavorite</span><span class="sxs-lookup"><span data-stu-id="c3fc0-142">isFavorite</span></span>|<span data-ttu-id="c3fc0-143">boolean</span><span class="sxs-lookup"><span data-stu-id="c3fc0-143">boolean</span></span>|<span data-ttu-id="c3fc0-144">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-144">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="c3fc0-145">mailboxType</span><span class="sxs-lookup"><span data-stu-id="c3fc0-145">mailboxType</span></span>|<span data-ttu-id="c3fc0-146">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-146">string</span></span>|<span data-ttu-id="c3fc0-147">由此人的电子邮件地址的邮箱的类型。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-147">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="c3fc0-148">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c3fc0-148">officeLocation</span></span>|<span data-ttu-id="c3fc0-149">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-149">string</span></span>|<span data-ttu-id="c3fc0-150">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-150">The location of the person's office.</span></span>|
|<span data-ttu-id="c3fc0-151">personNotes</span><span class="sxs-lookup"><span data-stu-id="c3fc0-151">personNotes</span></span>|<span data-ttu-id="c3fc0-152">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-152">string</span></span>|<span data-ttu-id="c3fc0-153">用户对此人员所做的自由格式备注。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-153">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="c3fc0-154">personType</span><span class="sxs-lookup"><span data-stu-id="c3fc0-154">personType</span></span>|<span data-ttu-id="c3fc0-155">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-155">string</span></span>|<span data-ttu-id="c3fc0-156">人员，例如通讯组列表的类型。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-156">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="c3fc0-157">phones</span><span class="sxs-lookup"><span data-stu-id="c3fc0-157">phones</span></span>|<span data-ttu-id="c3fc0-158">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="c3fc0-158">[phone](phone.md) collection</span></span>|<span data-ttu-id="c3fc0-159">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-159">The person's phone numbers.</span></span>|
|<span data-ttu-id="c3fc0-160">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="c3fc0-160">postalAddresses</span></span>|<span data-ttu-id="c3fc0-161">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="c3fc0-161">[location](location.md) collection</span></span>|<span data-ttu-id="c3fc0-162">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-162">The person's addresses.</span></span>|
|<span data-ttu-id="c3fc0-163">profession</span><span class="sxs-lookup"><span data-stu-id="c3fc0-163">profession</span></span>|<span data-ttu-id="c3fc0-164">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-164">string</span></span>|<span data-ttu-id="c3fc0-165">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-165">The person's profession.</span></span>|
|<span data-ttu-id="c3fc0-166">sources</span><span class="sxs-lookup"><span data-stu-id="c3fc0-166">sources</span></span>|<span data-ttu-id="c3fc0-167">[personDataSource](persondatasource.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3fc0-167">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="c3fc0-168">源用户数据来自，例如目录或 Outlook 联系人。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-168">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="c3fc0-169">surname</span><span class="sxs-lookup"><span data-stu-id="c3fc0-169">surname</span></span>|<span data-ttu-id="c3fc0-170">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-170">string</span></span>|<span data-ttu-id="c3fc0-171">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-171">The person's surname.</span></span>|
|<span data-ttu-id="c3fc0-172">title</span><span class="sxs-lookup"><span data-stu-id="c3fc0-172">title</span></span>|<span data-ttu-id="c3fc0-173">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-173">string</span></span>|<span data-ttu-id="c3fc0-174">此人的标题。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-174">The person's title.</span></span>|
|<span data-ttu-id="c3fc0-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3fc0-175">userPrincipalName</span></span>|<span data-ttu-id="c3fc0-176">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-176">string</span></span>|<span data-ttu-id="c3fc0-p105">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="c3fc0-181">websites</span><span class="sxs-lookup"><span data-stu-id="c3fc0-181">websites</span></span>|<span data-ttu-id="c3fc0-182">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="c3fc0-182">[website](website.md) collection</span></span>|<span data-ttu-id="c3fc0-183">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-183">The person's websites.</span></span>|
|<span data-ttu-id="c3fc0-184">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="c3fc0-184">yomiCompany</span></span>|<span data-ttu-id="c3fc0-185">string</span><span class="sxs-lookup"><span data-stu-id="c3fc0-185">string</span></span>|<span data-ttu-id="c3fc0-186">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-186">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3fc0-187">Relationships</span><span class="sxs-lookup"><span data-stu-id="c3fc0-187">Relationships</span></span>

<span data-ttu-id="c3fc0-188">无</span><span class="sxs-lookup"><span data-stu-id="c3fc0-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3fc0-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3fc0-189">JSON representation</span></span>

<span data-ttu-id="c3fc0-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3fc0-190">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
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
