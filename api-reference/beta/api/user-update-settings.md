---
title: 更新设置
description: '更新设置对象的属性。 '
ms.openlocfilehash: 53b5fb2ce37aa9d80466face5ec03d1b54e87c09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048294"
---
# <a name="update-settings"></a><span data-ttu-id="d6356-103">更新设置</span><span class="sxs-lookup"><span data-stu-id="d6356-103">Update settings</span></span>

> <span data-ttu-id="d6356-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6356-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6356-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6356-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6356-106">更新[设置](../resources/user-settings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6356-106">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="d6356-107">在同一组织的用户可以根据他们输入首选项或组织策略的不同设置。</span><span class="sxs-lookup"><span data-stu-id="d6356-107">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="d6356-108">若要获取用户当前设置，请参阅[当前用户设置](user-get-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="d6356-108">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d6356-109">权限</span><span class="sxs-lookup"><span data-stu-id="d6356-109">Permissions</span></span>

<span data-ttu-id="d6356-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6356-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6356-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6356-112">Permission type</span></span>      | <span data-ttu-id="d6356-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6356-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6356-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6356-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d6356-115">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6356-115">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="d6356-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6356-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6356-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6356-117">Not supported.</span></span>    |
|<span data-ttu-id="d6356-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6356-118">Application</span></span> | <span data-ttu-id="d6356-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6356-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6356-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6356-120">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
```

<span data-ttu-id="d6356-121">请求用户 id 或者 userPrincipalName 才可以访问由用户或由具有 User.ReadWrite.All 权限的用户。</span><span class="sxs-lookup"><span data-stu-id="d6356-121">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="d6356-122">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6356-122">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH https://graph.microsoft.com/beta/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="d6356-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6356-123">Request headers</span></span>

| <span data-ttu-id="d6356-124">标头</span><span class="sxs-lookup"><span data-stu-id="d6356-124">Header</span></span>       | <span data-ttu-id="d6356-125">值</span><span class="sxs-lookup"><span data-stu-id="d6356-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d6356-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6356-126">Authorization</span></span>  | <span data-ttu-id="d6356-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6356-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6356-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6356-129">Content-Type</span></span>  | <span data-ttu-id="d6356-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d6356-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6356-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6356-131">Request body</span></span>

<span data-ttu-id="d6356-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d6356-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d6356-135">属性</span><span class="sxs-lookup"><span data-stu-id="d6356-135">Property</span></span>     | <span data-ttu-id="d6356-136">类型</span><span class="sxs-lookup"><span data-stu-id="d6356-136">Type</span></span>   |<span data-ttu-id="d6356-137">说明</span><span class="sxs-lookup"><span data-stu-id="d6356-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6356-138">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="d6356-138">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="d6356-139">布尔</span><span class="sxs-lookup"><span data-stu-id="d6356-139">Boolean</span></span>|<span data-ttu-id="d6356-140">设置为 true 禁用代理人访问的[趋势](../resources/insights-trending.md)API 或禁止用户访问 Office 深入中的文档。</span><span class="sxs-lookup"><span data-stu-id="d6356-140">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="d6356-141">设置为 true 还会影响的 Office 365 中显示的内容相关性-例如，建议 SharePoint 主页中的网站和中的 OneDrive for Business 的发现视图显示相关性较低的结果。</span><span class="sxs-lookup"><span data-stu-id="d6356-141">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="d6356-142">此设置反映在[Office 深入](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)的控件状态。</span><span class="sxs-lookup"><span data-stu-id="d6356-142">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="d6356-143">示例</span><span class="sxs-lookup"><span data-stu-id="d6356-143">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="d6356-144">请求</span><span class="sxs-lookup"><span data-stu-id="d6356-144">Request</span></span>

<span data-ttu-id="d6356-145">下面是一个示例请求如何选择退出 Delve 用户并禁用其上为整个组织的内容相关性的贡献。</span><span class="sxs-lookup"><span data-stu-id="d6356-145">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="d6356-146">响应</span><span class="sxs-lookup"><span data-stu-id="d6356-146">Response</span></span>

<span data-ttu-id="d6356-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6356-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="d6356-150">批量请求</span><span class="sxs-lookup"><span data-stu-id="d6356-150">Batch request</span></span>

<span data-ttu-id="d6356-151">还有可能退出 Delve 从多个用户并禁用上为整个组织通过批处理请求的内容相关性做出贡献。</span><span class="sxs-lookup"><span data-stu-id="d6356-151">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="d6356-152">若要了解详细信息，请参阅[JSON 批处理](/graph/json-batching)。</span><span class="sxs-lookup"><span data-stu-id="d6356-152">To learn more, see [JSON batching](/graph/json-batching).</span></span>

<span data-ttu-id="d6356-153">**重要说明**： 仅[Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)角色组的成员可以更新多个用户。</span><span class="sxs-lookup"><span data-stu-id="d6356-153">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 


