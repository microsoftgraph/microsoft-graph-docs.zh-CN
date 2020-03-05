---
title: 克隆团队
description: 创建团队的副本。 此操作还会创建相应组的副本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 782be85dc7a82e56bc5a2dc0d4449b6562f68c17
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452615"
---
# <a name="clone-a-team"></a><span data-ttu-id="5b509-104">克隆团队</span><span class="sxs-lookup"><span data-stu-id="5b509-104">Clone a team</span></span>

<span data-ttu-id="5b509-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5b509-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b509-106">创建[团队](../resources/team.md)的副本。</span><span class="sxs-lookup"><span data-stu-id="5b509-106">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="5b509-107">此操作还会创建相应[组](../resources/group.md)的副本。</span><span class="sxs-lookup"><span data-stu-id="5b509-107">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="5b509-108">您可以指定要克隆的团队部分：</span><span class="sxs-lookup"><span data-stu-id="5b509-108">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="5b509-109">**应用**-复制团队中安装的 Microsoft 团队应用。</span><span class="sxs-lookup"><span data-stu-id="5b509-109">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="5b509-110">**频道**–复制通道结构（而不是通道中的邮件）。</span><span class="sxs-lookup"><span data-stu-id="5b509-110">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="5b509-111">**members** –复制组的成员和所有者。</span><span class="sxs-lookup"><span data-stu-id="5b509-111">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="5b509-112">**设置**–复制团队内的所有设置以及关键组设置。</span><span class="sxs-lookup"><span data-stu-id="5b509-112">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="5b509-113">**选项卡**–复制频道中的选项卡。</span><span class="sxs-lookup"><span data-stu-id="5b509-113">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="5b509-114">当选项卡被克隆时，它们将被置于未配置状态--它们将显示在 Microsoft 团队中的选项卡栏上，在第一次打开它们时，您将完成配置屏幕。</span><span class="sxs-lookup"><span data-stu-id="5b509-114">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="5b509-115">（如果打开该选项卡的用户没有配置应用的权限，他们将看到一条消息，说明该选项卡尚未配置。）</span><span class="sxs-lookup"><span data-stu-id="5b509-115">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="5b509-116">克隆是一项长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="5b509-116">Cloning is a long-running operation.</span></span>
<span data-ttu-id="5b509-117">在 POST 克隆返回之后，您需要获取 Location：头所返回的[操作](../resources/teamsasyncoperation.md)，以查看它是 "正在运行" 还是 "已成功" 或 "失败"。</span><span class="sxs-lookup"><span data-stu-id="5b509-117">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) returned by the Location: header to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="5b509-118">您应继续获取，直到状态不为 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="5b509-118">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="5b509-119">建议的获取延迟为5秒。</span><span class="sxs-lookup"><span data-stu-id="5b509-119">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b509-120">权限</span><span class="sxs-lookup"><span data-stu-id="5b509-120">Permissions</span></span>

<span data-ttu-id="5b509-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b509-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b509-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b509-123">Permission type</span></span>      | <span data-ttu-id="5b509-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b509-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b509-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b509-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b509-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b509-126">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b509-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b509-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b509-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b509-128">Not supported.</span></span>    |
|<span data-ttu-id="5b509-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b509-129">Application</span></span>                            | <span data-ttu-id="5b509-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b509-130">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b509-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b509-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="5b509-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b509-132">Request headers</span></span>
| <span data-ttu-id="5b509-133">标头</span><span class="sxs-lookup"><span data-stu-id="5b509-133">Header</span></span>       | <span data-ttu-id="5b509-134">值</span><span class="sxs-lookup"><span data-stu-id="5b509-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b509-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b509-135">Authorization</span></span>  | <span data-ttu-id="5b509-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b509-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b509-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b509-138">Content-Type</span></span>  | <span data-ttu-id="5b509-139">application/json</span><span class="sxs-lookup"><span data-stu-id="5b509-139">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b509-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b509-140">Request body</span></span>

| <span data-ttu-id="5b509-141">属性</span><span class="sxs-lookup"><span data-stu-id="5b509-141">Property</span></span>     | <span data-ttu-id="5b509-142">类型</span><span class="sxs-lookup"><span data-stu-id="5b509-142">Type</span></span>   |<span data-ttu-id="5b509-143">说明</span><span class="sxs-lookup"><span data-stu-id="5b509-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b509-144">classification</span><span class="sxs-lookup"><span data-stu-id="5b509-144">classification</span></span>|<span data-ttu-id="5b509-145">String （可选）</span><span class="sxs-lookup"><span data-stu-id="5b509-145">String (optional)</span></span>|<span data-ttu-id="5b509-146">描述组的分类（如低、中或高业务影响）。</span><span class="sxs-lookup"><span data-stu-id="5b509-146">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="5b509-147">此属性的有效值是通过基于[模板定义](../resources/directorysettingtemplate.md)创建 ClassificationList[设置](../resources/directorysetting.md)值来定义的。</span><span class="sxs-lookup"><span data-stu-id="5b509-147">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="5b509-148">如果未指定分类，则将从原始团队/组复制分类。</span><span class="sxs-lookup"><span data-stu-id="5b509-148">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="5b509-149">说明</span><span class="sxs-lookup"><span data-stu-id="5b509-149">description</span></span>|<span data-ttu-id="5b509-150">String （可选）</span><span class="sxs-lookup"><span data-stu-id="5b509-150">String (optional)</span></span>|<span data-ttu-id="5b509-151">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="5b509-151">An optional description for the group.</span></span> <span data-ttu-id="5b509-152">如果未指定此属性，则它将保留为空。</span><span class="sxs-lookup"><span data-stu-id="5b509-152">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="5b509-153">displayName</span><span class="sxs-lookup"><span data-stu-id="5b509-153">displayName</span></span>|<span data-ttu-id="5b509-154">String</span><span class="sxs-lookup"><span data-stu-id="5b509-154">String</span></span>|<span data-ttu-id="5b509-p109">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="5b509-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="5b509-158">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5b509-158">mailNickname</span></span>|<span data-ttu-id="5b509-159">String</span><span class="sxs-lookup"><span data-stu-id="5b509-159">String</span></span>|<span data-ttu-id="5b509-160">组的邮件别名，在组织中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="5b509-160">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="5b509-161">创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="5b509-161">This property must be specified when a group is created.</span></span> <span data-ttu-id="5b509-162">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="5b509-162">Supports $filter.</span></span> <span data-ttu-id="5b509-163">如果未指定此属性，则将从 displayName 计算。</span><span class="sxs-lookup"><span data-stu-id="5b509-163">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="5b509-164">已知问题：此属性当前被忽略。</span><span class="sxs-lookup"><span data-stu-id="5b509-164">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="5b509-165">partsToClone</span><span class="sxs-lookup"><span data-stu-id="5b509-165">partsToClone</span></span>| [<span data-ttu-id="5b509-166">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="5b509-166">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="5b509-167">要克隆的部分的逗号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="5b509-167">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="5b509-168">法律部门是 "应用、选项卡、设置、通道、成员"。</span><span class="sxs-lookup"><span data-stu-id="5b509-168">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="5b509-169">visibility</span><span class="sxs-lookup"><span data-stu-id="5b509-169">visibility</span></span>|<span data-ttu-id="5b509-170">[teamVisibilityType](../resources/teamvisibilitytype.md) （可选）</span><span class="sxs-lookup"><span data-stu-id="5b509-170">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="5b509-171">指定组的可见性。</span><span class="sxs-lookup"><span data-stu-id="5b509-171">Specifies the visibility of the group.</span></span> <span data-ttu-id="5b509-172">可能的值为： **Private**、 **Public**。</span><span class="sxs-lookup"><span data-stu-id="5b509-172">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="5b509-173">如果未指定可见性，将从原始团队/组复制可见性。</span><span class="sxs-lookup"><span data-stu-id="5b509-173">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="5b509-174">如果克隆的团队是**educationClass**团队，则忽略 visibility 参数，新组的可见性将设置为 HiddenMembership。</span><span class="sxs-lookup"><span data-stu-id="5b509-174">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="5b509-175">响应</span><span class="sxs-lookup"><span data-stu-id="5b509-175">Response</span></span>

<span data-ttu-id="5b509-176">如果成功，此方法将返回一个`202 Accepted`位置为的响应代码：标头，指向[操作](../resources/teamsasyncoperation.md)资源。</span><span class="sxs-lookup"><span data-stu-id="5b509-176">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="5b509-177">操作完成后，操作资源将告知您创建的团队的 id。</span><span class="sxs-lookup"><span data-stu-id="5b509-177">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="5b509-178">示例</span><span class="sxs-lookup"><span data-stu-id="5b509-178">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5b509-179">请求</span><span class="sxs-lookup"><span data-stu-id="5b509-179">Request</span></span>
<span data-ttu-id="5b509-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b509-180">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5b509-181">响应</span><span class="sxs-lookup"><span data-stu-id="5b509-181">Response</span></span>
<span data-ttu-id="5b509-182">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5b509-182">The following is an example of the response.</span></span> <span data-ttu-id="5b509-183">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5b509-183">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5b509-184">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b509-184">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
