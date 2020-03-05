---
title: 配置文件资源类型
description: 表示为用户描述的属性，以及通过 microsoft Graph 在 Microsoft 365 和第三方服务和体验中呈现的共享人员体验。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c5c7d7765d546dad5f6de39f72f092b3bf9daee6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521465"
---
# <a name="profile-resource-type"></a><span data-ttu-id="4a545-103">配置文件资源类型</span><span class="sxs-lookup"><span data-stu-id="4a545-103">profile resource type</span></span>

<span data-ttu-id="4a545-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4a545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a545-105">表示租户中人员的描述性属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-105">Represents descriptive properties of a person in a tenant.</span></span> <span data-ttu-id="4a545-106">这些属性在跨 Microsoft 365 和第三方服务的共享人员体验和通过 Microsoft Graph 的体验中呈现。</span><span class="sxs-lookup"><span data-stu-id="4a545-106">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

## <a name="methods"></a><span data-ttu-id="4a545-107">方法</span><span class="sxs-lookup"><span data-stu-id="4a545-107">Methods</span></span>

| <span data-ttu-id="4a545-108">方法</span><span class="sxs-lookup"><span data-stu-id="4a545-108">Method</span></span>                                                                     | <span data-ttu-id="4a545-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a545-109">Return Type</span></span>                                                    | <span data-ttu-id="4a545-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a545-110">Description</span></span>                                                                          |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------|
| [<span data-ttu-id="4a545-111">获取个人资料</span><span class="sxs-lookup"><span data-stu-id="4a545-111">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="4a545-112">profile</span><span class="sxs-lookup"><span data-stu-id="4a545-112">profile</span></span>](profile.md)                                          | <span data-ttu-id="4a545-113">读取 profile 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a545-113">Read properties and relationships of profile object.</span></span>                                 |
| [<span data-ttu-id="4a545-114">删除个人资料</span><span class="sxs-lookup"><span data-stu-id="4a545-114">Delete profile</span></span>](../api/profile-delete.md)                                         | <span data-ttu-id="4a545-115">无</span><span class="sxs-lookup"><span data-stu-id="4a545-115">None</span></span>                                                           | <span data-ttu-id="4a545-116">删除**配置文件**对象。</span><span class="sxs-lookup"><span data-stu-id="4a545-116">Delete a **profile** object.</span></span>                                                               |
| [<span data-ttu-id="4a545-117">列表帐户</span><span class="sxs-lookup"><span data-stu-id="4a545-117">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="4a545-118">[userAccountInformation](useraccountinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-118">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="4a545-119">获取**userAccountInformation**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-119">Get a **userAccountInformation** object collection.</span></span>                                      |
| [<span data-ttu-id="4a545-120">创建 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="4a545-120">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="4a545-121">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="4a545-121">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="4a545-122">通过发布到周年纪念集合创建新的**personAnniversary** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-122">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>           |
| [<span data-ttu-id="4a545-123">列出周年纪念</span><span class="sxs-lookup"><span data-stu-id="4a545-123">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="4a545-124">[personAnniversary](personanniversary.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-124">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="4a545-125">获取**personAnniversary**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-125">Get a **personAnniversary** object collection.</span></span>                                           |
| [<span data-ttu-id="4a545-126">创建 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="4a545-126">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="4a545-127">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="4a545-127">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="4a545-128">通过发布到**educationalActivities**集合创建新的**educationalActivity** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-128">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="4a545-129">列出 educationalActivities</span><span class="sxs-lookup"><span data-stu-id="4a545-129">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="4a545-130">[educationalActivity](educationalactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-130">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="4a545-131">获取**educationalActivity**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-131">Get an **educationalActivity** object collection.</span></span>                                         |
| [<span data-ttu-id="4a545-132">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="4a545-132">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="4a545-133">itemEmail</span><span class="sxs-lookup"><span data-stu-id="4a545-133">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="4a545-134">通过发布到电子邮件集合创建新的**itemEmail** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-134">Create a new **itemEmail** by posting to the emails collection.</span></span>                          |
| [<span data-ttu-id="4a545-135">列出电子邮件</span><span class="sxs-lookup"><span data-stu-id="4a545-135">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="4a545-136">[itemEmail](itememail.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-136">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="4a545-137">获取**itemEmail**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-137">Get an **itemEmail** object collection.</span></span>                                                   |
| [<span data-ttu-id="4a545-138">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="4a545-138">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="4a545-139">personInterest</span><span class="sxs-lookup"><span data-stu-id="4a545-139">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="4a545-140">通过发布到 "兴趣" 集合创建新的**personInterest** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-140">Create a new **personInterest** by posting to the interests collection.</span></span>                  |
| [<span data-ttu-id="4a545-141">列出兴趣</span><span class="sxs-lookup"><span data-stu-id="4a545-141">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="4a545-142">[personInterest](personinterest.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-142">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="4a545-143">获取**personInterest**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-143">Get a **personInterest** object collection.</span></span>                                              |
| [<span data-ttu-id="4a545-144">创建 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="4a545-144">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="4a545-145">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="4a545-145">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="4a545-146">通过发布到语言集合创建新的**languageProficiency** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-146">Create a new **languageProficiency** by posting to the languages collection.</span></span>             |
| [<span data-ttu-id="4a545-147">列出语言</span><span class="sxs-lookup"><span data-stu-id="4a545-147">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="4a545-148">[languageProficiency](languageproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-148">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="4a545-149">获取**languageProficiency**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-149">Get a **languageProficiency** object collection.</span></span>                                         |
| [<span data-ttu-id="4a545-150">列出名称</span><span class="sxs-lookup"><span data-stu-id="4a545-150">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="4a545-151">[contact.personname](personname.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-151">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="4a545-152">获取**contact.personname**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-152">Get a **personName** object collection.</span></span>                                                  |
| [<span data-ttu-id="4a545-153">创建 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="4a545-153">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="4a545-154">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="4a545-154">personName</span></span>](personName.md)                                    | <span data-ttu-id="4a545-155">通过发布到名称集合创建新的**contact.personname**对象。</span><span class="sxs-lookup"><span data-stu-id="4a545-155">Create a new **personName** object by posting to the names collection.</span></span>                   |
| [<span data-ttu-id="4a545-156">列出网站</span><span class="sxs-lookup"><span data-stu-id="4a545-156">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="4a545-157">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-157">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="4a545-158">获取**personWebsite**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-158">Get a **personWebsite** object collection.</span></span>                                               |
| [<span data-ttu-id="4a545-159">创建 itemPhone</span><span class="sxs-lookup"><span data-stu-id="4a545-159">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="4a545-160">itemPhone</span><span class="sxs-lookup"><span data-stu-id="4a545-160">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="4a545-161">通过发布到 "电话" 集合创建新的 itemPhone。</span><span class="sxs-lookup"><span data-stu-id="4a545-161">Create a new itemPhone by posting to the phones collection.</span></span>                          |
| [<span data-ttu-id="4a545-162">列出电话</span><span class="sxs-lookup"><span data-stu-id="4a545-162">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="4a545-163">[itemPhone](itemphone.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-163">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="4a545-164">获取**itemPhone**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-164">Get a **itemPhone** object collection.</span></span>                                                   |
| [<span data-ttu-id="4a545-165">创建 workPosition</span><span class="sxs-lookup"><span data-stu-id="4a545-165">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="4a545-166">workPosition</span><span class="sxs-lookup"><span data-stu-id="4a545-166">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="4a545-167">通过发布到 "职位" 集合创建新的 workPosition。</span><span class="sxs-lookup"><span data-stu-id="4a545-167">Create a new workPosition by posting to the positions collection.</span></span>                    |
| [<span data-ttu-id="4a545-168">列表位置</span><span class="sxs-lookup"><span data-stu-id="4a545-168">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="4a545-169">[workPosition](workposition.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-169">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="4a545-170">获取**workPosition**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-170">Get a **workPosition** object collection.</span></span>                                                |
| [<span data-ttu-id="4a545-171">创建 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4a545-171">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="4a545-172">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4a545-172">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="4a545-173">通过发布到项目集合创建新的**projectParticipation** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-173">Create a new **projectParticipation** by posting to the projects collection.</span></span>             |
| [<span data-ttu-id="4a545-174">列出项目</span><span class="sxs-lookup"><span data-stu-id="4a545-174">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="4a545-175">[projectParticipation](projectparticipation.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-175">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="4a545-176">获取**projectParticipation**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-176">Get a **projectParticipation** object collection.</span></span>                                        |
| [<span data-ttu-id="4a545-177">创建 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="4a545-177">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="4a545-178">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="4a545-178">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="4a545-179">通过发布到技能集合创建新的**skillProficiency** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-179">Create a new **skillProficiency** by posting to the skills collection.</span></span>                   |
| [<span data-ttu-id="4a545-180">列表技能</span><span class="sxs-lookup"><span data-stu-id="4a545-180">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="4a545-181">[skillProficiency](skillproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-181">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="4a545-182">获取**skillProficiency**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-182">Get a **skillProficiency** object collection.</span></span>                                            |
| [<span data-ttu-id="4a545-183">创建 webAccount</span><span class="sxs-lookup"><span data-stu-id="4a545-183">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="4a545-184">webAccount</span><span class="sxs-lookup"><span data-stu-id="4a545-184">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="4a545-185">通过发布到 webAccounts 集合创建新的**webAccount** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-185">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                    |
| [<span data-ttu-id="4a545-186">列出 webAccounts</span><span class="sxs-lookup"><span data-stu-id="4a545-186">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="4a545-187">[webAccount](webaccount.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-187">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="4a545-188">获取**webAccount**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-188">Get a **webAccount** object collection.</span></span>                                                  |
| [<span data-ttu-id="4a545-189">创建 personWebsite</span><span class="sxs-lookup"><span data-stu-id="4a545-189">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="4a545-190">personWebsite</span><span class="sxs-lookup"><span data-stu-id="4a545-190">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="4a545-191">通过发布到网站集创建新的**personWebsite** 。</span><span class="sxs-lookup"><span data-stu-id="4a545-191">Create a new **personWebsite** by posting to the websites collection.</span></span>                    |
| [<span data-ttu-id="4a545-192">列出网站</span><span class="sxs-lookup"><span data-stu-id="4a545-192">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="4a545-193">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-193">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="4a545-194">获取**personWebsite**对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a545-194">Get a **personWebsite** object collection.</span></span>                                               |

## <a name="properties"></a><span data-ttu-id="4a545-195">属性</span><span class="sxs-lookup"><span data-stu-id="4a545-195">Properties</span></span>

| <span data-ttu-id="4a545-196">属性</span><span class="sxs-lookup"><span data-stu-id="4a545-196">Property</span></span>     | <span data-ttu-id="4a545-197">类型</span><span class="sxs-lookup"><span data-stu-id="4a545-197">Type</span></span>        | <span data-ttu-id="4a545-198">说明</span><span class="sxs-lookup"><span data-stu-id="4a545-198">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a545-199">id</span><span class="sxs-lookup"><span data-stu-id="4a545-199">id</span></span>            |<span data-ttu-id="4a545-200">String</span><span class="sxs-lookup"><span data-stu-id="4a545-200">String</span></span>       | <span data-ttu-id="4a545-201">只读。</span><span class="sxs-lookup"><span data-stu-id="4a545-201">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="4a545-202">关系</span><span class="sxs-lookup"><span data-stu-id="4a545-202">Relationships</span></span>

| <span data-ttu-id="4a545-203">关系</span><span class="sxs-lookup"><span data-stu-id="4a545-203">Relationship</span></span>          | <span data-ttu-id="4a545-204">类型</span><span class="sxs-lookup"><span data-stu-id="4a545-204">Type</span></span>                                                         | <span data-ttu-id="4a545-205">说明</span><span class="sxs-lookup"><span data-stu-id="4a545-205">Description</span></span>         |
|:----------------------|:-------------------------------------------------------------|:--------------------|
|<span data-ttu-id="4a545-206">上级</span><span class="sxs-lookup"><span data-stu-id="4a545-206">account</span></span>                |<span data-ttu-id="4a545-207">[userAccountInformation](useraccountinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-207">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="4a545-208">表示特定绑定到用户帐户的信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-208">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="4a545-209">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-209">Read-only.</span></span> <span data-ttu-id="4a545-210">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-210">Nullable.</span></span>|
|<span data-ttu-id="4a545-211">周年</span><span class="sxs-lookup"><span data-stu-id="4a545-211">anniversaries</span></span>          |<span data-ttu-id="4a545-212">[personAnniversary](personanniversary.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-212">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="4a545-213">代表与人员关联的有意义的日期的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-213">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="4a545-214">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-214">Read-only.</span></span> <span data-ttu-id="4a545-215">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-215">Nullable.</span></span>|
|<span data-ttu-id="4a545-216">educationalActivities</span><span class="sxs-lookup"><span data-stu-id="4a545-216">educationalActivities</span></span>  |<span data-ttu-id="4a545-217">[educationalActivity](educationalactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-217">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="4a545-218">表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。</span><span class="sxs-lookup"><span data-stu-id="4a545-218">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="4a545-219">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-219">Read-only.</span></span> <span data-ttu-id="4a545-220">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-220">Nullable.</span></span>|
|<span data-ttu-id="4a545-221">电子邮件</span><span class="sxs-lookup"><span data-stu-id="4a545-221">emails</span></span>                 |<span data-ttu-id="4a545-222">[itemEmail](itememail.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-222">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="4a545-223">表示有关与用户相关联的电子邮件地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-223">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="4a545-224">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-224">Read-only.</span></span> <span data-ttu-id="4a545-225">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-225">Nullable.</span></span>|
|<span data-ttu-id="4a545-226">interests</span><span class="sxs-lookup"><span data-stu-id="4a545-226">interests</span></span>              |<span data-ttu-id="4a545-227">[personInterest](personinterest.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-227">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="4a545-228">提供有关用户在各种服务中与其自身关联的兴趣的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-228">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="4a545-229">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-229">Read-only.</span></span> <span data-ttu-id="4a545-230">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-230">Nullable.</span></span>|
|<span data-ttu-id="4a545-231">languages</span><span class="sxs-lookup"><span data-stu-id="4a545-231">languages</span></span>              |<span data-ttu-id="4a545-232">[languageProficiency](languageproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-232">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="4a545-233">表示有关用户已添加到其配置文件中的语言的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-233">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="4a545-234">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-234">Read-only.</span></span> <span data-ttu-id="4a545-235">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-235">Nullable.</span></span>|
|<span data-ttu-id="4a545-236">phones</span><span class="sxs-lookup"><span data-stu-id="4a545-236">phones</span></span>                 |<span data-ttu-id="4a545-237">[itemPhone](itemphone.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-237">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="4a545-238">表示有关与各种服务中的用户关联的电话号码的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-238">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="4a545-239">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-239">Read-only.</span></span> <span data-ttu-id="4a545-240">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-240">Nullable.</span></span>|
|<span data-ttu-id="4a545-241">位置</span><span class="sxs-lookup"><span data-stu-id="4a545-241">positions</span></span>              |<span data-ttu-id="4a545-242">[workPosition](workposition.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-242">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="4a545-243">表示有关与用户配置文件相关联的工作职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-243">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="4a545-244">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-244">Read-only.</span></span> <span data-ttu-id="4a545-245">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-245">Nullable.</span></span>|
|<span data-ttu-id="4a545-246">projects</span><span class="sxs-lookup"><span data-stu-id="4a545-246">projects</span></span>               |<span data-ttu-id="4a545-247">[projectParticipation](projectparticipation.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-247">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="4a545-248">表示有关与用户关联的项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-248">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="4a545-249">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-249">Read-only.</span></span> <span data-ttu-id="4a545-250">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-250">Nullable.</span></span>|
|<span data-ttu-id="4a545-251">skills</span><span class="sxs-lookup"><span data-stu-id="4a545-251">skills</span></span>                 |<span data-ttu-id="4a545-252">[skillProficiency](skillproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-252">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="4a545-253">表示有关与各种服务中的用户相关的技能的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-253">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="4a545-254">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-254">Read-only.</span></span> <span data-ttu-id="4a545-255">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-255">Nullable.</span></span>|
|<span data-ttu-id="4a545-256">webAccounts</span><span class="sxs-lookup"><span data-stu-id="4a545-256">webAccounts</span></span>            |<span data-ttu-id="4a545-257">[webAccount](webaccount.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-257">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="4a545-258">表示用户已将其添加到其用户配置文件中的 web 帐户。</span><span class="sxs-lookup"><span data-stu-id="4a545-258">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="4a545-259">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-259">Read-only.</span></span> <span data-ttu-id="4a545-260">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4a545-260">Nullable.</span></span>|
|<span data-ttu-id="4a545-261">websites</span><span class="sxs-lookup"><span data-stu-id="4a545-261">websites</span></span>               |<span data-ttu-id="4a545-262">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a545-262">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="4a545-263">表示有关与各种服务中的用户相关联的网站的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a545-263">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="4a545-264">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="4a545-264">Read-only.</span></span> <span data-ttu-id="4a545-265">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4a545-265">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a545-266">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a545-266">JSON representation</span></span>

<span data-ttu-id="4a545-267">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a545-267">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
