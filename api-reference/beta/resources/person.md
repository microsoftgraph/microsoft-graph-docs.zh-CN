---
title: person 资源类型
description: 有关来自邮件、联系人和社交网络的人员的信息聚合。用户可以是本地联系人、来自社交网络的联系人、组织的目录以及来自最近通信（例如电子邮件和 Skype）的人员。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4df5f82bd14ba56969c26facef82b59f3ac7e3f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521937"
---
# <a name="person-resource-type"></a><span data-ttu-id="5656e-104">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="5656e-104">person resource type</span></span>

<span data-ttu-id="5656e-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5656e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5656e-106">有关来自邮件、联系人和社交网络的人员的信息聚合。</span><span class="sxs-lookup"><span data-stu-id="5656e-106">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="5656e-107">用户可以是本地联系人、来自社交网络的联系人、组织的目录以及来自最近通信（例如电子邮件和 Skype）的人员。</span><span class="sxs-lookup"><span data-stu-id="5656e-107">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="5656e-108">方法</span><span class="sxs-lookup"><span data-stu-id="5656e-108">Methods</span></span>

| <span data-ttu-id="5656e-109">方法</span><span class="sxs-lookup"><span data-stu-id="5656e-109">Method</span></span> | <span data-ttu-id="5656e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5656e-110">Return Type</span></span> | <span data-ttu-id="5656e-111">说明</span><span class="sxs-lookup"><span data-stu-id="5656e-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="5656e-112">List people</span><span class="sxs-lookup"><span data-stu-id="5656e-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="5656e-113">**person**</span><span class="sxs-lookup"><span data-stu-id="5656e-113">**person**</span></span> |<span data-ttu-id="5656e-114">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="5656e-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="5656e-115">属性</span><span class="sxs-lookup"><span data-stu-id="5656e-115">Properties</span></span>

| <span data-ttu-id="5656e-116">属性</span><span class="sxs-lookup"><span data-stu-id="5656e-116">Property</span></span> | <span data-ttu-id="5656e-117">类型</span><span class="sxs-lookup"><span data-stu-id="5656e-117">Type</span></span> | <span data-ttu-id="5656e-118">说明</span><span class="sxs-lookup"><span data-stu-id="5656e-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5656e-119">birthday</span><span class="sxs-lookup"><span data-stu-id="5656e-119">birthday</span></span>|<span data-ttu-id="5656e-120">string</span><span class="sxs-lookup"><span data-stu-id="5656e-120">string</span></span>|<span data-ttu-id="5656e-121">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="5656e-121">The person's birthday.</span></span>|
|<span data-ttu-id="5656e-122">companyName</span><span class="sxs-lookup"><span data-stu-id="5656e-122">companyName</span></span>|<span data-ttu-id="5656e-123">string</span><span class="sxs-lookup"><span data-stu-id="5656e-123">string</span></span>|<span data-ttu-id="5656e-124">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="5656e-124">The name of the person's company.</span></span>|
|<span data-ttu-id="5656e-125">department</span><span class="sxs-lookup"><span data-stu-id="5656e-125">department</span></span>|<span data-ttu-id="5656e-126">string</span><span class="sxs-lookup"><span data-stu-id="5656e-126">string</span></span>|<span data-ttu-id="5656e-127">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="5656e-127">The person's department.</span></span>|
|<span data-ttu-id="5656e-128">displayName</span><span class="sxs-lookup"><span data-stu-id="5656e-128">displayName</span></span>|<span data-ttu-id="5656e-129">string</span><span class="sxs-lookup"><span data-stu-id="5656e-129">string</span></span>|<span data-ttu-id="5656e-130">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5656e-130">The person's display name.</span></span>|
|<span data-ttu-id="5656e-131">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="5656e-131">emailAddresses</span></span>|<span data-ttu-id="5656e-132">[rankedEmailAddress](rankedemailaddress.md)集合</span><span class="sxs-lookup"><span data-stu-id="5656e-132">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="5656e-133">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5656e-133">The person's email addresses.</span></span>|
|<span data-ttu-id="5656e-134">givenName</span><span class="sxs-lookup"><span data-stu-id="5656e-134">givenName</span></span>|<span data-ttu-id="5656e-135">string</span><span class="sxs-lookup"><span data-stu-id="5656e-135">string</span></span>|<span data-ttu-id="5656e-136">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="5656e-136">The person's given name.</span></span>|
|<span data-ttu-id="5656e-137">id</span><span class="sxs-lookup"><span data-stu-id="5656e-137">id</span></span>|<span data-ttu-id="5656e-138">string</span><span class="sxs-lookup"><span data-stu-id="5656e-138">string</span></span>|<span data-ttu-id="5656e-139">人员的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5656e-139">The person's unique identifier.</span></span> <span data-ttu-id="5656e-140">只读。</span><span class="sxs-lookup"><span data-stu-id="5656e-140">Read-only.</span></span>|
|<span data-ttu-id="5656e-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="5656e-141">isFavorite</span></span>|<span data-ttu-id="5656e-142">boolean</span><span class="sxs-lookup"><span data-stu-id="5656e-142">boolean</span></span>|<span data-ttu-id="5656e-143">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="5656e-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="5656e-144">mailboxType</span><span class="sxs-lookup"><span data-stu-id="5656e-144">mailboxType</span></span>|<span data-ttu-id="5656e-145">string</span><span class="sxs-lookup"><span data-stu-id="5656e-145">string</span></span>|<span data-ttu-id="5656e-146">由个人的电子邮件地址表示的邮箱类型。</span><span class="sxs-lookup"><span data-stu-id="5656e-146">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="5656e-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="5656e-147">officeLocation</span></span>|<span data-ttu-id="5656e-148">string</span><span class="sxs-lookup"><span data-stu-id="5656e-148">string</span></span>|<span data-ttu-id="5656e-149">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="5656e-149">The location of the person's office.</span></span>|
|<span data-ttu-id="5656e-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="5656e-150">personNotes</span></span>|<span data-ttu-id="5656e-151">string</span><span class="sxs-lookup"><span data-stu-id="5656e-151">string</span></span>|<span data-ttu-id="5656e-152">用户对此人员所做的自由格式备注。</span><span class="sxs-lookup"><span data-stu-id="5656e-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="5656e-153">personType</span><span class="sxs-lookup"><span data-stu-id="5656e-153">personType</span></span>|<span data-ttu-id="5656e-154">string</span><span class="sxs-lookup"><span data-stu-id="5656e-154">string</span></span>|<span data-ttu-id="5656e-155">人员类型，例如通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="5656e-155">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="5656e-156">phones</span><span class="sxs-lookup"><span data-stu-id="5656e-156">phones</span></span>|<span data-ttu-id="5656e-157">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="5656e-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="5656e-158">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="5656e-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="5656e-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="5656e-159">postalAddresses</span></span>|<span data-ttu-id="5656e-160">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="5656e-160">[location](location.md) collection</span></span>|<span data-ttu-id="5656e-161">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="5656e-161">The person's addresses.</span></span>|
|<span data-ttu-id="5656e-162">profession</span><span class="sxs-lookup"><span data-stu-id="5656e-162">profession</span></span>|<span data-ttu-id="5656e-163">string</span><span class="sxs-lookup"><span data-stu-id="5656e-163">string</span></span>|<span data-ttu-id="5656e-164">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="5656e-164">The person's profession.</span></span>|
|<span data-ttu-id="5656e-165">源</span><span class="sxs-lookup"><span data-stu-id="5656e-165">sources</span></span>|<span data-ttu-id="5656e-166">[personDataSource](persondatasource.md)集合</span><span class="sxs-lookup"><span data-stu-id="5656e-166">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="5656e-167">用户数据来自的源，例如目录或 Outlook 联系人。</span><span class="sxs-lookup"><span data-stu-id="5656e-167">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="5656e-168">surname</span><span class="sxs-lookup"><span data-stu-id="5656e-168">surname</span></span>|<span data-ttu-id="5656e-169">string</span><span class="sxs-lookup"><span data-stu-id="5656e-169">string</span></span>|<span data-ttu-id="5656e-170">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="5656e-170">The person's surname.</span></span>|
|<span data-ttu-id="5656e-171">title</span><span class="sxs-lookup"><span data-stu-id="5656e-171">title</span></span>|<span data-ttu-id="5656e-172">string</span><span class="sxs-lookup"><span data-stu-id="5656e-172">string</span></span>|<span data-ttu-id="5656e-173">人员的职务。</span><span class="sxs-lookup"><span data-stu-id="5656e-173">The person's title.</span></span>|
|<span data-ttu-id="5656e-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5656e-174">userPrincipalName</span></span>|<span data-ttu-id="5656e-175">string</span><span class="sxs-lookup"><span data-stu-id="5656e-175">string</span></span>|<span data-ttu-id="5656e-p104">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="5656e-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="5656e-180">websites</span><span class="sxs-lookup"><span data-stu-id="5656e-180">websites</span></span>|<span data-ttu-id="5656e-181">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="5656e-181">[website](website.md) collection</span></span>|<span data-ttu-id="5656e-182">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="5656e-182">The person's websites.</span></span>|
|<span data-ttu-id="5656e-183">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="5656e-183">yomiCompany</span></span>|<span data-ttu-id="5656e-184">string</span><span class="sxs-lookup"><span data-stu-id="5656e-184">string</span></span>|<span data-ttu-id="5656e-185">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="5656e-185">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5656e-186">关系</span><span class="sxs-lookup"><span data-stu-id="5656e-186">Relationships</span></span>

<span data-ttu-id="5656e-187">无</span><span class="sxs-lookup"><span data-stu-id="5656e-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5656e-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5656e-188">JSON representation</span></span>

<span data-ttu-id="5656e-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5656e-189">Here is a JSON representation of the resource.</span></span>

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
