---
title: 在 Microsoft Graph 中使用 $search 查询参数
description: Microsoft Graph 支持 $search OData 查询参数，以便限制请求的结果来匹配搜索条件。
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 6e158d1d631536b11799b0b638b018dbbc98ef94
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443107"
---
# <a name="use-the-search-query-parameter-to-match-a-search-criterion"></a><span data-ttu-id="87e4f-103">使用搜索查询参数匹配搜索条件</span><span class="sxs-lookup"><span data-stu-id="87e4f-103">Use the search query parameter to match a search criterion</span></span>

<span data-ttu-id="87e4f-104">除了[其他 OData 查询参数](/graph/query-parameters)，Microsoft Graph 还支持`$search`查询参数，以便限制请求的结果来匹配搜索条件。</span><span class="sxs-lookup"><span data-stu-id="87e4f-104">In addition to [other OData query parameters](/graph/query-parameters), Microsoft Graph supports the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

<span data-ttu-id="87e4f-105">对`$search`查询参数的支持因实体而异，某些实体(例如派生自 [directoryObject](/graph/api/resources/directoryobject)的 Microsoft Azure Active Directory 资源)仅支持[高级查询](/graph/aad-advanced-queries)中的`$search`。</span><span class="sxs-lookup"><span data-stu-id="87e4f-105">The support for the `$search` query parameter varies by entity, with some, such as Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), supporting `$search` only in [advanced queries](/graph/aad-advanced-queries).</span></span>

> [!NOTE]
> <span data-ttu-id="87e4f-106">`$search`查询参数当前在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="87e4f-106">The `$search` query parameter is currently not available in Azure AD B2C tenants.</span></span>

## <a name="using-search-on-message-collections"></a><span data-ttu-id="87e4f-107">对 message 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="87e4f-107">Using $search on message collections</span></span>

<span data-ttu-id="87e4f-108">可根据特定邮件属性值搜索邮件。</span><span class="sxs-lookup"><span data-stu-id="87e4f-108">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="87e4f-109">搜索结果按邮件发送日期和时间进行排序。</span><span class="sxs-lookup"><span data-stu-id="87e4f-109">The results of the search are sorted by the date and time that the message was sent.</span></span> <span data-ttu-id="87e4f-110">`$search` 请求最多可返回 250 个结果。</span><span class="sxs-lookup"><span data-stu-id="87e4f-110">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="87e4f-111">如果确实要搜索邮件，且仅指定值，而未指定特定邮件属性，搜索依据为默认搜索属性 **from**、**subject** 和 **body**。</span><span class="sxs-lookup"><span data-stu-id="87e4f-111">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="87e4f-112">下面的示例返回登录用户收件箱中三个默认搜索属性中有任意一个包含“pizza”的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="87e4f-112">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="87e4f-113">也可以指定下表中的邮件属性名来搜索邮件，这些属性名可由关键字查询语言 (KQL) 语法识别。</span><span class="sxs-lookup"><span data-stu-id="87e4f-113">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="87e4f-114">这些属性名对应于 Microsoft Graph **message** 实体中定义的属性。</span><span class="sxs-lookup"><span data-stu-id="87e4f-114">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="87e4f-115">Outlook 和其他 Microsoft 365 应用程序（如 SharePoint）支持 KQL 语法，从而为数据存储提供了方便使用的公共发现域。</span><span class="sxs-lookup"><span data-stu-id="87e4f-115">Outlook and other Microsoft 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="87e4f-116">可搜索的电子邮件属性</span><span class="sxs-lookup"><span data-stu-id="87e4f-116">Searchable email property</span></span>                | <span data-ttu-id="87e4f-117">说明</span><span class="sxs-lookup"><span data-stu-id="87e4f-117">Description</span></span> | <span data-ttu-id="87e4f-118">示例</span><span class="sxs-lookup"><span data-stu-id="87e4f-118">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="87e4f-119">**attachment**</span><span class="sxs-lookup"><span data-stu-id="87e4f-119">**attachment**</span></span>           | <span data-ttu-id="87e4f-120">电子邮件附件的文件名。</span><span class="sxs-lookup"><span data-stu-id="87e4f-120">The names of files attached to an email message.</span></span>|<span data-ttu-id="87e4f-121">[GET][search-att-example] `../me/messages?$search="attachment:api-catalog.md"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-121">[GET][search-att-example] `../me/messages?$search="attachment:api-catalog.md"`</span></span>
| <span data-ttu-id="87e4f-122">**bcc**</span><span class="sxs-lookup"><span data-stu-id="87e4f-122">**bcc**</span></span>           | <span data-ttu-id="87e4f-123">电子邮件的 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="87e4f-123">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|<span data-ttu-id="87e4f-124">[GET][search-bcc-example] `../me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`</span><span class="sxs-lookup"><span data-stu-id="87e4f-124">[GET][search-bcc-example] `../me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`</span></span>
| <span data-ttu-id="87e4f-125">**body**</span><span class="sxs-lookup"><span data-stu-id="87e4f-125">**body**</span></span>           | <span data-ttu-id="87e4f-126">电子邮件正文。</span><span class="sxs-lookup"><span data-stu-id="87e4f-126">The body of an email message.</span></span>|<span data-ttu-id="87e4f-127">[GET][search-body-example] `../me/messages?$search="body:excitement"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-127">[GET][search-body-example] `../me/messages?$search="body:excitement"`</span></span>
| <span data-ttu-id="87e4f-128">**cc**</span><span class="sxs-lookup"><span data-stu-id="87e4f-128">**cc**</span></span>           | <span data-ttu-id="87e4f-129">电子邮件的 **cc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="87e4f-129">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|<span data-ttu-id="87e4f-130">[GET][search-cc-example] `../me/messages?$search="cc:danas"&$select=subject,ccRecipients`</span><span class="sxs-lookup"><span data-stu-id="87e4f-130">[GET][search-cc-example] `../me/messages?$search="cc:danas"&$select=subject,ccRecipients`</span></span>
| <span data-ttu-id="87e4f-131">**from**</span><span class="sxs-lookup"><span data-stu-id="87e4f-131">**from**</span></span>           | <span data-ttu-id="87e4f-132">电子邮件的发件人，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="87e4f-132">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>| <span data-ttu-id="87e4f-133">[GET][search-from-example] `../me/messages?$search="from:randiw"&$select=subject,from`</span><span class="sxs-lookup"><span data-stu-id="87e4f-133">[GET][search-from-example] `../me/messages?$search="from:randiw"&$select=subject,from`</span></span>
| <span data-ttu-id="87e4f-134">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="87e4f-134">**hasAttachment**</span></span> | <span data-ttu-id="87e4f-135">如果电子邮件附件不是内联附件，则为 true；否则，为 false。</span><span class="sxs-lookup"><span data-stu-id="87e4f-135">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> | <span data-ttu-id="87e4f-136">[GET][search-from-example] `../me/messages?$search="hasAttachments:true"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-136">[GET][search-from-example] `../me/messages?$search="hasAttachments:true"`</span></span>
| <span data-ttu-id="87e4f-137">**importance**</span><span class="sxs-lookup"><span data-stu-id="87e4f-137">**importance**</span></span>           | <span data-ttu-id="87e4f-138">发件人在发送邮件时可以指定的电子邮件重要性。</span><span class="sxs-lookup"><span data-stu-id="87e4f-138">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="87e4f-139">可取值包括 `low`、`medium` 或 `high`。</span><span class="sxs-lookup"><span data-stu-id="87e4f-139">The possible values are `low`, `medium`, or `high`.</span></span>|<span data-ttu-id="87e4f-140">[GET][search-imp-example] `../me/messages?$search="importance:high"&$select=subject,importance`</span><span class="sxs-lookup"><span data-stu-id="87e4f-140">[GET][search-imp-example] `../me/messages?$search="importance:high"&$select=subject,importance`</span></span>
| <span data-ttu-id="87e4f-141">**Kind**</span><span class="sxs-lookup"><span data-stu-id="87e4f-141">**kind**</span></span>           | <span data-ttu-id="87e4f-142">邮件类型。</span><span class="sxs-lookup"><span data-stu-id="87e4f-142">The type of message.</span></span> <span data-ttu-id="87e4f-143">可取值包括 `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks` 或 `voicemail`。</span><span class="sxs-lookup"><span data-stu-id="87e4f-143">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>| <span data-ttu-id="87e4f-144">[GET][search-kind-example] `../me/messages?$search="kind:voicemail"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-144">[GET][search-kind-example] `../me/messages?$search="kind:voicemail"`</span></span>
| <span data-ttu-id="87e4f-145">**participants**</span><span class="sxs-lookup"><span data-stu-id="87e4f-145">**participants**</span></span>           | <span data-ttu-id="87e4f-146">电子邮件的 **from**、**to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="87e4f-146">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>| <span data-ttu-id="87e4f-147">[GET][search-part-example] `../me/messages?$search="participants:danas"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-147">[GET][search-part-example] `../me/messages?$search="participants:danas"`</span></span>
| <span data-ttu-id="87e4f-148">**received**</span><span class="sxs-lookup"><span data-stu-id="87e4f-148">**received**</span></span>           | <span data-ttu-id="87e4f-149">收件人接收电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="87e4f-149">The date that an email message was received by a recipient.</span></span>| <span data-ttu-id="87e4f-150">[GET][search-rcvd-example] `../me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`</span><span class="sxs-lookup"><span data-stu-id="87e4f-150">[GET][search-rcvd-example] `../me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`</span></span>
| <span data-ttu-id="87e4f-151">**recipients**</span><span class="sxs-lookup"><span data-stu-id="87e4f-151">**recipients**</span></span>           | <span data-ttu-id="87e4f-152">电子邮件的 **to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="87e4f-152">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>| <span data-ttu-id="87e4f-153">[GET][search-rcpts-example] `../me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`</span><span class="sxs-lookup"><span data-stu-id="87e4f-153">[GET][search-rcpts-example] `../me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`</span></span>
| <span data-ttu-id="87e4f-154">**sent**</span><span class="sxs-lookup"><span data-stu-id="87e4f-154">**sent**</span></span>           | <span data-ttu-id="87e4f-155">发件人发送电子邮件的日期。</span><span class="sxs-lookup"><span data-stu-id="87e4f-155">The date that an email message was sent by the sender.</span></span>|<span data-ttu-id="87e4f-156">[GET][search-sent-example] `../me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`</span><span class="sxs-lookup"><span data-stu-id="87e4f-156">[GET][search-sent-example] `../me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`</span></span>
| <span data-ttu-id="87e4f-157">**size**</span><span class="sxs-lookup"><span data-stu-id="87e4f-157">**size**</span></span>           | <span data-ttu-id="87e4f-158">邮件大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="87e4f-158">The size of an item in bytes.</span></span>|<span data-ttu-id="87e4f-159">[GET][search-size-example] `../me/messages?$search="size:1..500000"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-159">[GET][search-size-example] `../me/messages?$search="size:1..500000"`</span></span>
| <span data-ttu-id="87e4f-160">**subject**</span><span class="sxs-lookup"><span data-stu-id="87e4f-160">**subject**</span></span>           | <span data-ttu-id="87e4f-p105">电子邮件主题行中的文本。</span><span class="sxs-lookup"><span data-stu-id="87e4f-p105">The text in the subject line of an email message. .</span></span>|<span data-ttu-id="87e4f-163">[GET][search-sbj-example] `../me/messages?$search="subject:has"&$select=subject`</span><span class="sxs-lookup"><span data-stu-id="87e4f-163">[GET][search-sbj-example] `../me/messages?$search="subject:has"&$select=subject`</span></span>
| <span data-ttu-id="87e4f-164">**to**</span><span class="sxs-lookup"><span data-stu-id="87e4f-164">**to**</span></span>           | <span data-ttu-id="87e4f-165">电子邮件的 **to** 字段，可指定为 SMTP 地址、显示名称或别名。</span><span class="sxs-lookup"><span data-stu-id="87e4f-165">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|<span data-ttu-id="87e4f-166">[GET][search-to-example]`.../me/messages?$search="to:randiw"&$select=subject,toRecipients`</span><span class="sxs-lookup"><span data-stu-id="87e4f-166">[GET][search-to-example]`.../me/messages?$search="to:randiw"&$select=subject,toRecipients`</span></span>


<span data-ttu-id="87e4f-167">若要详细了解 可搜索的电子邮件属性、KQL 语法、受支持的运算符和搜索技巧，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="87e4f-167">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="87e4f-168">[Exchange 中的可搜索属性](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。</span><span class="sxs-lookup"><span data-stu-id="87e4f-168">[Searchable properties in Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="87e4f-169">关键字查询语言 (KQL) 语法参考</span><span class="sxs-lookup"><span data-stu-id="87e4f-169">Keyword Query Language (KQL) syntax reference</span></span>](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [<span data-ttu-id="87e4f-170">Exchange 2016 中的就地电子数据展示的邮件属性和搜索运算符</span><span class="sxs-lookup"><span data-stu-id="87e4f-170">Message properties and search operators for In-Place eDiscovery in Exchange 2016</span></span>](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

## <a name="using-search-on-person-collections"></a><span data-ttu-id="87e4f-171">对 person 集合使用 $search</span><span class="sxs-lookup"><span data-stu-id="87e4f-171">Using $search on person collections</span></span>

<span data-ttu-id="87e4f-172">可以使用 Microsoft Graph [People API](/graph/api/resources/person) 检索与用户最相关的人员。</span><span class="sxs-lookup"><span data-stu-id="87e4f-172">You can use the Microsoft Graph [People API](/graph/api/resources/person) to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="87e4f-173">相关性由用户的通信和协作模式及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="87e4f-173">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="87e4f-174">People API 支持 `$search` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="87e4f-174">The People API supports the `$search` query parameter.</span></span> <span data-ttu-id="87e4f-175">`$search` 请求最多可返回 250 个结果。</span><span class="sxs-lookup"><span data-stu-id="87e4f-175">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="87e4f-176">人员搜索就是按 [person](/graph/api/resources/person) 资源的 **displayName** 和 **emailAddress** 属性进行搜索。</span><span class="sxs-lookup"><span data-stu-id="87e4f-176">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person) resource.</span></span>

<span data-ttu-id="87e4f-177">以下请求在已登录用户的 **人员** 集合中的每个人员的 **displayName** 和 **emailAddress** 属性中，为名为“Irene McGowen”的人员执行搜索。</span><span class="sxs-lookup"><span data-stu-id="87e4f-177">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="87e4f-178">由于一个名为“Irene McGowan”的人员与登录用户相关，因此返回了“Irene McGowan”的信息。</span><span class="sxs-lookup"><span data-stu-id="87e4f-178">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="87e4f-179">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="87e4f-179">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

<span data-ttu-id="87e4f-180">若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people-example.md#search-people)。</span><span class="sxs-lookup"><span data-stu-id="87e4f-180">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

## <a name="using-search-on-directory-object-collections"></a><span data-ttu-id="87e4f-181">在目录对象集合上使用 $search</span><span class="sxs-lookup"><span data-stu-id="87e4f-181">Using $search on directory object collections</span></span>

<span data-ttu-id="87e4f-182">派生自 [directoryObject](/graph/api/resources/directoryobject) 的 Azure AD 资源及其关系仅在高级查询中支持 `$search` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="87e4f-182">Azure AD resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject) support the `$search` query parameter only in advanced queries.</span></span> <span data-ttu-id="87e4f-183">使用标记化方法的搜索的工作原理是提取输入和输出字符串中的单词，并使用空格、数字、不同的大小写和符号分隔这些词，如下所示:</span><span class="sxs-lookup"><span data-stu-id="87e4f-183">The search uses a tokenization approach which works by extracting words from your input and output string, using spaces, numbers, different casing, and symbols to separate the words, as follows:</span></span>

* <span data-ttu-id="87e4f-184">**空格**：`hello world` => `hello`、 `world`</span><span class="sxs-lookup"><span data-stu-id="87e4f-184">**Spaces**: `hello world` => `hello`, `world`</span></span>
* <span data-ttu-id="87e4f-185">**不同的大小写**⁽¹⁾：`HelloWorld` 或 `helloWORLD` => `hello`、`world`</span><span class="sxs-lookup"><span data-stu-id="87e4f-185">**Different casing**⁽¹⁾: `HelloWorld` or `helloWORLD` => `hello`, `world`</span></span>
* <span data-ttu-id="87e4f-186">**符号**⁽⁾：`hello.world` => `hello`、`.`、`world`， `helloworld`</span><span class="sxs-lookup"><span data-stu-id="87e4f-186">**Symbols**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`</span></span>
* <span data-ttu-id="87e4f-187">**数字**：`hello123world` => `hello`、`123`、 `world`</span><span class="sxs-lookup"><span data-stu-id="87e4f-187">**Numbers**: `hello123world` => `hello`, `123`, `world`</span></span>

<span data-ttu-id="87e4f-188">⁽¹⁾ 目前，标记化仅在大小写从小写转换为大写时才有效，因此 `HELLOworld` 被视为一个标记：`helloworld`，`HelloWORld` 是两个标记：`hello`、`world`。</span><span class="sxs-lookup"><span data-stu-id="87e4f-188">⁽¹⁾ Currently, tokenization only works when the casing is changing from lowercase to uppercase, so `HELLOworld` is considered a single token: `helloworld`, and `HelloWORld` is two tokens: `hello`, `world`.</span></span> <span data-ttu-id="87e4f-189">⁽²⁾ 标记化逻辑还会合并仅由符号分隔的单词；例如，搜索 `helloworld` 将找到 `hello-world` 和 `hello.world`。</span><span class="sxs-lookup"><span data-stu-id="87e4f-189">⁽²⁾ Tokenization logic also combines words that are separated only by symbols; for example, searching for `helloworld` will find `hello-world` and `hello.world`.</span></span>

> <span data-ttu-id="87e4f-190">**注意**：标记化后，标记将独立于原始大小写进行匹配，并且将以任何顺序匹配。</span><span class="sxs-lookup"><span data-stu-id="87e4f-190">**Note**: after tokenization, the tokens are matched independently of the original casing, and they are matched in any order.</span></span>

<span data-ttu-id="87e4f-191">标记化搜索仅适用于 **displayName** 和 **description** 字段。</span><span class="sxs-lookup"><span data-stu-id="87e4f-191">The tokenized search support works only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="87e4f-192">字符串类型的任何字段都可以放入 `$search`; **displayName** 和 **说明之外的字段** 默认为 `$filter` `startswith` 行为。</span><span class="sxs-lookup"><span data-stu-id="87e4f-192">Any field of String type can be put in `$search`; fields other than **displayName** and **description** default to `$filter` `startswith` behavior.</span></span> <span data-ttu-id="87e4f-193">例如：</span><span class="sxs-lookup"><span data-stu-id="87e4f-193">For example:</span></span>

`https://graph.microsoft.com/v1.0/groups/?$search="displayName:OneVideo"`

<span data-ttu-id="87e4f-194">这将查找显示名称看起来像 "OneVideo" 的所有组。</span><span class="sxs-lookup"><span data-stu-id="87e4f-194">This looks for all groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="87e4f-195">也可与`$search`配合使用`$filter`。</span><span class="sxs-lookup"><span data-stu-id="87e4f-195">`$search` can be used together with `$filter` as well.</span></span> <span data-ttu-id="87e4f-196">例如：</span><span class="sxs-lookup"><span data-stu-id="87e4f-196">For example:</span></span>

`https://graph.microsoft.com/v1.0/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

<span data-ttu-id="87e4f-197">这将查找显示名称类似于“OneVideo”的所有启用邮件的组。</span><span class="sxs-lookup"><span data-stu-id="87e4f-197">This looks for all mail-enabled groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="87e4f-198">结果是根据逻辑结合（"AND"）和`$filter`整个查询`$search`来限制。</span><span class="sxs-lookup"><span data-stu-id="87e4f-198">The results are restricted based on a logical conjunction (an "AND") of the `$filter` and the entire query in the `$search`.</span></span> <span data-ttu-id="87e4f-199">搜索文本基于大小写进行标记，但是匹配以不区分大小写的方式执行。</span><span class="sxs-lookup"><span data-stu-id="87e4f-199">The search text is tokenized based on casing, but matches are performed in a case-insensitive manner.</span></span> <span data-ttu-id="87e4f-200">例如，“OneVideo”将被分割成两个输入标记“one”和“video”，但是匹配不区分大小写的属性。</span><span class="sxs-lookup"><span data-stu-id="87e4f-200">For example, "OneVideo" would be split into two input tokens "one" and "video", but matches properties insensitive to case.</span></span>

<span data-ttu-id="87e4f-201">搜索的语法遵循以下规则：</span><span class="sxs-lookup"><span data-stu-id="87e4f-201">The syntax of search follows these rules:</span></span>

* <span data-ttu-id="87e4f-202">通用格式：$search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span><span class="sxs-lookup"><span data-stu-id="87e4f-202">Generic format: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span></span>
* <span data-ttu-id="87e4f-203">支持任何子句。</span><span class="sxs-lookup"><span data-stu-id="87e4f-203">Any number of clauses is supported.</span></span> <span data-ttu-id="87e4f-204">支持适用于优先级的括号。</span><span class="sxs-lookup"><span data-stu-id="87e4f-204">Parentheses for precedence is also supported.</span></span>
* <span data-ttu-id="87e4f-205">每个子句的语法是："\<property>:\<text to search>"。</span><span class="sxs-lookup"><span data-stu-id="87e4f-205">The syntax for each clause is: "\<property>:\<text to search>".</span></span>
* <span data-ttu-id="87e4f-206">必须在子句中指定属性名称。</span><span class="sxs-lookup"><span data-stu-id="87e4f-206">The property name must be specified in the clause.</span></span> <span data-ttu-id="87e4f-207">可以在中使用的任何属性`$filter`也可以在内使用 `$search`。</span><span class="sxs-lookup"><span data-stu-id="87e4f-207">Any property that can be used in `$filter` can also be used inside `$search`.</span></span> <span data-ttu-id="87e4f-208">根据属性的不同，如果属性不支持搜索，那么搜索行为要么是“search”，要么是“start with”。</span><span class="sxs-lookup"><span data-stu-id="87e4f-208">Depending on the property, the search behavior is either "search" or "startswith" if search is not supported on the property.</span></span>
* <span data-ttu-id="87e4f-209">必须将完整子句部分置于双引号内。</span><span class="sxs-lookup"><span data-stu-id="87e4f-209">The whole clause part must be put inside double quotes.</span></span>
* <span data-ttu-id="87e4f-210">必须将逻辑运算符 "AND" 和 "OR" 置于双引号之外。</span><span class="sxs-lookup"><span data-stu-id="87e4f-210">Logical operator 'AND' 'OR' must be put outside double quotes.</span></span> <span data-ttu-id="87e4f-211">它们必须处于大写形式。</span><span class="sxs-lookup"><span data-stu-id="87e4f-211">They must be in upper case.</span></span>
* <span data-ttu-id="87e4f-p116">考虑到整个子句部分需要放在双引号内，如果包含双引号和反斜杠，则需要使用反斜杠对其进行转义。其他字符不需要进行转义。</span><span class="sxs-lookup"><span data-stu-id="87e4f-p116">Given that the whole clause part needs to be put inside double quotes, if it contains double quote and backslash, it needs to be escaped with a backslash. No other characters need to be escaped.</span></span>

<span data-ttu-id="87e4f-214">下表显示了一些示例。</span><span class="sxs-lookup"><span data-stu-id="87e4f-214">The following table shows some examples.</span></span>

| <span data-ttu-id="87e4f-215">对象类</span><span class="sxs-lookup"><span data-stu-id="87e4f-215">Object class</span></span> | <span data-ttu-id="87e4f-216">说明</span><span class="sxs-lookup"><span data-stu-id="87e4f-216">Description</span></span> | <span data-ttu-id="87e4f-217">示例</span><span class="sxs-lookup"><span data-stu-id="87e4f-217">Example</span></span> |
| ------------ | ----------- | ------- |
| <span data-ttu-id="87e4f-218">用户</span><span class="sxs-lookup"><span data-stu-id="87e4f-218">User</span></span> | <span data-ttu-id="87e4f-219">通讯簿显示用户的名称。</span><span class="sxs-lookup"><span data-stu-id="87e4f-219">Address book display name of the user.</span></span> | <span data-ttu-id="87e4f-220">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-220">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr"`</span></span>  |
| <span data-ttu-id="87e4f-221">用户</span><span class="sxs-lookup"><span data-stu-id="87e4f-221">User</span></span> | <span data-ttu-id="87e4f-222">通讯簿显示用户的名称或邮件。</span><span class="sxs-lookup"><span data-stu-id="87e4f-222">Address book display name or mail of the user.</span></span> | <span data-ttu-id="87e4f-223">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr" OR "mail:Guthr"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-223">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr" OR "mail:Guthr"`</span></span> |
| <span data-ttu-id="87e4f-224">Group</span><span class="sxs-lookup"><span data-stu-id="87e4f-224">Group</span></span> | <span data-ttu-id="87e4f-225">通讯簿显群组的名称或说明。</span><span class="sxs-lookup"><span data-stu-id="87e4f-225">Address book display name or description of the group.</span></span> | <span data-ttu-id="87e4f-226">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-226">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive"`</span></span> |
| <span data-ttu-id="87e4f-227">Group</span><span class="sxs-lookup"><span data-stu-id="87e4f-227">Group</span></span> | <span data-ttu-id="87e4f-228">通讯簿在启用邮件组上显示名称。</span><span class="sxs-lookup"><span data-stu-id="87e4f-228">Address book display name on a mail-enabled group.</span></span> | <span data-ttu-id="87e4f-229">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"`</span><span class="sxs-lookup"><span data-stu-id="87e4f-229">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"`</span></span> |


<span data-ttu-id="87e4f-230">你在 `$search` 中提供的字符串输入以及可搜索属性都按空格、不同的大小写和字符类型（数字和特殊字符）划分为多个部分。</span><span class="sxs-lookup"><span data-stu-id="87e4f-230">Both the string inputs you provide in `$search`, as well as the searchable properties, are split up into parts by spaces, different casing, and character types (numbers and special characters).</span></span>

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

## <a name="see-also"></a><span data-ttu-id="87e4f-231">另请参阅</span><span class="sxs-lookup"><span data-stu-id="87e4f-231">See also</span></span>

- [<span data-ttu-id="87e4f-232">使用查询参数自定义响应</span><span class="sxs-lookup"><span data-stu-id="87e4f-232">Use query parameters to customize responses</span></span>](/graph/query-parameters)
- [<span data-ttu-id="87e4f-233">Azure AD 目录对象的高级查询功能</span><span class="sxs-lookup"><span data-stu-id="87e4f-233">Advanced query capabilities on Azure AD directory objects</span></span>](/graph/aad-advanced-queries)
- [<span data-ttu-id="87e4f-234">查询参数限制</span><span class="sxs-lookup"><span data-stu-id="87e4f-234">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
