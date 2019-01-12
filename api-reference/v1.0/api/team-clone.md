---
title: 克隆团队
description: 创建的工作组的副本。 此操作还将创建相应的组的副本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: afd0c4d1f264989a349a300201ea4a1c528fd681
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912496"
---
# <a name="clone-a-team"></a><span data-ttu-id="918e3-104">克隆团队</span><span class="sxs-lookup"><span data-stu-id="918e3-104">Clone a team</span></span>



<span data-ttu-id="918e3-105">创建[团队](../resources/team.md)的副本。</span><span class="sxs-lookup"><span data-stu-id="918e3-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="918e3-106">此操作还将创建相应的[组](../resources/group.md)的副本。</span><span class="sxs-lookup"><span data-stu-id="918e3-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="918e3-107">您可以指定团队要克隆哪些的部分：</span><span class="sxs-lookup"><span data-stu-id="918e3-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="918e3-108">**应用程序**-副本的 Microsoft 团队的团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="918e3-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="918e3-109">**通道**– 将复制的通道结构 （但不是在进入频道的消息）。</span><span class="sxs-lookup"><span data-stu-id="918e3-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="918e3-110">**成员**– 将复制的成员和组的所有者。</span><span class="sxs-lookup"><span data-stu-id="918e3-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="918e3-111">**设置**– 将复制的团队，以及关键组设置中的所有设置。</span><span class="sxs-lookup"><span data-stu-id="918e3-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="918e3-112">**选项卡**– 副本通道中的选项卡。</span><span class="sxs-lookup"><span data-stu-id="918e3-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="918e3-113">选项卡克隆时，他们将放在未配置状态--Microsoft 团队中的选项卡栏上显示和首次打开它们，您将通过配置屏幕。</span><span class="sxs-lookup"><span data-stu-id="918e3-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="918e3-114">（如果打开选项卡的人员没有配置应用程序的权限，他们将看到一条消息，说明尚未已配置选项卡）。</span><span class="sxs-lookup"><span data-stu-id="918e3-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="918e3-115">克隆是长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="918e3-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="918e3-116">POST 克隆返回后，您需要获取[操作](../resources/teamsasyncoperation.md)以查看是否"运行"或"成功"或"失败"。</span><span class="sxs-lookup"><span data-stu-id="918e3-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="918e3-117">您应继续 GET 之前状态未"运行"。</span><span class="sxs-lookup"><span data-stu-id="918e3-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="918e3-118">获取之间的建议的延迟为 5 秒。</span><span class="sxs-lookup"><span data-stu-id="918e3-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="918e3-119">权限</span><span class="sxs-lookup"><span data-stu-id="918e3-119">Permissions</span></span>

<span data-ttu-id="918e3-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="918e3-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="918e3-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="918e3-122">Permission type</span></span>      | <span data-ttu-id="918e3-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="918e3-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="918e3-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="918e3-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="918e3-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="918e3-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="918e3-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="918e3-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="918e3-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="918e3-127">Not supported.</span></span>    |
|<span data-ttu-id="918e3-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="918e3-128">Application</span></span>                            | <span data-ttu-id="918e3-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="918e3-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="918e3-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="918e3-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="918e3-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="918e3-131">Request headers</span></span>
| <span data-ttu-id="918e3-132">标头</span><span class="sxs-lookup"><span data-stu-id="918e3-132">Header</span></span>       | <span data-ttu-id="918e3-133">值</span><span class="sxs-lookup"><span data-stu-id="918e3-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="918e3-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="918e3-134">Authorization</span></span>  | <span data-ttu-id="918e3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="918e3-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="918e3-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="918e3-137">Content-Type</span></span>  | <span data-ttu-id="918e3-138">application/json</span><span class="sxs-lookup"><span data-stu-id="918e3-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="918e3-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="918e3-139">Request body</span></span>

| <span data-ttu-id="918e3-140">属性</span><span class="sxs-lookup"><span data-stu-id="918e3-140">Property</span></span>     | <span data-ttu-id="918e3-141">类型</span><span class="sxs-lookup"><span data-stu-id="918e3-141">Type</span></span>   |<span data-ttu-id="918e3-142">说明</span><span class="sxs-lookup"><span data-stu-id="918e3-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="918e3-143">Classification</span><span class="sxs-lookup"><span data-stu-id="918e3-143">classification</span></span>|<span data-ttu-id="918e3-144">字符串 （可选）</span><span class="sxs-lookup"><span data-stu-id="918e3-144">String (optional)</span></span>|<span data-ttu-id="918e3-145">介绍组 （如低、 中等或高的业务影响） 的分类。</span><span class="sxs-lookup"><span data-stu-id="918e3-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="918e3-146">如果未指定分类，将从原始团队组复制的分类。</span><span class="sxs-lookup"><span data-stu-id="918e3-146">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="918e3-147">说明</span><span class="sxs-lookup"><span data-stu-id="918e3-147">description</span></span>|<span data-ttu-id="918e3-148">字符串 （可选）</span><span class="sxs-lookup"><span data-stu-id="918e3-148">String (optional)</span></span>|<span data-ttu-id="918e3-149">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="918e3-149">An optional description for the group.</span></span> <span data-ttu-id="918e3-150">如果未指定此属性，它将为空。</span><span class="sxs-lookup"><span data-stu-id="918e3-150">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="918e3-151">displayName</span><span class="sxs-lookup"><span data-stu-id="918e3-151">displayName</span></span>|<span data-ttu-id="918e3-152">字符串</span><span class="sxs-lookup"><span data-stu-id="918e3-152">String</span></span>|<span data-ttu-id="918e3-p109">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="918e3-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="918e3-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="918e3-156">mailNickname</span></span>|<span data-ttu-id="918e3-157">字符串</span><span class="sxs-lookup"><span data-stu-id="918e3-157">String</span></span>|<span data-ttu-id="918e3-158">邮件的组中，组织中唯一的别名。</span><span class="sxs-lookup"><span data-stu-id="918e3-158">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="918e3-159">创建组后，必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="918e3-159">This property must be specified when a group is created.</span></span> <span data-ttu-id="918e3-160">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="918e3-160">Supports $filter.</span></span> <span data-ttu-id="918e3-161">如果未指定此属性，将从 displayName 计算。</span><span class="sxs-lookup"><span data-stu-id="918e3-161">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="918e3-162">已知问题： 当前忽略此属性。</span><span class="sxs-lookup"><span data-stu-id="918e3-162">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="918e3-163">partsToClone</span><span class="sxs-lookup"><span data-stu-id="918e3-163">partsToClone</span></span>| [<span data-ttu-id="918e3-164">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="918e3-164">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="918e3-165">要克隆的部分以逗号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="918e3-165">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="918e3-166">法律部件是"应用程序、 选项卡、 设置、 通道、 成员"。</span><span class="sxs-lookup"><span data-stu-id="918e3-166">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="918e3-167">visibility</span><span class="sxs-lookup"><span data-stu-id="918e3-167">visibility</span></span>|<span data-ttu-id="918e3-168">[teamVisibilityType](../resources/teamvisibilitytype.md)（可选）</span><span class="sxs-lookup"><span data-stu-id="918e3-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="918e3-169">指定组的可见性。</span><span class="sxs-lookup"><span data-stu-id="918e3-169">Specifies the visibility of the group.</span></span> <span data-ttu-id="918e3-170">可能的值为：**专用**的**公共**。</span><span class="sxs-lookup"><span data-stu-id="918e3-170">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="918e3-171">如果未指定可见性，则将从原始团队组复制可见性。</span><span class="sxs-lookup"><span data-stu-id="918e3-171">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="918e3-172">如果正在克隆团队**educationClass**团队、 可见性参数将被忽略，并将被新组的可见性设置为 HiddenMembership。</span><span class="sxs-lookup"><span data-stu-id="918e3-172">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="918e3-173">响应</span><span class="sxs-lookup"><span data-stu-id="918e3-173">Response</span></span>

<span data-ttu-id="918e3-174">如果成功，则此方法将返回`202 Accepted`与某个位置的响应代码： 指向[操作](../resources/teamsasyncoperation.md)资源的标头。</span><span class="sxs-lookup"><span data-stu-id="918e3-174">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="918e3-175">完成该操作后，操作资源会告诉您创建的团队的 id。</span><span class="sxs-lookup"><span data-stu-id="918e3-175">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="918e3-176">示例</span><span class="sxs-lookup"><span data-stu-id="918e3-176">Example</span></span>
#### <a name="request"></a><span data-ttu-id="918e3-177">请求</span><span class="sxs-lookup"><span data-stu-id="918e3-177">Request</span></span>
<span data-ttu-id="918e3-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="918e3-178">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
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

#### <a name="response"></a><span data-ttu-id="918e3-179">响应</span><span class="sxs-lookup"><span data-stu-id="918e3-179">Response</span></span>
<span data-ttu-id="918e3-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="918e3-180">The following is an example of the response.</span></span> <span data-ttu-id="918e3-181">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="918e3-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="918e3-182">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="918e3-182">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
