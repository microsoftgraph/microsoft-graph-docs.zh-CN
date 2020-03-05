---
title: person 资源类型
description: 邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 27f0f5c27814ff09433cc68b82930878feb95963
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447204"
---
# <a name="person-resource-type"></a><span data-ttu-id="9c61b-104">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c61b-104">person resource type</span></span>

<span data-ttu-id="9c61b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c61b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c61b-p102">邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。</span><span class="sxs-lookup"><span data-stu-id="9c61b-p102">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="9c61b-108">方法</span><span class="sxs-lookup"><span data-stu-id="9c61b-108">Methods</span></span>

| <span data-ttu-id="9c61b-109">方法</span><span class="sxs-lookup"><span data-stu-id="9c61b-109">Method</span></span> | <span data-ttu-id="9c61b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9c61b-110">Return Type</span></span> | <span data-ttu-id="9c61b-111">说明</span><span class="sxs-lookup"><span data-stu-id="9c61b-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c61b-112">List people</span><span class="sxs-lookup"><span data-stu-id="9c61b-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="9c61b-113">**person**</span><span class="sxs-lookup"><span data-stu-id="9c61b-113">**person**</span></span> |<span data-ttu-id="9c61b-114">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="9c61b-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="9c61b-115">属性</span><span class="sxs-lookup"><span data-stu-id="9c61b-115">Properties</span></span>

| <span data-ttu-id="9c61b-116">属性</span><span class="sxs-lookup"><span data-stu-id="9c61b-116">Property</span></span> | <span data-ttu-id="9c61b-117">类型</span><span class="sxs-lookup"><span data-stu-id="9c61b-117">Type</span></span> | <span data-ttu-id="9c61b-118">说明</span><span class="sxs-lookup"><span data-stu-id="9c61b-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9c61b-119">birthday</span><span class="sxs-lookup"><span data-stu-id="9c61b-119">birthday</span></span>|<span data-ttu-id="9c61b-120">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-120">String</span></span>|<span data-ttu-id="9c61b-121">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="9c61b-121">The person's birthday.</span></span>|
|<span data-ttu-id="9c61b-122">companyName</span><span class="sxs-lookup"><span data-stu-id="9c61b-122">companyName</span></span>|<span data-ttu-id="9c61b-123">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-123">String</span></span>|<span data-ttu-id="9c61b-124">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="9c61b-124">The name of the person's company.</span></span>|
|<span data-ttu-id="9c61b-125">department</span><span class="sxs-lookup"><span data-stu-id="9c61b-125">department</span></span>|<span data-ttu-id="9c61b-126">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-126">String</span></span>|<span data-ttu-id="9c61b-127">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="9c61b-127">The person's department.</span></span>|
|<span data-ttu-id="9c61b-128">displayName</span><span class="sxs-lookup"><span data-stu-id="9c61b-128">displayName</span></span>|<span data-ttu-id="9c61b-129">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-129">String</span></span>|<span data-ttu-id="9c61b-130">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9c61b-130">The person's display name.</span></span>|
|<span data-ttu-id="9c61b-131">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="9c61b-131">scoredEmailAddresses</span></span>|<span data-ttu-id="9c61b-132">[scoredEmailAddress](scoredemailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="9c61b-132">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="9c61b-133">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9c61b-133">The person's email addresses.</span></span>|
|<span data-ttu-id="9c61b-134">givenName</span><span class="sxs-lookup"><span data-stu-id="9c61b-134">givenName</span></span>|<span data-ttu-id="9c61b-135">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-135">String</span></span>|<span data-ttu-id="9c61b-136">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="9c61b-136">The person's given name.</span></span>|
|<span data-ttu-id="9c61b-137">id</span><span class="sxs-lookup"><span data-stu-id="9c61b-137">id</span></span>|<span data-ttu-id="9c61b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="9c61b-138">String</span></span>|<span data-ttu-id="9c61b-p103">人员的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9c61b-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="9c61b-141">imAddress</span><span class="sxs-lookup"><span data-stu-id="9c61b-141">imAddress</span></span>|<span data-ttu-id="9c61b-142">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-142">String</span></span>|<span data-ttu-id="9c61b-p104">用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。</span><span class="sxs-lookup"><span data-stu-id="9c61b-p104">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="9c61b-145">isFavorite</span><span class="sxs-lookup"><span data-stu-id="9c61b-145">isFavorite</span></span>|<span data-ttu-id="9c61b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c61b-146">Boolean</span></span>|<span data-ttu-id="9c61b-147">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="9c61b-147">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="9c61b-148">jobTitle</span><span class="sxs-lookup"><span data-stu-id="9c61b-148">jobTitle</span></span>|<span data-ttu-id="9c61b-149">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-149">String</span></span>|<span data-ttu-id="9c61b-150">人员的职务。</span><span class="sxs-lookup"><span data-stu-id="9c61b-150">The person's job title.</span></span>|
|<span data-ttu-id="9c61b-151">officeLocation</span><span class="sxs-lookup"><span data-stu-id="9c61b-151">officeLocation</span></span>|<span data-ttu-id="9c61b-152">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-152">String</span></span>|<span data-ttu-id="9c61b-153">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="9c61b-153">The location of the person's office.</span></span>|
|<span data-ttu-id="9c61b-154">personNotes</span><span class="sxs-lookup"><span data-stu-id="9c61b-154">personNotes</span></span>|<span data-ttu-id="9c61b-155">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-155">String</span></span>|<span data-ttu-id="9c61b-156">用户对此人员所做的自由格式备注。</span><span class="sxs-lookup"><span data-stu-id="9c61b-156">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="9c61b-157">personType</span><span class="sxs-lookup"><span data-stu-id="9c61b-157">personType</span></span>|[<span data-ttu-id="9c61b-158">personType</span><span class="sxs-lookup"><span data-stu-id="9c61b-158">personType</span></span>](persontype.md) |<span data-ttu-id="9c61b-159">人员类型。</span><span class="sxs-lookup"><span data-stu-id="9c61b-159">The type of person.</span></span>|
|<span data-ttu-id="9c61b-160">phones</span><span class="sxs-lookup"><span data-stu-id="9c61b-160">phones</span></span>|<span data-ttu-id="9c61b-161">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="9c61b-161">[phone](phone.md) collection</span></span>|<span data-ttu-id="9c61b-162">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="9c61b-162">The person's phone numbers.</span></span>|
|<span data-ttu-id="9c61b-163">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="9c61b-163">postalAddresses</span></span>|<span data-ttu-id="9c61b-164">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="9c61b-164">[location](location.md) collection</span></span>|<span data-ttu-id="9c61b-165">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="9c61b-165">The person's addresses.</span></span>|
|<span data-ttu-id="9c61b-166">profession</span><span class="sxs-lookup"><span data-stu-id="9c61b-166">profession</span></span>|<span data-ttu-id="9c61b-167">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-167">String</span></span>|<span data-ttu-id="9c61b-168">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="9c61b-168">The person's profession.</span></span>|
|<span data-ttu-id="9c61b-169">surname</span><span class="sxs-lookup"><span data-stu-id="9c61b-169">surname</span></span>|<span data-ttu-id="9c61b-170">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-170">String</span></span>|<span data-ttu-id="9c61b-171">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="9c61b-171">The person's surname.</span></span>|
|<span data-ttu-id="9c61b-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c61b-172">userPrincipalName</span></span>|<span data-ttu-id="9c61b-173">字符串</span><span class="sxs-lookup"><span data-stu-id="9c61b-173">String</span></span>|<span data-ttu-id="9c61b-p105">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="9c61b-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="9c61b-178">websites</span><span class="sxs-lookup"><span data-stu-id="9c61b-178">websites</span></span>|<span data-ttu-id="9c61b-179">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="9c61b-179">[website](website.md) collection</span></span>|<span data-ttu-id="9c61b-180">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="9c61b-180">The person's websites.</span></span>|
|<span data-ttu-id="9c61b-181">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="9c61b-181">yomiCompany</span></span>|<span data-ttu-id="9c61b-182">String</span><span class="sxs-lookup"><span data-stu-id="9c61b-182">String</span></span>|<span data-ttu-id="9c61b-183">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="9c61b-183">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c61b-184">Relationships</span><span class="sxs-lookup"><span data-stu-id="9c61b-184">Relationships</span></span>

<span data-ttu-id="9c61b-185">无。</span><span class="sxs-lookup"><span data-stu-id="9c61b-185">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c61b-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c61b-186">JSON representation</span></span>

<span data-ttu-id="9c61b-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c61b-187">The following is a JSON representation of the resource.</span></span>

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
