---
title: 配置文件资源类型
description: 表示为用户描述的属性，以及通过 microsoft Graph 在 Microsoft 365 和第三方服务和体验中呈现的共享人员体验。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 367a2c556b560056bcab44e6c20ae7851e493e48
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950477"
---
# <a name="profile-resource-type"></a><span data-ttu-id="8c092-103">配置文件资源类型</span><span class="sxs-lookup"><span data-stu-id="8c092-103">profile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c092-104">表示租户中人员的描述性属性。</span><span class="sxs-lookup"><span data-stu-id="8c092-104">Represents descriptive properties of a person in a tenant.</span></span> <span data-ttu-id="8c092-105">这些属性在跨 Microsoft 365 和第三方服务的共享人员体验和通过 Microsoft Graph 的体验中呈现。</span><span class="sxs-lookup"><span data-stu-id="8c092-105">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

## <a name="methods"></a><span data-ttu-id="8c092-106">方法</span><span class="sxs-lookup"><span data-stu-id="8c092-106">Methods</span></span>

| <span data-ttu-id="8c092-107">方法</span><span class="sxs-lookup"><span data-stu-id="8c092-107">Method</span></span>                                                                     | <span data-ttu-id="8c092-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c092-108">Return Type</span></span>                                                    | <span data-ttu-id="8c092-109">说明</span><span class="sxs-lookup"><span data-stu-id="8c092-109">Description</span></span>                                                                          |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------|
| [<span data-ttu-id="8c092-110">获取配置文件</span><span class="sxs-lookup"><span data-stu-id="8c092-110">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="8c092-111">profile</span><span class="sxs-lookup"><span data-stu-id="8c092-111">profile</span></span>](profile.md)                                          | <span data-ttu-id="8c092-112">读取 profile 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8c092-112">Read properties and relationships of profile object.</span></span>                                 |
| [<span data-ttu-id="8c092-113">删除配置文件</span><span class="sxs-lookup"><span data-stu-id="8c092-113">Delete profile</span></span>](../api/profile-delete.md)                                         | <span data-ttu-id="8c092-114">无</span><span class="sxs-lookup"><span data-stu-id="8c092-114">None</span></span>                                                           | <span data-ttu-id="8c092-115">删除**配置文件**对象。</span><span class="sxs-lookup"><span data-stu-id="8c092-115">Delete a **profile** object.</span></span>                                                               |
| [<span data-ttu-id="8c092-116">列表帐户</span><span class="sxs-lookup"><span data-stu-id="8c092-116">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="8c092-117">[userAccountInformation](useraccountinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-117">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="8c092-118">获取**userAccountInformation**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-118">Get a **userAccountInformation** object collection.</span></span>                                      |
| [<span data-ttu-id="8c092-119">创建 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="8c092-119">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="8c092-120">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="8c092-120">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="8c092-121">通过发布到周年纪念集合创建新的**personAnniversary** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-121">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>           |
| [<span data-ttu-id="8c092-122">列出周年纪念</span><span class="sxs-lookup"><span data-stu-id="8c092-122">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="8c092-123">[personAnniversary](personanniversary.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-123">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="8c092-124">获取**personAnniversary**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-124">Get a **personAnniversary** object collection.</span></span>                                           |
| [<span data-ttu-id="8c092-125">创建 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="8c092-125">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="8c092-126">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="8c092-126">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="8c092-127">通过发布到**educationalActivities**集合创建新的**educationalActivity** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-127">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="8c092-128">列出 educationalActivities</span><span class="sxs-lookup"><span data-stu-id="8c092-128">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="8c092-129">[educationalActivity](educationalactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-129">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="8c092-130">获取**educationalActivity**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-130">Get an **educationalActivity** object collection.</span></span>                                         |
| [<span data-ttu-id="8c092-131">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="8c092-131">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="8c092-132">itemEmail</span><span class="sxs-lookup"><span data-stu-id="8c092-132">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="8c092-133">通过发布到电子邮件集合创建新的**itemEmail** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-133">Create a new **itemEmail** by posting to the emails collection.</span></span>                          |
| [<span data-ttu-id="8c092-134">列出电子邮件</span><span class="sxs-lookup"><span data-stu-id="8c092-134">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="8c092-135">[itemEmail](itememail.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-135">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="8c092-136">获取**itemEmail**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-136">Get an **itemEmail** object collection.</span></span>                                                   |
| [<span data-ttu-id="8c092-137">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="8c092-137">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="8c092-138">personInterest</span><span class="sxs-lookup"><span data-stu-id="8c092-138">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="8c092-139">通过发布到 "兴趣" 集合创建新的**personInterest** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-139">Create a new **personInterest** by posting to the interests collection.</span></span>                  |
| [<span data-ttu-id="8c092-140">列出兴趣</span><span class="sxs-lookup"><span data-stu-id="8c092-140">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="8c092-141">[personInterest](personinterest.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-141">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="8c092-142">获取**personInterest**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-142">Get a **personInterest** object collection.</span></span>                                              |
| [<span data-ttu-id="8c092-143">创建 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="8c092-143">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="8c092-144">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="8c092-144">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="8c092-145">通过发布到语言集合创建新的**languageProficiency** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-145">Create a new **languageProficiency** by posting to the languages collection.</span></span>             |
| [<span data-ttu-id="8c092-146">列出语言</span><span class="sxs-lookup"><span data-stu-id="8c092-146">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="8c092-147">[languageProficiency](languageproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-147">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="8c092-148">获取**languageProficiency**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-148">Get a **languageProficiency** object collection.</span></span>                                         |
| [<span data-ttu-id="8c092-149">列出名称</span><span class="sxs-lookup"><span data-stu-id="8c092-149">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="8c092-150">[contact.personname](personname.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-150">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="8c092-151">获取**contact.personname**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-151">Get a **personName** object collection.</span></span>                                                  |
| [<span data-ttu-id="8c092-152">创建 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="8c092-152">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="8c092-153">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="8c092-153">personName</span></span>](personName.md)                                    | <span data-ttu-id="8c092-154">通过发布到名称集合创建新的**contact.personname**对象。</span><span class="sxs-lookup"><span data-stu-id="8c092-154">Create a new **personName** object by posting to the names collection.</span></span>                   |
| [<span data-ttu-id="8c092-155">列出网站</span><span class="sxs-lookup"><span data-stu-id="8c092-155">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="8c092-156">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-156">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="8c092-157">获取**personWebsite**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-157">Get a **personWebsite** object collection.</span></span>                                               |
| [<span data-ttu-id="8c092-158">创建 itemPhone</span><span class="sxs-lookup"><span data-stu-id="8c092-158">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="8c092-159">itemPhone</span><span class="sxs-lookup"><span data-stu-id="8c092-159">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="8c092-160">通过发布到 "电话" 集合创建新的 itemPhone。</span><span class="sxs-lookup"><span data-stu-id="8c092-160">Create a new itemPhone by posting to the phones collection.</span></span>                          |
| [<span data-ttu-id="8c092-161">列出电话</span><span class="sxs-lookup"><span data-stu-id="8c092-161">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="8c092-162">[itemPhone](itemphone.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-162">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="8c092-163">获取**itemPhone**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-163">Get a **itemPhone** object collection.</span></span>                                                   |
| [<span data-ttu-id="8c092-164">创建 workPosition</span><span class="sxs-lookup"><span data-stu-id="8c092-164">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="8c092-165">workPosition</span><span class="sxs-lookup"><span data-stu-id="8c092-165">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="8c092-166">通过发布到 "职位" 集合创建新的 workPosition。</span><span class="sxs-lookup"><span data-stu-id="8c092-166">Create a new workPosition by posting to the positions collection.</span></span>                    |
| [<span data-ttu-id="8c092-167">列表位置</span><span class="sxs-lookup"><span data-stu-id="8c092-167">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="8c092-168">[workPosition](workposition.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-168">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="8c092-169">获取**workPosition**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-169">Get a **workPosition** object collection.</span></span>                                                |
| [<span data-ttu-id="8c092-170">创建 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="8c092-170">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="8c092-171">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="8c092-171">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="8c092-172">通过发布到项目集合创建新的**projectParticipation** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-172">Create a new **projectParticipation** by posting to the projects collection.</span></span>             |
| [<span data-ttu-id="8c092-173">列出项目</span><span class="sxs-lookup"><span data-stu-id="8c092-173">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="8c092-174">[projectParticipation](projectparticipation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-174">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="8c092-175">获取**projectParticipation**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-175">Get a **projectParticipation** object collection.</span></span>                                        |
| [<span data-ttu-id="8c092-176">创建 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="8c092-176">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="8c092-177">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="8c092-177">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="8c092-178">通过发布到技能集合创建新的**skillProficiency** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-178">Create a new **skillProficiency** by posting to the skills collection.</span></span>                   |
| [<span data-ttu-id="8c092-179">列表技能</span><span class="sxs-lookup"><span data-stu-id="8c092-179">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="8c092-180">[skillProficiency](skillproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-180">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="8c092-181">获取**skillProficiency**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-181">Get a **skillProficiency** object collection.</span></span>                                            |
| [<span data-ttu-id="8c092-182">创建 webAccount</span><span class="sxs-lookup"><span data-stu-id="8c092-182">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="8c092-183">webAccount</span><span class="sxs-lookup"><span data-stu-id="8c092-183">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="8c092-184">通过发布到 webAccounts 集合创建新的**webAccount** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-184">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                    |
| [<span data-ttu-id="8c092-185">列出 webAccounts</span><span class="sxs-lookup"><span data-stu-id="8c092-185">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="8c092-186">[webAccount](webaccount.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-186">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="8c092-187">获取**webAccount**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-187">Get a **webAccount** object collection.</span></span>                                                  |
| [<span data-ttu-id="8c092-188">创建 personWebsite</span><span class="sxs-lookup"><span data-stu-id="8c092-188">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="8c092-189">personWebsite</span><span class="sxs-lookup"><span data-stu-id="8c092-189">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="8c092-190">通过发布到网站集创建新的**personWebsite** 。</span><span class="sxs-lookup"><span data-stu-id="8c092-190">Create a new **personWebsite** by posting to the websites collection.</span></span>                    |
| [<span data-ttu-id="8c092-191">列出网站</span><span class="sxs-lookup"><span data-stu-id="8c092-191">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="8c092-192">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-192">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="8c092-193">获取**personWebsite**对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c092-193">Get a **personWebsite** object collection.</span></span>                                               |

## <a name="properties"></a><span data-ttu-id="8c092-194">属性</span><span class="sxs-lookup"><span data-stu-id="8c092-194">Properties</span></span>

| <span data-ttu-id="8c092-195">属性</span><span class="sxs-lookup"><span data-stu-id="8c092-195">Property</span></span>     | <span data-ttu-id="8c092-196">类型</span><span class="sxs-lookup"><span data-stu-id="8c092-196">Type</span></span>        | <span data-ttu-id="8c092-197">说明</span><span class="sxs-lookup"><span data-stu-id="8c092-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c092-198">id</span><span class="sxs-lookup"><span data-stu-id="8c092-198">id</span></span>            |<span data-ttu-id="8c092-199">String</span><span class="sxs-lookup"><span data-stu-id="8c092-199">String</span></span>       | <span data-ttu-id="8c092-200">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-200">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="8c092-201">关系</span><span class="sxs-lookup"><span data-stu-id="8c092-201">Relationships</span></span>

| <span data-ttu-id="8c092-202">关系</span><span class="sxs-lookup"><span data-stu-id="8c092-202">Relationship</span></span>          | <span data-ttu-id="8c092-203">类型</span><span class="sxs-lookup"><span data-stu-id="8c092-203">Type</span></span>                                                         | <span data-ttu-id="8c092-204">描述</span><span class="sxs-lookup"><span data-stu-id="8c092-204">Description</span></span>         |
|:----------------------|:-------------------------------------------------------------|:--------------------|
|<span data-ttu-id="8c092-205">上级</span><span class="sxs-lookup"><span data-stu-id="8c092-205">account</span></span>                |<span data-ttu-id="8c092-206">[userAccountInformation](useraccountinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-206">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="8c092-207">表示特定绑定到用户帐户的信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-207">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="8c092-208">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-208">Read-only.</span></span> <span data-ttu-id="8c092-209">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-209">Nullable.</span></span>|
|<span data-ttu-id="8c092-210">周年</span><span class="sxs-lookup"><span data-stu-id="8c092-210">anniversaries</span></span>          |<span data-ttu-id="8c092-211">[personAnniversary](personanniversary.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-211">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="8c092-212">代表与人员关联的有意义的日期的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-212">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="8c092-213">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-213">Read-only.</span></span> <span data-ttu-id="8c092-214">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-214">Nullable.</span></span>|
|<span data-ttu-id="8c092-215">educationalActivities</span><span class="sxs-lookup"><span data-stu-id="8c092-215">educationalActivities</span></span>  |<span data-ttu-id="8c092-216">[educationalActivity](educationalactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-216">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="8c092-217">表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。</span><span class="sxs-lookup"><span data-stu-id="8c092-217">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="8c092-218">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-218">Read-only.</span></span> <span data-ttu-id="8c092-219">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-219">Nullable.</span></span>|
|<span data-ttu-id="8c092-220">电子邮件</span><span class="sxs-lookup"><span data-stu-id="8c092-220">emails</span></span>                 |<span data-ttu-id="8c092-221">[itemEmail](itememail.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-221">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="8c092-222">表示有关与用户相关联的电子邮件地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-222">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="8c092-223">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-223">Read-only.</span></span> <span data-ttu-id="8c092-224">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-224">Nullable.</span></span>|
|<span data-ttu-id="8c092-225">interests</span><span class="sxs-lookup"><span data-stu-id="8c092-225">interests</span></span>              |<span data-ttu-id="8c092-226">[personInterest](personinterest.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-226">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="8c092-227">提供有关用户在各种服务中与其自身关联的兴趣的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-227">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="8c092-228">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-228">Read-only.</span></span> <span data-ttu-id="8c092-229">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-229">Nullable.</span></span>|
|<span data-ttu-id="8c092-230">languages</span><span class="sxs-lookup"><span data-stu-id="8c092-230">languages</span></span>              |<span data-ttu-id="8c092-231">[languageProficiency](languageproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-231">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="8c092-232">表示有关用户已添加到其配置文件中的语言的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-232">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="8c092-233">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-233">Read-only.</span></span> <span data-ttu-id="8c092-234">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-234">Nullable.</span></span>|
|<span data-ttu-id="8c092-235">phones</span><span class="sxs-lookup"><span data-stu-id="8c092-235">phones</span></span>                 |<span data-ttu-id="8c092-236">[itemPhone](itemphone.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-236">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="8c092-237">表示有关与各种服务中的用户关联的电话号码的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-237">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="8c092-238">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-238">Read-only.</span></span> <span data-ttu-id="8c092-239">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-239">Nullable.</span></span>|
|<span data-ttu-id="8c092-240">位置</span><span class="sxs-lookup"><span data-stu-id="8c092-240">positions</span></span>              |<span data-ttu-id="8c092-241">[workPosition](workposition.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-241">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="8c092-242">表示有关与用户配置文件相关联的工作职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-242">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="8c092-243">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-243">Read-only.</span></span> <span data-ttu-id="8c092-244">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-244">Nullable.</span></span>|
|<span data-ttu-id="8c092-245">projects</span><span class="sxs-lookup"><span data-stu-id="8c092-245">projects</span></span>               |<span data-ttu-id="8c092-246">[projectParticipation](projectparticipation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-246">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="8c092-247">表示有关与用户关联的项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-247">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="8c092-248">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-248">Read-only.</span></span> <span data-ttu-id="8c092-249">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-249">Nullable.</span></span>|
|<span data-ttu-id="8c092-250">skills</span><span class="sxs-lookup"><span data-stu-id="8c092-250">skills</span></span>                 |<span data-ttu-id="8c092-251">[skillProficiency](skillproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-251">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="8c092-252">表示有关与各种服务中的用户相关的技能的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-252">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="8c092-253">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-253">Read-only.</span></span> <span data-ttu-id="8c092-254">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-254">Nullable.</span></span>|
|<span data-ttu-id="8c092-255">webAccounts</span><span class="sxs-lookup"><span data-stu-id="8c092-255">webAccounts</span></span>            |<span data-ttu-id="8c092-256">[webAccount](webaccount.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-256">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="8c092-257">表示用户已将其添加到其用户配置文件中的 web 帐户。</span><span class="sxs-lookup"><span data-stu-id="8c092-257">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="8c092-258">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-258">Read-only.</span></span> <span data-ttu-id="8c092-259">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-259">Nullable.</span></span>|
|<span data-ttu-id="8c092-260">websites</span><span class="sxs-lookup"><span data-stu-id="8c092-260">websites</span></span>               |<span data-ttu-id="8c092-261">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c092-261">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="8c092-262">表示有关与各种服务中的用户相关联的网站的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c092-262">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="8c092-263">只读。</span><span class="sxs-lookup"><span data-stu-id="8c092-263">Read-only.</span></span> <span data-ttu-id="8c092-264">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c092-264">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c092-265">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c092-265">JSON representation</span></span>

<span data-ttu-id="8c092-266">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c092-266">The following is a JSON representation of the resource.</span></span>

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
