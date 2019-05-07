---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Normal
ms.openlocfilehash: e2caffafe114f0023a849cecef98f8173bf6468f
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638632"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="6ff83-103">更新 serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="6ff83-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ff83-104">更新 serviceprincipal 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6ff83-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ff83-105">权限</span><span class="sxs-lookup"><span data-stu-id="6ff83-105">Permissions</span></span>
<span data-ttu-id="6ff83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ff83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff83-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ff83-108">Permission type</span></span>      | <span data-ttu-id="6ff83-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ff83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ff83-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ff83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ff83-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ff83-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ff83-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ff83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ff83-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ff83-113">Not supported.</span></span>    |
|<span data-ttu-id="6ff83-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ff83-114">Application</span></span> | <span data-ttu-id="6ff83-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ff83-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ff83-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ff83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6ff83-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ff83-117">Request headers</span></span>
| <span data-ttu-id="6ff83-118">名称</span><span class="sxs-lookup"><span data-stu-id="6ff83-118">Name</span></span>       | <span data-ttu-id="6ff83-119">类型</span><span class="sxs-lookup"><span data-stu-id="6ff83-119">Type</span></span> | <span data-ttu-id="6ff83-120">说明</span><span class="sxs-lookup"><span data-stu-id="6ff83-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6ff83-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ff83-121">Authorization</span></span>  | <span data-ttu-id="6ff83-122">string</span><span class="sxs-lookup"><span data-stu-id="6ff83-122">string</span></span>  | <span data-ttu-id="6ff83-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ff83-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ff83-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ff83-125">Request body</span></span>
<span data-ttu-id="6ff83-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6ff83-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6ff83-129">属性</span><span class="sxs-lookup"><span data-stu-id="6ff83-129">Property</span></span>     | <span data-ttu-id="6ff83-130">类型</span><span class="sxs-lookup"><span data-stu-id="6ff83-130">Type</span></span>   |<span data-ttu-id="6ff83-131">说明</span><span class="sxs-lookup"><span data-stu-id="6ff83-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ff83-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="6ff83-132">accountEnabled</span></span>|<span data-ttu-id="6ff83-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff83-133">Boolean</span></span>|                <span data-ttu-id="6ff83-134">如果服务主体帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="6ff83-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="6ff83-135">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="6ff83-135">appDisplayName</span></span>|<span data-ttu-id="6ff83-136">String</span><span class="sxs-lookup"><span data-stu-id="6ff83-136">String</span></span>|<span data-ttu-id="6ff83-137">关联应用程序公开的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ff83-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="6ff83-138">appId</span><span class="sxs-lookup"><span data-stu-id="6ff83-138">appId</span></span>|<span data-ttu-id="6ff83-139">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-139">String</span></span>|<span data-ttu-id="6ff83-140">关联应用程序的唯一标识符（其 **appId** 属性）。</span><span class="sxs-lookup"><span data-stu-id="6ff83-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="6ff83-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="6ff83-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="6ff83-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff83-142">Boolean</span></span>|<span data-ttu-id="6ff83-143">指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。</span><span class="sxs-lookup"><span data-stu-id="6ff83-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="6ff83-144">**注释**: 需要版本1.5 或更高版本, 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="6ff83-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="6ff83-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="6ff83-145">appRoles</span></span>|<span data-ttu-id="6ff83-146">appRole</span><span class="sxs-lookup"><span data-stu-id="6ff83-146">appRole</span></span>|<span data-ttu-id="6ff83-147">关联应用程序公开的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="6ff83-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="6ff83-148">有关详细信息, 请参阅 application entity **Notes**上的**appRoles**属性定义: 需要版本1.5 或更高版本, 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="6ff83-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="6ff83-149">displayName</span><span class="sxs-lookup"><span data-stu-id="6ff83-149">displayName</span></span>|<span data-ttu-id="6ff83-150">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-150">String</span></span>|<span data-ttu-id="6ff83-151">服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ff83-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="6ff83-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="6ff83-152">errorUrl</span></span>|<span data-ttu-id="6ff83-153">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-153">String</span></span>|            |
|<span data-ttu-id="6ff83-154">homepage</span><span class="sxs-lookup"><span data-stu-id="6ff83-154">homepage</span></span>|<span data-ttu-id="6ff83-155">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-155">String</span></span>|<span data-ttu-id="6ff83-156">关联应用程序的主页的 URL。</span><span class="sxs-lookup"><span data-stu-id="6ff83-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="6ff83-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="6ff83-157">keyCredentials</span></span>|<span data-ttu-id="6ff83-158">keyCredential</span><span class="sxs-lookup"><span data-stu-id="6ff83-158">keyCredential</span></span>|<span data-ttu-id="6ff83-159">与服务帐户关联的密钥凭据集合。</span><span class="sxs-lookup"><span data-stu-id="6ff83-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="6ff83-160">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="6ff83-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="6ff83-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="6ff83-161">logoutUrl</span></span>|<span data-ttu-id="6ff83-162">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-162">String</span></span>| <span data-ttu-id="6ff83-163">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="6ff83-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="6ff83-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="6ff83-164">oauth2Permissions</span></span>|<span data-ttu-id="6ff83-165">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="6ff83-165">oAuth2Permission</span></span>|<span data-ttu-id="6ff83-166">关联应用程序的 OAuth 2.0 权限。</span><span class="sxs-lookup"><span data-stu-id="6ff83-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="6ff83-167">有关详细信息，请参阅应用程序实体上的 **oauth2Permissions** 属性定义。</span><span class="sxs-lookup"><span data-stu-id="6ff83-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="6ff83-168">**注释**: 需要版本1.5 或更高版本, 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="6ff83-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="6ff83-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="6ff83-169">passwordCredentials</span></span>|<span data-ttu-id="6ff83-170">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="6ff83-170">passwordCredential</span></span>|<span data-ttu-id="6ff83-171">与服务帐户关联的密码凭据集合。</span><span class="sxs-lookup"><span data-stu-id="6ff83-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="6ff83-172">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="6ff83-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="6ff83-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="6ff83-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="6ff83-174">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-174">String</span></span>|<span data-ttu-id="6ff83-175">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="6ff83-175">Reserved for internal use only.</span></span> <span data-ttu-id="6ff83-176">请勿写入属性，否则将依赖该属性。</span><span class="sxs-lookup"><span data-stu-id="6ff83-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="6ff83-177">可能会在未来版本中删除。</span><span class="sxs-lookup"><span data-stu-id="6ff83-177">May be removed in future versions.</span></span>                            <span data-ttu-id="6ff83-178">**备注**: 需要1.5 版或更高版本。</span><span class="sxs-lookup"><span data-stu-id="6ff83-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="6ff83-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="6ff83-179">publisherName</span></span>|<span data-ttu-id="6ff83-180">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-180">String</span></span>|<span data-ttu-id="6ff83-181">在其中指定关联应用程序的租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ff83-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="6ff83-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="6ff83-182">replyUrls</span></span>|<span data-ttu-id="6ff83-183">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-183">String</span></span>|<span data-ttu-id="6ff83-184">向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="6ff83-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="6ff83-185">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="6ff83-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="6ff83-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="6ff83-186">samlMetadataUrl</span></span>|<span data-ttu-id="6ff83-187">String</span><span class="sxs-lookup"><span data-stu-id="6ff83-187">String</span></span>|            |
|<span data-ttu-id="6ff83-188">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="6ff83-188">servicePrincipalNames</span></span>|<span data-ttu-id="6ff83-189">字符串</span><span class="sxs-lookup"><span data-stu-id="6ff83-189">String</span></span>|<span data-ttu-id="6ff83-190">标识关联应用程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="6ff83-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="6ff83-191">有关详细信息，请参阅[应用程序对象和服务主体对象](https://msdn.microsoft.com/library/azure/dn132633.aspx)。</span><span class="sxs-lookup"><span data-stu-id="6ff83-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="6ff83-192">**注释**: 不可为 null, 多值属性上的筛选表达式需要**any**运算符;有关详细信息, 请参阅[支持的查询、筛选器和分页选项](https://msdn.microsoft.com/library/azure/dn727074.aspx)。</span><span class="sxs-lookup"><span data-stu-id="6ff83-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="6ff83-193">tags</span><span class="sxs-lookup"><span data-stu-id="6ff83-193">tags</span></span>|<span data-ttu-id="6ff83-194">String</span><span class="sxs-lookup"><span data-stu-id="6ff83-194">String</span></span>|                                        <span data-ttu-id="6ff83-195">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="6ff83-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="6ff83-196">响应</span><span class="sxs-lookup"><span data-stu-id="6ff83-196">Response</span></span>

<span data-ttu-id="6ff83-197">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6ff83-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ff83-198">示例</span><span class="sxs-lookup"><span data-stu-id="6ff83-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ff83-199">请求</span><span class="sxs-lookup"><span data-stu-id="6ff83-199">Request</span></span>
<span data-ttu-id="6ff83-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ff83-200">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="6ff83-201">响应</span><span class="sxs-lookup"><span data-stu-id="6ff83-201">Response</span></span>
<span data-ttu-id="6ff83-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ff83-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ff83-205">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6ff83-205">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6ff83-206">语言</span><span class="sxs-lookup"><span data-stu-id="6ff83-206">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_serviceprincipal-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ff83-207">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ff83-207">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_serviceprincipal-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
