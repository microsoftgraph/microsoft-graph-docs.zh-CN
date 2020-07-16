---
title: 配置文件资源类型
description: 表示对用户进行了说明的属性，以及通过 microsoft Graph 在 Microsoft 365 和第三方服务和体验中进行的共享的用户体验。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f80dfccbd662e1e398c0d4b79b0086575a83e2b
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050877"
---
# <a name="profile-resource-type"></a><span data-ttu-id="bf8b7-103">配置文件资源类型</span><span class="sxs-lookup"><span data-stu-id="bf8b7-103">profile resource type</span></span>

<span data-ttu-id="bf8b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf8b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf8b7-105">表示对租户中的用户进行描述性的属性，例如，周年纪念和教育活动。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-105">Represents properties that are descriptive of a user in a tenant, for example, anniversaries and education activities.</span></span> <span data-ttu-id="bf8b7-106">这些属性在共享中通过 Microsoft 365 和第三方服务体验，并通过 Microsoft Graph 体验。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-106">These properties are surfaced in shared, people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

<span data-ttu-id="bf8b7-107">以编程方式，这些属性表示为**配置文件**资源的[关系](#relationships)。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-107">Programmatically, these properties are expressed as [relationships](#relationships) of the **profile** resource.</span></span> <span data-ttu-id="bf8b7-108">若要获取这些导航属性之一或为用户创建这些属性的实例，请对该属性使用相应的 GET 或 POST 方法（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-108">To get one of these navigation properties or create an instance of these properties for the user, use the corresponding GET or POST method on that property, where applicable.</span></span> <span data-ttu-id="bf8b7-109">请参阅下面列出的[方法](#methods)。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-109">See the [methods](#methods) listed below.</span></span>

## <a name="methods"></a><span data-ttu-id="bf8b7-110">方法</span><span class="sxs-lookup"><span data-stu-id="bf8b7-110">Methods</span></span>

| <span data-ttu-id="bf8b7-111">方法</span><span class="sxs-lookup"><span data-stu-id="bf8b7-111">Method</span></span>                                                                     | <span data-ttu-id="bf8b7-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="bf8b7-112">Return Type</span></span>                                                    | <span data-ttu-id="bf8b7-113">说明</span><span class="sxs-lookup"><span data-stu-id="bf8b7-113">Description</span></span>                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [<span data-ttu-id="bf8b7-114">获取个人资料</span><span class="sxs-lookup"><span data-stu-id="bf8b7-114">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="bf8b7-115">profile</span><span class="sxs-lookup"><span data-stu-id="bf8b7-115">profile</span></span>](profile.md)                                          | <span data-ttu-id="bf8b7-116">读取 profile 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-116">Read properties and relationships of the profile object.</span></span>                                         |
| [<span data-ttu-id="bf8b7-117">删除个人资料</span><span class="sxs-lookup"><span data-stu-id="bf8b7-117">Delete profile</span></span>](../api/profile-delete.md)                                 | <span data-ttu-id="bf8b7-118">无</span><span class="sxs-lookup"><span data-stu-id="bf8b7-118">None</span></span>                                                           | <span data-ttu-id="bf8b7-119">删除**配置文件**对象。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-119">Delete a **profile** object.</span></span>                                                                 |
| [<span data-ttu-id="bf8b7-120">列表帐户</span><span class="sxs-lookup"><span data-stu-id="bf8b7-120">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="bf8b7-121">[userAccountInformation](useraccountinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-121">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="bf8b7-122">获取**userAccountInformation**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-122">Get a **userAccountInformation** object collection.</span></span>                                          |
| [<span data-ttu-id="bf8b7-123">创建 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="bf8b7-123">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="bf8b7-124">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="bf8b7-124">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="bf8b7-125">通过发布到周年纪念集合创建新的**personAnniversary** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-125">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>               |
| [<span data-ttu-id="bf8b7-126">列出周年纪念</span><span class="sxs-lookup"><span data-stu-id="bf8b7-126">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="bf8b7-127">[personAnniversary](personanniversary.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-127">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="bf8b7-128">获取**personAnniversary**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-128">Get a **personAnniversary** object collection.</span></span>                                               |
| [<span data-ttu-id="bf8b7-129">创建 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="bf8b7-129">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="bf8b7-130">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="bf8b7-130">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="bf8b7-131">通过发布到**educationalActivities**集合创建新的**educationalActivity** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-131">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="bf8b7-132">列出 educationalActivities</span><span class="sxs-lookup"><span data-stu-id="bf8b7-132">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="bf8b7-133">[educationalActivity](educationalactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-133">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="bf8b7-134">获取**educationalActivity**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-134">Get an **educationalActivity** object collection.</span></span>                                            |
| [<span data-ttu-id="bf8b7-135">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="bf8b7-135">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="bf8b7-136">itemEmail</span><span class="sxs-lookup"><span data-stu-id="bf8b7-136">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="bf8b7-137">通过发布到电子邮件集合创建新的**itemEmail** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-137">Create a new **itemEmail** by posting to the emails collection.</span></span>                              |
| [<span data-ttu-id="bf8b7-138">列出电子邮件</span><span class="sxs-lookup"><span data-stu-id="bf8b7-138">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="bf8b7-139">[itemEmail](itememail.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-139">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="bf8b7-140">获取**itemEmail**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-140">Get an **itemEmail** object collection.</span></span>                                                      |
| [<span data-ttu-id="bf8b7-141">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="bf8b7-141">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="bf8b7-142">personInterest</span><span class="sxs-lookup"><span data-stu-id="bf8b7-142">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="bf8b7-143">通过发布到 "兴趣" 集合创建新的**personInterest** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-143">Create a new **personInterest** by posting to the interests collection.</span></span>                      |
| [<span data-ttu-id="bf8b7-144">列出兴趣</span><span class="sxs-lookup"><span data-stu-id="bf8b7-144">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="bf8b7-145">[personInterest](personinterest.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-145">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="bf8b7-146">获取**personInterest**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-146">Get a **personInterest** object collection.</span></span>                                                  |
| [<span data-ttu-id="bf8b7-147">创建 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="bf8b7-147">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="bf8b7-148">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="bf8b7-148">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="bf8b7-149">通过发布到语言集合创建新的**languageProficiency** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-149">Create a new **languageProficiency** by posting to the languages collection.</span></span>                 |
| [<span data-ttu-id="bf8b7-150">列出语言</span><span class="sxs-lookup"><span data-stu-id="bf8b7-150">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="bf8b7-151">[languageProficiency](languageproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-151">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="bf8b7-152">获取**languageProficiency**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-152">Get a **languageProficiency** object collection.</span></span>                                             |
| [<span data-ttu-id="bf8b7-153">列出名称</span><span class="sxs-lookup"><span data-stu-id="bf8b7-153">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="bf8b7-154">[contact.personname](personname.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-154">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="bf8b7-155">获取**contact.personname**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-155">Get a **personName** object collection.</span></span>                                                      |
| [<span data-ttu-id="bf8b7-156">创建 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="bf8b7-156">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="bf8b7-157">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="bf8b7-157">personName</span></span>](personName.md)                                    | <span data-ttu-id="bf8b7-158">通过发布到名称集合创建新的**contact.personname**对象。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-158">Create a new **personName** object by posting to the names collection.</span></span>                       |
| [<span data-ttu-id="bf8b7-159">列出网站</span><span class="sxs-lookup"><span data-stu-id="bf8b7-159">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="bf8b7-160">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-160">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="bf8b7-161">获取**personWebsite**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-161">Get a **personWebsite** object collection.</span></span>                                                   |
| [<span data-ttu-id="bf8b7-162">创建 itemPhone</span><span class="sxs-lookup"><span data-stu-id="bf8b7-162">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="bf8b7-163">itemPhone</span><span class="sxs-lookup"><span data-stu-id="bf8b7-163">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="bf8b7-164">通过发布到 "电话" 集合创建新的 itemPhone。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-164">Create a new itemPhone by posting to the phones collection.</span></span>                                  |
| [<span data-ttu-id="bf8b7-165">列出电话</span><span class="sxs-lookup"><span data-stu-id="bf8b7-165">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="bf8b7-166">[itemPhone](itemphone.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-166">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="bf8b7-167">获取**itemPhone**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-167">Get a **itemPhone** object collection.</span></span>                                                       |
| [<span data-ttu-id="bf8b7-168">创建 workPosition</span><span class="sxs-lookup"><span data-stu-id="bf8b7-168">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="bf8b7-169">workPosition</span><span class="sxs-lookup"><span data-stu-id="bf8b7-169">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="bf8b7-170">通过发布到 "职位" 集合创建新的 workPosition。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-170">Create a new workPosition by posting to the positions collection.</span></span>                            |
| [<span data-ttu-id="bf8b7-171">列表位置</span><span class="sxs-lookup"><span data-stu-id="bf8b7-171">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="bf8b7-172">[workPosition](workposition.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-172">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="bf8b7-173">获取**workPosition**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-173">Get a **workPosition** object collection.</span></span>                                                    |
| [<span data-ttu-id="bf8b7-174">创建 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="bf8b7-174">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="bf8b7-175">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="bf8b7-175">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="bf8b7-176">通过发布到项目集合创建新的**projectParticipation** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-176">Create a new **projectParticipation** by posting to the projects collection.</span></span>                 |
| [<span data-ttu-id="bf8b7-177">列出项目</span><span class="sxs-lookup"><span data-stu-id="bf8b7-177">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="bf8b7-178">[projectParticipation](projectparticipation.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-178">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="bf8b7-179">获取**projectParticipation**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-179">Get a **projectParticipation** object collection.</span></span>                                            |
| [<span data-ttu-id="bf8b7-180">创建 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="bf8b7-180">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="bf8b7-181">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="bf8b7-181">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="bf8b7-182">通过发布到技能集合创建新的**skillProficiency** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-182">Create a new **skillProficiency** by posting to the skills collection.</span></span>                       |
| [<span data-ttu-id="bf8b7-183">列表技能</span><span class="sxs-lookup"><span data-stu-id="bf8b7-183">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="bf8b7-184">[skillProficiency](skillproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-184">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="bf8b7-185">获取**skillProficiency**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-185">Get a **skillProficiency** object collection.</span></span>                                                |
| [<span data-ttu-id="bf8b7-186">创建 webAccount</span><span class="sxs-lookup"><span data-stu-id="bf8b7-186">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="bf8b7-187">webAccount</span><span class="sxs-lookup"><span data-stu-id="bf8b7-187">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="bf8b7-188">通过发布到 webAccounts 集合创建新的**webAccount** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-188">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                        |
| [<span data-ttu-id="bf8b7-189">列出 webAccounts</span><span class="sxs-lookup"><span data-stu-id="bf8b7-189">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="bf8b7-190">[webAccount](webaccount.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-190">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="bf8b7-191">获取**webAccount**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-191">Get a **webAccount** object collection.</span></span>                                                      |
| [<span data-ttu-id="bf8b7-192">创建 personWebsite</span><span class="sxs-lookup"><span data-stu-id="bf8b7-192">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="bf8b7-193">personWebsite</span><span class="sxs-lookup"><span data-stu-id="bf8b7-193">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="bf8b7-194">通过发布到网站集创建新的**personWebsite** 。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-194">Create a new **personWebsite** by posting to the websites collection.</span></span>                        |
| [<span data-ttu-id="bf8b7-195">列出网站</span><span class="sxs-lookup"><span data-stu-id="bf8b7-195">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="bf8b7-196">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-196">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="bf8b7-197">获取**personWebsite**对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-197">Get a **personWebsite** object collection.</span></span>                                                   |

## <a name="properties"></a><span data-ttu-id="bf8b7-198">属性</span><span class="sxs-lookup"><span data-stu-id="bf8b7-198">Properties</span></span>

| <span data-ttu-id="bf8b7-199">属性</span><span class="sxs-lookup"><span data-stu-id="bf8b7-199">Property</span></span>     | <span data-ttu-id="bf8b7-200">类型</span><span class="sxs-lookup"><span data-stu-id="bf8b7-200">Type</span></span>        | <span data-ttu-id="bf8b7-201">说明</span><span class="sxs-lookup"><span data-stu-id="bf8b7-201">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bf8b7-202">id</span><span class="sxs-lookup"><span data-stu-id="bf8b7-202">id</span></span>            |<span data-ttu-id="bf8b7-203">String</span><span class="sxs-lookup"><span data-stu-id="bf8b7-203">String</span></span>       | <span data-ttu-id="bf8b7-204">只读。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-204">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="bf8b7-205">关系</span><span class="sxs-lookup"><span data-stu-id="bf8b7-205">Relationships</span></span>

| <span data-ttu-id="bf8b7-206">关系</span><span class="sxs-lookup"><span data-stu-id="bf8b7-206">Relationship</span></span>          | <span data-ttu-id="bf8b7-207">类型</span><span class="sxs-lookup"><span data-stu-id="bf8b7-207">Type</span></span>                                                         | <span data-ttu-id="bf8b7-208">说明</span><span class="sxs-lookup"><span data-stu-id="bf8b7-208">Description</span></span>                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="bf8b7-209">上级</span><span class="sxs-lookup"><span data-stu-id="bf8b7-209">account</span></span>                |<span data-ttu-id="bf8b7-210">[userAccountInformation](useraccountinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-210">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="bf8b7-211">表示特定绑定到用户帐户的信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-211">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="bf8b7-212">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-212">Read-only.</span></span> <span data-ttu-id="bf8b7-213">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-213">Nullable.</span></span>                                                             |
|<span data-ttu-id="bf8b7-214">周年</span><span class="sxs-lookup"><span data-stu-id="bf8b7-214">anniversaries</span></span>          |<span data-ttu-id="bf8b7-215">[personAnniversary](personanniversary.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-215">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="bf8b7-216">代表与人员关联的有意义的日期的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-216">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="bf8b7-217">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-217">Read-only.</span></span> <span data-ttu-id="bf8b7-218">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-218">Nullable.</span></span>                                                      |
|<span data-ttu-id="bf8b7-219">educationalActivities</span><span class="sxs-lookup"><span data-stu-id="bf8b7-219">educationalActivities</span></span>  |<span data-ttu-id="bf8b7-220">[educationalActivity](educationalactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-220">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="bf8b7-221">表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-221">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="bf8b7-222">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-222">Read-only.</span></span> <span data-ttu-id="bf8b7-223">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-223">Nullable.</span></span>|
|<span data-ttu-id="bf8b7-224">电子邮件</span><span class="sxs-lookup"><span data-stu-id="bf8b7-224">emails</span></span>                 |<span data-ttu-id="bf8b7-225">[itemEmail](itememail.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-225">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="bf8b7-226">表示有关与用户相关联的电子邮件地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-226">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="bf8b7-227">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-227">Read-only.</span></span> <span data-ttu-id="bf8b7-228">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-228">Nullable.</span></span>                                           |
|<span data-ttu-id="bf8b7-229">interests</span><span class="sxs-lookup"><span data-stu-id="bf8b7-229">interests</span></span>              |<span data-ttu-id="bf8b7-230">[personInterest](personinterest.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-230">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="bf8b7-231">提供有关用户在各种服务中与其自身关联的兴趣的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-231">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="bf8b7-232">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-232">Read-only.</span></span> <span data-ttu-id="bf8b7-233">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-233">Nullable.</span></span>                |
|<span data-ttu-id="bf8b7-234">languages</span><span class="sxs-lookup"><span data-stu-id="bf8b7-234">languages</span></span>              |<span data-ttu-id="bf8b7-235">[languageProficiency](languageproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-235">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="bf8b7-236">表示有关用户已添加到其配置文件中的语言的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-236">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="bf8b7-237">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-237">Read-only.</span></span> <span data-ttu-id="bf8b7-238">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-238">Nullable.</span></span>                                   |
|<span data-ttu-id="bf8b7-239">phones</span><span class="sxs-lookup"><span data-stu-id="bf8b7-239">phones</span></span>                 |<span data-ttu-id="bf8b7-240">[itemPhone](itemphone.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-240">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="bf8b7-241">表示有关与各种服务中的用户关联的电话号码的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-241">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="bf8b7-242">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-242">Read-only.</span></span> <span data-ttu-id="bf8b7-243">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-243">Nullable.</span></span>                           |
|<span data-ttu-id="bf8b7-244">位置</span><span class="sxs-lookup"><span data-stu-id="bf8b7-244">positions</span></span>              |<span data-ttu-id="bf8b7-245">[workPosition](workposition.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-245">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="bf8b7-246">表示有关与用户配置文件相关联的工作职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-246">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="bf8b7-247">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-247">Read-only.</span></span> <span data-ttu-id="bf8b7-248">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-248">Nullable.</span></span>                                    |
|<span data-ttu-id="bf8b7-249">projects</span><span class="sxs-lookup"><span data-stu-id="bf8b7-249">projects</span></span>               |<span data-ttu-id="bf8b7-250">[projectParticipation](projectparticipation.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-250">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="bf8b7-251">表示有关与用户关联的项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-251">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="bf8b7-252">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-252">Read-only.</span></span> <span data-ttu-id="bf8b7-253">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-253">Nullable.</span></span>                                                    |
|<span data-ttu-id="bf8b7-254">skills</span><span class="sxs-lookup"><span data-stu-id="bf8b7-254">skills</span></span>                 |<span data-ttu-id="bf8b7-255">[skillProficiency](skillproficiency.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-255">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="bf8b7-256">表示有关与各种服务中的用户相关的技能的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-256">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="bf8b7-257">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-257">Read-only.</span></span> <span data-ttu-id="bf8b7-258">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-258">Nullable.</span></span>                                  |
|<span data-ttu-id="bf8b7-259">webAccounts</span><span class="sxs-lookup"><span data-stu-id="bf8b7-259">webAccounts</span></span>            |<span data-ttu-id="bf8b7-260">[webAccount](webaccount.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-260">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="bf8b7-261">表示用户已将其添加到其用户配置文件中的 web 帐户。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-261">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="bf8b7-262">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-262">Read-only.</span></span> <span data-ttu-id="bf8b7-263">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-263">Nullable.</span></span>                               |
|<span data-ttu-id="bf8b7-264">websites</span><span class="sxs-lookup"><span data-stu-id="bf8b7-264">websites</span></span>               |<span data-ttu-id="bf8b7-265">[personWebsite](personwebsite.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf8b7-265">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="bf8b7-266">表示有关与各种服务中的用户相关联的网站的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-266">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="bf8b7-267">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-267">Read-only.</span></span> <span data-ttu-id="bf8b7-268">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-268">Nullable.</span></span>                                |

## <a name="json-representation"></a><span data-ttu-id="bf8b7-269">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf8b7-269">JSON representation</span></span>

<span data-ttu-id="bf8b7-270">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf8b7-270">The following is a JSON representation of the resource.</span></span>

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
    "id": "String (identifier)"
}
```

<!--
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
-->


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
