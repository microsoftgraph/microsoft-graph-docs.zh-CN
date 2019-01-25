---
title: person 资源类型
description: 有关跨邮件、 联系人和社交网络从个人信息的聚合。 人员可以是本地联系人、 社交网络的联系人，贵组织的目录和 （如电子邮件和 Skype） 最近通信的人员。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 32a2c9905ab52e9b229bb8673fb4a84d90a706ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512400"
---
# <a name="person-resource-type"></a><span data-ttu-id="577a1-104">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="577a1-104">person resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="577a1-105">有关跨邮件、 联系人和社交网络从个人信息的聚合。</span><span class="sxs-lookup"><span data-stu-id="577a1-105">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="577a1-106">人员可以是本地联系人、 社交网络的联系人，贵组织的目录和 （如电子邮件和 Skype） 最近通信的人员。</span><span class="sxs-lookup"><span data-stu-id="577a1-106">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="577a1-107">方法</span><span class="sxs-lookup"><span data-stu-id="577a1-107">Methods</span></span>

| <span data-ttu-id="577a1-108">方法</span><span class="sxs-lookup"><span data-stu-id="577a1-108">Method</span></span> | <span data-ttu-id="577a1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="577a1-109">Return Type</span></span> | <span data-ttu-id="577a1-110">说明</span><span class="sxs-lookup"><span data-stu-id="577a1-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="577a1-111">List people</span><span class="sxs-lookup"><span data-stu-id="577a1-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="577a1-112">**person**</span><span class="sxs-lookup"><span data-stu-id="577a1-112">**person**</span></span> |<span data-ttu-id="577a1-113">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="577a1-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="577a1-114">属性</span><span class="sxs-lookup"><span data-stu-id="577a1-114">Properties</span></span>

| <span data-ttu-id="577a1-115">属性</span><span class="sxs-lookup"><span data-stu-id="577a1-115">Property</span></span> | <span data-ttu-id="577a1-116">类型</span><span class="sxs-lookup"><span data-stu-id="577a1-116">Type</span></span> | <span data-ttu-id="577a1-117">说明</span><span class="sxs-lookup"><span data-stu-id="577a1-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="577a1-118">birthday</span><span class="sxs-lookup"><span data-stu-id="577a1-118">birthday</span></span>|<span data-ttu-id="577a1-119">string</span><span class="sxs-lookup"><span data-stu-id="577a1-119">string</span></span>|<span data-ttu-id="577a1-120">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="577a1-120">The person's birthday.</span></span>|
|<span data-ttu-id="577a1-121">companyName</span><span class="sxs-lookup"><span data-stu-id="577a1-121">companyName</span></span>|<span data-ttu-id="577a1-122">string</span><span class="sxs-lookup"><span data-stu-id="577a1-122">string</span></span>|<span data-ttu-id="577a1-123">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="577a1-123">The name of the person's company.</span></span>|
|<span data-ttu-id="577a1-124">department</span><span class="sxs-lookup"><span data-stu-id="577a1-124">department</span></span>|<span data-ttu-id="577a1-125">string</span><span class="sxs-lookup"><span data-stu-id="577a1-125">string</span></span>|<span data-ttu-id="577a1-126">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="577a1-126">The person's department.</span></span>|
|<span data-ttu-id="577a1-127">displayName</span><span class="sxs-lookup"><span data-stu-id="577a1-127">displayName</span></span>|<span data-ttu-id="577a1-128">string</span><span class="sxs-lookup"><span data-stu-id="577a1-128">string</span></span>|<span data-ttu-id="577a1-129">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="577a1-129">The person's display name.</span></span>|
|<span data-ttu-id="577a1-130">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="577a1-130">emailAddresses</span></span>|<span data-ttu-id="577a1-131">[rankedEmailAddress](rankedemailaddress.md)集合</span><span class="sxs-lookup"><span data-stu-id="577a1-131">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="577a1-132">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="577a1-132">The person's email addresses.</span></span>|
|<span data-ttu-id="577a1-133">givenName</span><span class="sxs-lookup"><span data-stu-id="577a1-133">givenName</span></span>|<span data-ttu-id="577a1-134">string</span><span class="sxs-lookup"><span data-stu-id="577a1-134">string</span></span>|<span data-ttu-id="577a1-135">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="577a1-135">The person's given name.</span></span>|
|<span data-ttu-id="577a1-136">id</span><span class="sxs-lookup"><span data-stu-id="577a1-136">id</span></span>|<span data-ttu-id="577a1-137">string</span><span class="sxs-lookup"><span data-stu-id="577a1-137">string</span></span>|<span data-ttu-id="577a1-p103">人员的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="577a1-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="577a1-140">isFavorite</span><span class="sxs-lookup"><span data-stu-id="577a1-140">isFavorite</span></span>|<span data-ttu-id="577a1-141">布尔</span><span class="sxs-lookup"><span data-stu-id="577a1-141">boolean</span></span>|<span data-ttu-id="577a1-142">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="577a1-142">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="577a1-143">MailboxType</span><span class="sxs-lookup"><span data-stu-id="577a1-143">mailboxType</span></span>|<span data-ttu-id="577a1-144">string</span><span class="sxs-lookup"><span data-stu-id="577a1-144">string</span></span>|<span data-ttu-id="577a1-145">由此人的电子邮件地址的邮箱的类型。</span><span class="sxs-lookup"><span data-stu-id="577a1-145">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="577a1-146">officeLocation</span><span class="sxs-lookup"><span data-stu-id="577a1-146">officeLocation</span></span>|<span data-ttu-id="577a1-147">string</span><span class="sxs-lookup"><span data-stu-id="577a1-147">string</span></span>|<span data-ttu-id="577a1-148">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="577a1-148">The location of the person's office.</span></span>|
|<span data-ttu-id="577a1-149">personNotes</span><span class="sxs-lookup"><span data-stu-id="577a1-149">personNotes</span></span>|<span data-ttu-id="577a1-150">string</span><span class="sxs-lookup"><span data-stu-id="577a1-150">string</span></span>|<span data-ttu-id="577a1-151">用户对此人员所做的自由格式备注。</span><span class="sxs-lookup"><span data-stu-id="577a1-151">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="577a1-152">personType</span><span class="sxs-lookup"><span data-stu-id="577a1-152">personType</span></span>|<span data-ttu-id="577a1-153">string</span><span class="sxs-lookup"><span data-stu-id="577a1-153">string</span></span>|<span data-ttu-id="577a1-154">人员，例如通讯组列表的类型。</span><span class="sxs-lookup"><span data-stu-id="577a1-154">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="577a1-155">phones</span><span class="sxs-lookup"><span data-stu-id="577a1-155">phones</span></span>|<span data-ttu-id="577a1-156">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="577a1-156">[phone](phone.md) collection</span></span>|<span data-ttu-id="577a1-157">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="577a1-157">The person's phone numbers.</span></span>|
|<span data-ttu-id="577a1-158">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="577a1-158">postalAddresses</span></span>|<span data-ttu-id="577a1-159">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="577a1-159">[location](location.md) collection</span></span>|<span data-ttu-id="577a1-160">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="577a1-160">The person's addresses.</span></span>|
|<span data-ttu-id="577a1-161">profession</span><span class="sxs-lookup"><span data-stu-id="577a1-161">profession</span></span>|<span data-ttu-id="577a1-162">string</span><span class="sxs-lookup"><span data-stu-id="577a1-162">string</span></span>|<span data-ttu-id="577a1-163">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="577a1-163">The person's profession.</span></span>|
|<span data-ttu-id="577a1-164">sources</span><span class="sxs-lookup"><span data-stu-id="577a1-164">sources</span></span>|<span data-ttu-id="577a1-165">[personDataSource](persondatasource.md)集合</span><span class="sxs-lookup"><span data-stu-id="577a1-165">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="577a1-166">源用户数据来自，例如目录或 Outlook 联系人。</span><span class="sxs-lookup"><span data-stu-id="577a1-166">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="577a1-167">surname</span><span class="sxs-lookup"><span data-stu-id="577a1-167">surname</span></span>|<span data-ttu-id="577a1-168">string</span><span class="sxs-lookup"><span data-stu-id="577a1-168">string</span></span>|<span data-ttu-id="577a1-169">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="577a1-169">The person's surname.</span></span>|
|<span data-ttu-id="577a1-170">title</span><span class="sxs-lookup"><span data-stu-id="577a1-170">title</span></span>|<span data-ttu-id="577a1-171">string</span><span class="sxs-lookup"><span data-stu-id="577a1-171">string</span></span>|<span data-ttu-id="577a1-172">此人的标题。</span><span class="sxs-lookup"><span data-stu-id="577a1-172">The person's title.</span></span>|
|<span data-ttu-id="577a1-173">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="577a1-173">userPrincipalName</span></span>|<span data-ttu-id="577a1-174">string</span><span class="sxs-lookup"><span data-stu-id="577a1-174">string</span></span>|<span data-ttu-id="577a1-p104">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="577a1-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="577a1-179">websites</span><span class="sxs-lookup"><span data-stu-id="577a1-179">websites</span></span>|<span data-ttu-id="577a1-180">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="577a1-180">[website](website.md) collection</span></span>|<span data-ttu-id="577a1-181">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="577a1-181">The person's websites.</span></span>|
|<span data-ttu-id="577a1-182">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="577a1-182">yomiCompany</span></span>|<span data-ttu-id="577a1-183">string</span><span class="sxs-lookup"><span data-stu-id="577a1-183">string</span></span>|<span data-ttu-id="577a1-184">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="577a1-184">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="577a1-185">Relationships</span><span class="sxs-lookup"><span data-stu-id="577a1-185">Relationships</span></span>

<span data-ttu-id="577a1-186">无</span><span class="sxs-lookup"><span data-stu-id="577a1-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="577a1-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="577a1-187">JSON representation</span></span>

<span data-ttu-id="577a1-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="577a1-188">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/person.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
