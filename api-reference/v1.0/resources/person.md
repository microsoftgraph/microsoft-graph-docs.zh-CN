---
title: person 资源类型
description: 邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 66c37327f329995a84a8017625f86fde989b4e3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035544"
---
# <a name="person-resource-type"></a><span data-ttu-id="d9c1d-104">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9c1d-104">person resource type</span></span>

<span data-ttu-id="d9c1d-p102">邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-p102">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="d9c1d-107">方法</span><span class="sxs-lookup"><span data-stu-id="d9c1d-107">Methods</span></span>

| <span data-ttu-id="d9c1d-108">方法</span><span class="sxs-lookup"><span data-stu-id="d9c1d-108">Method</span></span> | <span data-ttu-id="d9c1d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9c1d-109">Return Type</span></span> | <span data-ttu-id="d9c1d-110">说明</span><span class="sxs-lookup"><span data-stu-id="d9c1d-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9c1d-111">List people</span><span class="sxs-lookup"><span data-stu-id="d9c1d-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="d9c1d-112">**person**</span><span class="sxs-lookup"><span data-stu-id="d9c1d-112">**person**</span></span> |<span data-ttu-id="d9c1d-113">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="d9c1d-114">属性</span><span class="sxs-lookup"><span data-stu-id="d9c1d-114">Properties</span></span>

| <span data-ttu-id="d9c1d-115">属性</span><span class="sxs-lookup"><span data-stu-id="d9c1d-115">Property</span></span> | <span data-ttu-id="d9c1d-116">类型</span><span class="sxs-lookup"><span data-stu-id="d9c1d-116">Type</span></span> | <span data-ttu-id="d9c1d-117">说明</span><span class="sxs-lookup"><span data-stu-id="d9c1d-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d9c1d-118">birthday</span><span class="sxs-lookup"><span data-stu-id="d9c1d-118">birthday</span></span>|<span data-ttu-id="d9c1d-119">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-119">String</span></span>|<span data-ttu-id="d9c1d-120">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-120">The person's birthday.</span></span>|
|<span data-ttu-id="d9c1d-121">companyName</span><span class="sxs-lookup"><span data-stu-id="d9c1d-121">companyName</span></span>|<span data-ttu-id="d9c1d-122">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-122">String</span></span>|<span data-ttu-id="d9c1d-123">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-123">The name of the person's company.</span></span>|
|<span data-ttu-id="d9c1d-124">department</span><span class="sxs-lookup"><span data-stu-id="d9c1d-124">department</span></span>|<span data-ttu-id="d9c1d-125">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-125">String</span></span>|<span data-ttu-id="d9c1d-126">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-126">The person's department.</span></span>|
|<span data-ttu-id="d9c1d-127">displayName</span><span class="sxs-lookup"><span data-stu-id="d9c1d-127">displayName</span></span>|<span data-ttu-id="d9c1d-128">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-128">String</span></span>|<span data-ttu-id="d9c1d-129">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-129">The person's display name.</span></span>|
|<span data-ttu-id="d9c1d-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="d9c1d-130">scoredEmailAddresses</span></span>|<span data-ttu-id="d9c1d-131">[scoredEmailAddress](scoredemailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="d9c1d-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="d9c1d-132">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-132">The person's email addresses.</span></span>|
|<span data-ttu-id="d9c1d-133">givenName</span><span class="sxs-lookup"><span data-stu-id="d9c1d-133">givenName</span></span>|<span data-ttu-id="d9c1d-134">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-134">String</span></span>|<span data-ttu-id="d9c1d-135">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-135">The person's given name.</span></span>|
|<span data-ttu-id="d9c1d-136">id</span><span class="sxs-lookup"><span data-stu-id="d9c1d-136">id</span></span>|<span data-ttu-id="d9c1d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="d9c1d-137">String</span></span>|<span data-ttu-id="d9c1d-p103">人员的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="d9c1d-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="d9c1d-140">imAddress</span></span>|<span data-ttu-id="d9c1d-141">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-141">String</span></span>|<span data-ttu-id="d9c1d-p104">用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-p104">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="d9c1d-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="d9c1d-144">isFavorite</span></span>|<span data-ttu-id="d9c1d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9c1d-145">Boolean</span></span>|<span data-ttu-id="d9c1d-146">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="d9c1d-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d9c1d-147">jobTitle</span></span>|<span data-ttu-id="d9c1d-148">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-148">String</span></span>|<span data-ttu-id="d9c1d-149">人员的职务。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-149">The person's job title.</span></span>|
|<span data-ttu-id="d9c1d-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="d9c1d-150">officeLocation</span></span>|<span data-ttu-id="d9c1d-151">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-151">String</span></span>|<span data-ttu-id="d9c1d-152">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-152">The location of the person's office.</span></span>|
|<span data-ttu-id="d9c1d-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="d9c1d-153">personNotes</span></span>|<span data-ttu-id="d9c1d-154">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-154">String</span></span>|<span data-ttu-id="d9c1d-155">用户对此人员所做的自由格式备注。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-155">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="d9c1d-156">personType</span><span class="sxs-lookup"><span data-stu-id="d9c1d-156">personType</span></span>|[<span data-ttu-id="d9c1d-157">personType</span><span class="sxs-lookup"><span data-stu-id="d9c1d-157">personType</span></span>](persontype.md) |<span data-ttu-id="d9c1d-158">人员类型。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-158">The type of person.</span></span>|
|<span data-ttu-id="d9c1d-159">phones</span><span class="sxs-lookup"><span data-stu-id="d9c1d-159">phones</span></span>|<span data-ttu-id="d9c1d-160">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="d9c1d-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="d9c1d-161">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-161">The person's phone numbers.</span></span>|
|<span data-ttu-id="d9c1d-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="d9c1d-162">postalAddresses</span></span>|<span data-ttu-id="d9c1d-163">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="d9c1d-163">[location](location.md) collection</span></span>|<span data-ttu-id="d9c1d-164">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-164">The person's addresses.</span></span>|
|<span data-ttu-id="d9c1d-165">profession</span><span class="sxs-lookup"><span data-stu-id="d9c1d-165">profession</span></span>|<span data-ttu-id="d9c1d-166">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-166">String</span></span>|<span data-ttu-id="d9c1d-167">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-167">The person's profession.</span></span>|
|<span data-ttu-id="d9c1d-168">surname</span><span class="sxs-lookup"><span data-stu-id="d9c1d-168">surname</span></span>|<span data-ttu-id="d9c1d-169">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-169">String</span></span>|<span data-ttu-id="d9c1d-170">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-170">The person's surname.</span></span>|
|<span data-ttu-id="d9c1d-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d9c1d-171">userPrincipalName</span></span>|<span data-ttu-id="d9c1d-172">字符串</span><span class="sxs-lookup"><span data-stu-id="d9c1d-172">String</span></span>|<span data-ttu-id="d9c1d-p105">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="d9c1d-177">websites</span><span class="sxs-lookup"><span data-stu-id="d9c1d-177">websites</span></span>|<span data-ttu-id="d9c1d-178">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="d9c1d-178">[website](website.md) collection</span></span>|<span data-ttu-id="d9c1d-179">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-179">The person's websites.</span></span>|
|<span data-ttu-id="d9c1d-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="d9c1d-180">yomiCompany</span></span>|<span data-ttu-id="d9c1d-181">String</span><span class="sxs-lookup"><span data-stu-id="d9c1d-181">String</span></span>|<span data-ttu-id="d9c1d-182">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-182">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9c1d-183">Relationships</span><span class="sxs-lookup"><span data-stu-id="d9c1d-183">Relationships</span></span>

<span data-ttu-id="d9c1d-184">无。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9c1d-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9c1d-185">JSON representation</span></span>

<span data-ttu-id="d9c1d-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9c1d-186">The following is a JSON representation of the resource.</span></span>

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
