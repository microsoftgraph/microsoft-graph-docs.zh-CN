---
title: 克隆团队
description: 创建团队副本。 此操作还会创建相应组的副本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6469f6b2857792de7e1b6f261c8d82ad0f2a7648
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054362"
---
# <a name="clone-a-team"></a><span data-ttu-id="099ee-104">克隆团队</span><span class="sxs-lookup"><span data-stu-id="099ee-104">Clone a team</span></span>

<span data-ttu-id="099ee-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="099ee-105">Namespace: microsoft.graph</span></span>



<span data-ttu-id="099ee-106">创建团队 [的副本](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="099ee-106">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="099ee-107">此操作还会创建相应组 [的副本](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="099ee-107">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="099ee-108">可以指定要克隆的团队的哪些部分：</span><span class="sxs-lookup"><span data-stu-id="099ee-108">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="099ee-109">**应用**- Microsoft Teams团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="099ee-109">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="099ee-110">**channels** – 将频道结构 (，但不复制频道中) 。</span><span class="sxs-lookup"><span data-stu-id="099ee-110">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="099ee-111">**members** – 复制组的成员和所有者。</span><span class="sxs-lookup"><span data-stu-id="099ee-111">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="099ee-112">**settings** - 复制团队内的所有设置以及关键组设置。</span><span class="sxs-lookup"><span data-stu-id="099ee-112">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="099ee-113">**tabs** – 在频道内复制选项卡。</span><span class="sxs-lookup"><span data-stu-id="099ee-113">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="099ee-114">克隆选项卡时，选项卡将进入未配置状态 -它们显示在 Microsoft Teams 中的选项卡栏上，首次打开它们时，你将通过配置屏幕。</span><span class="sxs-lookup"><span data-stu-id="099ee-114">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="099ee-115"> (如果打开选项卡的用户没有配置应用的权限，他们会看到一条消息，说明尚未配置选项卡。) </span><span class="sxs-lookup"><span data-stu-id="099ee-115">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="099ee-116">克隆是一项长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="099ee-116">Cloning is a long-running operation.</span></span>
<span data-ttu-id="099ee-117">POST 克隆返回后，您需要获取操作以查看其[](../resources/teamsasyncoperation.md)是否"正在运行"或"成功"或"失败"。</span><span class="sxs-lookup"><span data-stu-id="099ee-117">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="099ee-118">您应该继续 GET，直到状态未"正在运行"。</span><span class="sxs-lookup"><span data-stu-id="099ee-118">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="099ee-119">GET 之间的建议延迟为 5 秒。</span><span class="sxs-lookup"><span data-stu-id="099ee-119">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="099ee-120">权限</span><span class="sxs-lookup"><span data-stu-id="099ee-120">Permissions</span></span>

<span data-ttu-id="099ee-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="099ee-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="099ee-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="099ee-123">Permission type</span></span>      | <span data-ttu-id="099ee-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="099ee-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="099ee-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="099ee-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="099ee-126">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="099ee-126">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="099ee-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="099ee-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="099ee-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="099ee-128">Not supported.</span></span>    |
|<span data-ttu-id="099ee-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="099ee-129">Application</span></span>                            | <span data-ttu-id="099ee-130">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="099ee-130">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="099ee-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="099ee-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="099ee-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="099ee-132">Request headers</span></span>
| <span data-ttu-id="099ee-133">标头</span><span class="sxs-lookup"><span data-stu-id="099ee-133">Header</span></span>       | <span data-ttu-id="099ee-134">值</span><span class="sxs-lookup"><span data-stu-id="099ee-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="099ee-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="099ee-135">Authorization</span></span>  | <span data-ttu-id="099ee-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="099ee-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="099ee-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="099ee-138">Content-Type</span></span>  | <span data-ttu-id="099ee-139">application/json</span><span class="sxs-lookup"><span data-stu-id="099ee-139">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="099ee-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="099ee-140">Request body</span></span>

| <span data-ttu-id="099ee-141">属性</span><span class="sxs-lookup"><span data-stu-id="099ee-141">Property</span></span>     | <span data-ttu-id="099ee-142">类型</span><span class="sxs-lookup"><span data-stu-id="099ee-142">Type</span></span>   |<span data-ttu-id="099ee-143">说明</span><span class="sxs-lookup"><span data-stu-id="099ee-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="099ee-144">classification</span><span class="sxs-lookup"><span data-stu-id="099ee-144">classification</span></span>|<span data-ttu-id="099ee-145">可选 (字符串) </span><span class="sxs-lookup"><span data-stu-id="099ee-145">String (optional)</span></span>|<span data-ttu-id="099ee-146">介绍组策略分类 (低、中或高业务影响) 。</span><span class="sxs-lookup"><span data-stu-id="099ee-146">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="099ee-147">如果未指定分类，则从原始团队/组复制分类。</span><span class="sxs-lookup"><span data-stu-id="099ee-147">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="099ee-148">说明</span><span class="sxs-lookup"><span data-stu-id="099ee-148">description</span></span>|<span data-ttu-id="099ee-149">可选 (字符串) </span><span class="sxs-lookup"><span data-stu-id="099ee-149">String (optional)</span></span>|<span data-ttu-id="099ee-150">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="099ee-150">An optional description for the group.</span></span> <span data-ttu-id="099ee-151">如果未指定此属性，则此属性将留空。</span><span class="sxs-lookup"><span data-stu-id="099ee-151">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="099ee-152">displayName</span><span class="sxs-lookup"><span data-stu-id="099ee-152">displayName</span></span>|<span data-ttu-id="099ee-153">String</span><span class="sxs-lookup"><span data-stu-id="099ee-153">String</span></span>|<span data-ttu-id="099ee-p109">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="099ee-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="099ee-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="099ee-157">mailNickname</span></span>|<span data-ttu-id="099ee-158">String</span><span class="sxs-lookup"><span data-stu-id="099ee-158">String</span></span>|<span data-ttu-id="099ee-159">组的邮件别名，在组织中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="099ee-159">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="099ee-160">创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="099ee-160">This property must be specified when a group is created.</span></span> <span data-ttu-id="099ee-161">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="099ee-161">Supports $filter.</span></span> <span data-ttu-id="099ee-162">如果未指定此属性，则从 displayName 计算此属性。</span><span class="sxs-lookup"><span data-stu-id="099ee-162">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="099ee-163">已知问题：此属性当前被忽略。</span><span class="sxs-lookup"><span data-stu-id="099ee-163">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="099ee-164">partsToClone</span><span class="sxs-lookup"><span data-stu-id="099ee-164">partsToClone</span></span>| [<span data-ttu-id="099ee-165">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="099ee-165">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="099ee-166">要克隆的部件的逗号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="099ee-166">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="099ee-167">法律部分为"应用、选项卡、设置、频道、成员"。</span><span class="sxs-lookup"><span data-stu-id="099ee-167">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="099ee-168">visibility</span><span class="sxs-lookup"><span data-stu-id="099ee-168">visibility</span></span>|<span data-ttu-id="099ee-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (可选) </span><span class="sxs-lookup"><span data-stu-id="099ee-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="099ee-170">指定组的可见性。</span><span class="sxs-lookup"><span data-stu-id="099ee-170">Specifies the visibility of the group.</span></span> <span data-ttu-id="099ee-171">可能的值是 **：Private** **、Public**。</span><span class="sxs-lookup"><span data-stu-id="099ee-171">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="099ee-172">如果未指定可见性，则从原始团队/组复制可见性。</span><span class="sxs-lookup"><span data-stu-id="099ee-172">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="099ee-173">如果要克隆的团队是 **educationClass** 团队，则忽略 visibility 参数，并且新组的可见性将设置为 HiddenMembership。</span><span class="sxs-lookup"><span data-stu-id="099ee-173">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="099ee-174">响应</span><span class="sxs-lookup"><span data-stu-id="099ee-174">Response</span></span>

<span data-ttu-id="099ee-175">如果成功，此方法将返回包含指向操作资源的 `202 Accepted` Location： 标头 [的响应](../resources/teamsasyncoperation.md) 代码。</span><span class="sxs-lookup"><span data-stu-id="099ee-175">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="099ee-176">操作完成后，操作资源将告知你已创建团队的 ID。</span><span class="sxs-lookup"><span data-stu-id="099ee-176">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="099ee-177">示例</span><span class="sxs-lookup"><span data-stu-id="099ee-177">Example</span></span>
#### <a name="request"></a><span data-ttu-id="099ee-178">请求</span><span class="sxs-lookup"><span data-stu-id="099ee-178">Request</span></span>
<span data-ttu-id="099ee-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="099ee-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="099ee-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="099ee-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clone_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```
# <a name="c"></a>[<span data-ttu-id="099ee-181">C#</span><span class="sxs-lookup"><span data-stu-id="099ee-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="099ee-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="099ee-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="099ee-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="099ee-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="099ee-184">Java</span><span class="sxs-lookup"><span data-stu-id="099ee-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clone-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="099ee-185">响应</span><span class="sxs-lookup"><span data-stu-id="099ee-185">Response</span></span>
<span data-ttu-id="099ee-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="099ee-186">The following is an example of the response.</span></span> <span data-ttu-id="099ee-187">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="099ee-187">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

