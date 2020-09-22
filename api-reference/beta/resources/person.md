---
title: person 资源类型
description: 有关来自邮件、联系人和社交网络的人员的信息聚合。用户可以是本地联系人、来自社交网络的联系人、组织的目录以及来自最近通信 (（如电子邮件和 Skype) ）的人员。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: cc63a75af497a2402955c39a2bcfc8efe370c782
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998038"
---
# <a name="person-resource-type"></a><span data-ttu-id="e5b2d-104">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5b2d-104">person resource type</span></span>

<span data-ttu-id="e5b2d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5b2d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b2d-p102">有关来自邮件、联系人和社交网络的人员的信息聚合。用户可以是本地联系人、来自社交网络的联系人、组织的目录以及来自最近通信 (（如电子邮件和 Skype) ）的人员。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-p102">An aggregation of information about a person from across mail, contacts and social networks. People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="e5b2d-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5b2d-108">Methods</span></span>

| <span data-ttu-id="e5b2d-109">方法</span><span class="sxs-lookup"><span data-stu-id="e5b2d-109">Method</span></span> | <span data-ttu-id="e5b2d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5b2d-110">Return Type</span></span> | <span data-ttu-id="e5b2d-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5b2d-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5b2d-112">List people</span><span class="sxs-lookup"><span data-stu-id="e5b2d-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="e5b2d-113">**person**</span><span class="sxs-lookup"><span data-stu-id="e5b2d-113">**person**</span></span> |<span data-ttu-id="e5b2d-114">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="e5b2d-115">属性</span><span class="sxs-lookup"><span data-stu-id="e5b2d-115">Properties</span></span>

| <span data-ttu-id="e5b2d-116">属性</span><span class="sxs-lookup"><span data-stu-id="e5b2d-116">Property</span></span> | <span data-ttu-id="e5b2d-117">类型</span><span class="sxs-lookup"><span data-stu-id="e5b2d-117">Type</span></span> | <span data-ttu-id="e5b2d-118">说明</span><span class="sxs-lookup"><span data-stu-id="e5b2d-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e5b2d-119">birthday</span><span class="sxs-lookup"><span data-stu-id="e5b2d-119">birthday</span></span>|<span data-ttu-id="e5b2d-120">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-120">string</span></span>|<span data-ttu-id="e5b2d-121">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-121">The person's birthday.</span></span>|
|<span data-ttu-id="e5b2d-122">companyName</span><span class="sxs-lookup"><span data-stu-id="e5b2d-122">companyName</span></span>|<span data-ttu-id="e5b2d-123">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-123">string</span></span>|<span data-ttu-id="e5b2d-124">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-124">The name of the person's company.</span></span>|
|<span data-ttu-id="e5b2d-125">department</span><span class="sxs-lookup"><span data-stu-id="e5b2d-125">department</span></span>|<span data-ttu-id="e5b2d-126">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-126">string</span></span>|<span data-ttu-id="e5b2d-127">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-127">The person's department.</span></span>|
|<span data-ttu-id="e5b2d-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e5b2d-128">displayName</span></span>|<span data-ttu-id="e5b2d-129">string</span><span class="sxs-lookup"><span data-stu-id="e5b2d-129">string</span></span>|<span data-ttu-id="e5b2d-130">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-130">The person's display name.</span></span>|
|<span data-ttu-id="e5b2d-131">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="e5b2d-131">emailAddresses</span></span>|<span data-ttu-id="e5b2d-132">[rankedEmailAddress](rankedemailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5b2d-132">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="e5b2d-133">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-133">The person's email addresses.</span></span>|
|<span data-ttu-id="e5b2d-134">givenName</span><span class="sxs-lookup"><span data-stu-id="e5b2d-134">givenName</span></span>|<span data-ttu-id="e5b2d-135">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-135">string</span></span>|<span data-ttu-id="e5b2d-136">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-136">The person's given name.</span></span>|
|<span data-ttu-id="e5b2d-137">id</span><span class="sxs-lookup"><span data-stu-id="e5b2d-137">id</span></span>|<span data-ttu-id="e5b2d-138">string</span><span class="sxs-lookup"><span data-stu-id="e5b2d-138">string</span></span>|<span data-ttu-id="e5b2d-p103">人员的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="e5b2d-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="e5b2d-141">isFavorite</span></span>|<span data-ttu-id="e5b2d-142">boolean</span><span class="sxs-lookup"><span data-stu-id="e5b2d-142">boolean</span></span>|<span data-ttu-id="e5b2d-143">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="e5b2d-144">mailboxType</span><span class="sxs-lookup"><span data-stu-id="e5b2d-144">mailboxType</span></span>|<span data-ttu-id="e5b2d-145">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-145">string</span></span>|<span data-ttu-id="e5b2d-146">由个人的电子邮件地址表示的邮箱类型。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-146">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="e5b2d-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e5b2d-147">officeLocation</span></span>|<span data-ttu-id="e5b2d-148">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-148">string</span></span>|<span data-ttu-id="e5b2d-149">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-149">The location of the person's office.</span></span>|
|<span data-ttu-id="e5b2d-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="e5b2d-150">personNotes</span></span>|<span data-ttu-id="e5b2d-151">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-151">string</span></span>|<span data-ttu-id="e5b2d-152">用户对此人员所做的自由格式备注。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="e5b2d-153">personType</span><span class="sxs-lookup"><span data-stu-id="e5b2d-153">personType</span></span>|<span data-ttu-id="e5b2d-154">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-154">string</span></span>|<span data-ttu-id="e5b2d-155">人员类型，例如通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-155">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="e5b2d-156">phones</span><span class="sxs-lookup"><span data-stu-id="e5b2d-156">phones</span></span>|<span data-ttu-id="e5b2d-157">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="e5b2d-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="e5b2d-158">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="e5b2d-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="e5b2d-159">postalAddresses</span></span>|<span data-ttu-id="e5b2d-160">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="e5b2d-160">[location](location.md) collection</span></span>|<span data-ttu-id="e5b2d-161">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-161">The person's addresses.</span></span>|
|<span data-ttu-id="e5b2d-162">profession</span><span class="sxs-lookup"><span data-stu-id="e5b2d-162">profession</span></span>|<span data-ttu-id="e5b2d-163">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-163">string</span></span>|<span data-ttu-id="e5b2d-164">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-164">The person's profession.</span></span>|
|<span data-ttu-id="e5b2d-165">源</span><span class="sxs-lookup"><span data-stu-id="e5b2d-165">sources</span></span>|<span data-ttu-id="e5b2d-166">[personDataSource](persondatasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5b2d-166">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="e5b2d-167">用户数据来自的源，例如目录或 Outlook 联系人。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-167">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="e5b2d-168">surname</span><span class="sxs-lookup"><span data-stu-id="e5b2d-168">surname</span></span>|<span data-ttu-id="e5b2d-169">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-169">string</span></span>|<span data-ttu-id="e5b2d-170">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-170">The person's surname.</span></span>|
|<span data-ttu-id="e5b2d-171">title</span><span class="sxs-lookup"><span data-stu-id="e5b2d-171">title</span></span>|<span data-ttu-id="e5b2d-172">string</span><span class="sxs-lookup"><span data-stu-id="e5b2d-172">string</span></span>|<span data-ttu-id="e5b2d-173">人员的职务。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-173">The person's title.</span></span>|
|<span data-ttu-id="e5b2d-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e5b2d-174">userPrincipalName</span></span>|<span data-ttu-id="e5b2d-175">string</span><span class="sxs-lookup"><span data-stu-id="e5b2d-175">string</span></span>|<span data-ttu-id="e5b2d-p104">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="e5b2d-180">websites</span><span class="sxs-lookup"><span data-stu-id="e5b2d-180">websites</span></span>|<span data-ttu-id="e5b2d-181">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="e5b2d-181">[website](website.md) collection</span></span>|<span data-ttu-id="e5b2d-182">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-182">The person's websites.</span></span>|
|<span data-ttu-id="e5b2d-183">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="e5b2d-183">yomiCompany</span></span>|<span data-ttu-id="e5b2d-184">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b2d-184">string</span></span>|<span data-ttu-id="e5b2d-185">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-185">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5b2d-186">关系</span><span class="sxs-lookup"><span data-stu-id="e5b2d-186">Relationships</span></span>

<span data-ttu-id="e5b2d-187">无</span><span class="sxs-lookup"><span data-stu-id="e5b2d-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5b2d-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5b2d-188">JSON representation</span></span>

<span data-ttu-id="e5b2d-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5b2d-189">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


