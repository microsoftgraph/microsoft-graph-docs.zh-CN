---
title: 更新设置
description: '更新 settings 对象的属性。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac4907867eebd0cf02bf4e978d1a48b1f1b47ce8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026514"
---
# <a name="update-settings"></a><span data-ttu-id="75578-103">更新设置</span><span class="sxs-lookup"><span data-stu-id="75578-103">Update settings</span></span>

<span data-ttu-id="75578-104">更新[settings](../resources/user-settings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="75578-104">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="75578-105">同一个组织中的用户可以根据自己的首选项或组织策略拥有不同的设置。</span><span class="sxs-lookup"><span data-stu-id="75578-105">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="75578-106">若要获取用户的当前设置, 请参阅[当前用户设置](user-get-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="75578-106">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="75578-107">权限</span><span class="sxs-lookup"><span data-stu-id="75578-107">Permissions</span></span>

<span data-ttu-id="75578-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75578-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75578-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="75578-110">Permission type</span></span>      | <span data-ttu-id="75578-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75578-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75578-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75578-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75578-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="75578-113">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="75578-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75578-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75578-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75578-115">Not supported.</span></span>    |
|<span data-ttu-id="75578-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="75578-116">Application</span></span> | <span data-ttu-id="75578-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75578-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75578-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75578-118">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="75578-119">具有“用户ID”或“userPrincipalName”的请求只能由用户或具有 User.ReadWrite.All 权限的用户访问。</span><span class="sxs-lookup"><span data-stu-id="75578-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="75578-120">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75578-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="75578-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="75578-121">Request headers</span></span>

| <span data-ttu-id="75578-122">标头</span><span class="sxs-lookup"><span data-stu-id="75578-122">Header</span></span>       | <span data-ttu-id="75578-123">值</span><span class="sxs-lookup"><span data-stu-id="75578-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="75578-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="75578-124">Authorization</span></span>  | <span data-ttu-id="75578-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75578-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="75578-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75578-127">Content-Type</span></span>  | <span data-ttu-id="75578-128">application/json</span><span class="sxs-lookup"><span data-stu-id="75578-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75578-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="75578-129">Request body</span></span>

<span data-ttu-id="75578-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="75578-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="75578-133">属性</span><span class="sxs-lookup"><span data-stu-id="75578-133">Property</span></span>     | <span data-ttu-id="75578-134">类型</span><span class="sxs-lookup"><span data-stu-id="75578-134">Type</span></span>   |<span data-ttu-id="75578-135">说明</span><span class="sxs-lookup"><span data-stu-id="75578-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75578-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="75578-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="75578-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="75578-137">Boolean</span></span>|<span data-ttu-id="75578-138">设置为 true 确实禁用对[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta)API 的代理访问, 并禁用用户对 Office Delve 中的文档的访问权限。</span><span class="sxs-lookup"><span data-stu-id="75578-138">Set to true do disable delegate access to the [Trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="75578-139">设置为 true 还会影响 Office 365 中显示的内容的相关性 (例如, SharePoint 主页中的建议网站和 OneDrive for Business 中的发现视图) 显示较少的相关结果。</span><span class="sxs-lookup"><span data-stu-id="75578-139">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="75578-140">此设置反映了[Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)中的控件状态。</span><span class="sxs-lookup"><span data-stu-id="75578-140">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="75578-141">示例</span><span class="sxs-lookup"><span data-stu-id="75578-141">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="75578-142">请求</span><span class="sxs-lookup"><span data-stu-id="75578-142">Request</span></span>

<span data-ttu-id="75578-143">下面的示例请求展示了如何从 Delve 中选择用户, 并对整个组织禁用其对内容相关性的贡献。</span><span class="sxs-lookup"><span data-stu-id="75578-143">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="75578-144">响应</span><span class="sxs-lookup"><span data-stu-id="75578-144">Response</span></span>

<span data-ttu-id="75578-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75578-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="75578-148">批量请求</span><span class="sxs-lookup"><span data-stu-id="75578-148">Batch request</span></span>

<span data-ttu-id="75578-149">此外, 还可以从 Delve 中自愿退出多个用户, 并通过批处理请求禁用对整个组织的内容关联的贡献。</span><span class="sxs-lookup"><span data-stu-id="75578-149">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="75578-150">若要了解详细信息, 请参阅[JSON 批处理](https://developer.microsoft.com/graph/docs/concepts/json_batching)。</span><span class="sxs-lookup"><span data-stu-id="75578-150">To learn more, see [JSON batching](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span></span>

<span data-ttu-id="75578-151">**重要说明**: 只有[组织管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)角色组的成员才能更新多个用户。</span><span class="sxs-lookup"><span data-stu-id="75578-151">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



