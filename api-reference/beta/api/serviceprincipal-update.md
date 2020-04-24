---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 3eba71074da995f635b89e011b138b6563671309
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805955"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="7130c-103">更新 serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="7130c-103">Update serviceprincipal</span></span>

<span data-ttu-id="7130c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7130c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7130c-105">更新 serviceprincipal 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7130c-105">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7130c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7130c-106">Permissions</span></span>
<span data-ttu-id="7130c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7130c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7130c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7130c-109">Permission type</span></span>      | <span data-ttu-id="7130c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7130c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7130c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7130c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7130c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7130c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7130c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7130c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7130c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7130c-114">Not supported.</span></span>    |
|<span data-ttu-id="7130c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7130c-115">Application</span></span> | <span data-ttu-id="7130c-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7130c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7130c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7130c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7130c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7130c-118">Request headers</span></span>
| <span data-ttu-id="7130c-119">名称</span><span class="sxs-lookup"><span data-stu-id="7130c-119">Name</span></span>       | <span data-ttu-id="7130c-120">类型</span><span class="sxs-lookup"><span data-stu-id="7130c-120">Type</span></span> | <span data-ttu-id="7130c-121">说明</span><span class="sxs-lookup"><span data-stu-id="7130c-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7130c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7130c-122">Authorization</span></span>  | <span data-ttu-id="7130c-123">string</span><span class="sxs-lookup"><span data-stu-id="7130c-123">string</span></span>  | <span data-ttu-id="7130c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7130c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7130c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7130c-126">Request body</span></span>
<span data-ttu-id="7130c-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7130c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7130c-130">属性</span><span class="sxs-lookup"><span data-stu-id="7130c-130">Property</span></span>     | <span data-ttu-id="7130c-131">类型</span><span class="sxs-lookup"><span data-stu-id="7130c-131">Type</span></span>   |<span data-ttu-id="7130c-132">说明</span><span class="sxs-lookup"><span data-stu-id="7130c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7130c-133">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7130c-133">accountEnabled</span></span>|<span data-ttu-id="7130c-134">布尔</span><span class="sxs-lookup"><span data-stu-id="7130c-134">Boolean</span></span>|                <span data-ttu-id="7130c-135">如果服务主体帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="7130c-135">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="7130c-136">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="7130c-136">appDisplayName</span></span>|<span data-ttu-id="7130c-137">String</span><span class="sxs-lookup"><span data-stu-id="7130c-137">String</span></span>|<span data-ttu-id="7130c-138">关联应用程序公开的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7130c-138">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="7130c-139">appId</span><span class="sxs-lookup"><span data-stu-id="7130c-139">appId</span></span>|<span data-ttu-id="7130c-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-140">String</span></span>|<span data-ttu-id="7130c-141">关联应用程序的唯一标识符（其 **appId** 属性）。</span><span class="sxs-lookup"><span data-stu-id="7130c-141">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="7130c-142">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="7130c-142">appRoleAssignmentRequired</span></span>|<span data-ttu-id="7130c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="7130c-143">Boolean</span></span>|<span data-ttu-id="7130c-144">指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。</span><span class="sxs-lookup"><span data-stu-id="7130c-144">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="7130c-145">**注释**：需要版本1.5 或更高版本，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-145">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="7130c-146">appRoles</span><span class="sxs-lookup"><span data-stu-id="7130c-146">appRoles</span></span>|<span data-ttu-id="7130c-147">appRole</span><span class="sxs-lookup"><span data-stu-id="7130c-147">appRole</span></span>|<span data-ttu-id="7130c-148">关联应用程序公开的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="7130c-148">The application roles exposed by the associated application.</span></span> <span data-ttu-id="7130c-149">有关详细信息，请参阅 application entity **Notes**上的**appRoles**属性定义：需要版本1.5 或更高版本，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-149">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="7130c-150">displayName</span><span class="sxs-lookup"><span data-stu-id="7130c-150">displayName</span></span>|<span data-ttu-id="7130c-151">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-151">String</span></span>|<span data-ttu-id="7130c-152">服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7130c-152">The display name for the service principal.</span></span>|
|<span data-ttu-id="7130c-153">errorUrl</span><span class="sxs-lookup"><span data-stu-id="7130c-153">errorUrl</span></span>|<span data-ttu-id="7130c-154">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-154">String</span></span>|            |
|<span data-ttu-id="7130c-155">homepage</span><span class="sxs-lookup"><span data-stu-id="7130c-155">homepage</span></span>|<span data-ttu-id="7130c-156">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-156">String</span></span>|<span data-ttu-id="7130c-157">关联应用程序的主页的 URL。</span><span class="sxs-lookup"><span data-stu-id="7130c-157">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="7130c-158">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="7130c-158">keyCredentials</span></span>|<span data-ttu-id="7130c-159">keyCredential</span><span class="sxs-lookup"><span data-stu-id="7130c-159">keyCredential</span></span>|<span data-ttu-id="7130c-160">与服务帐户关联的密钥凭据集合。</span><span class="sxs-lookup"><span data-stu-id="7130c-160">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="7130c-161">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-161">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="7130c-162">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="7130c-162">logoutUrl</span></span>|<span data-ttu-id="7130c-163">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-163">String</span></span>| <span data-ttu-id="7130c-164">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="7130c-164">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="7130c-165">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="7130c-165">oauth2Permissions</span></span>|<span data-ttu-id="7130c-166">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="7130c-166">oAuth2Permission</span></span>|<span data-ttu-id="7130c-167">关联应用程序的 OAuth 2.0 权限。</span><span class="sxs-lookup"><span data-stu-id="7130c-167">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="7130c-168">有关详细信息，请参阅应用程序实体上的 **oauth2Permissions** 属性定义。</span><span class="sxs-lookup"><span data-stu-id="7130c-168">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="7130c-169">**注释**：需要版本1.5 或更高版本，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-169">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="7130c-170">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="7130c-170">passwordCredentials</span></span>|<span data-ttu-id="7130c-171">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="7130c-171">passwordCredential</span></span>|<span data-ttu-id="7130c-172">与服务帐户关联的密码凭据集合。</span><span class="sxs-lookup"><span data-stu-id="7130c-172">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="7130c-173">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-173">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="7130c-174">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="7130c-174">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="7130c-175">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-175">String</span></span>|<span data-ttu-id="7130c-176">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="7130c-176">Reserved for internal use only.</span></span> <span data-ttu-id="7130c-177">请勿写入属性，否则将依赖该属性。</span><span class="sxs-lookup"><span data-stu-id="7130c-177">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="7130c-178">可能会在未来版本中删除。</span><span class="sxs-lookup"><span data-stu-id="7130c-178">May be removed in future versions.</span></span>                            <span data-ttu-id="7130c-179">**备注**：需要1.5 版或更高版本。</span><span class="sxs-lookup"><span data-stu-id="7130c-179">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="7130c-180">publisherName</span><span class="sxs-lookup"><span data-stu-id="7130c-180">publisherName</span></span>|<span data-ttu-id="7130c-181">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-181">String</span></span>|<span data-ttu-id="7130c-182">在其中指定关联应用程序的租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7130c-182">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="7130c-183">replyUrls</span><span class="sxs-lookup"><span data-stu-id="7130c-183">replyUrls</span></span>|<span data-ttu-id="7130c-184">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-184">String</span></span>|<span data-ttu-id="7130c-185">向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="7130c-185">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="7130c-186">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-186">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="7130c-187">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="7130c-187">samlMetadataUrl</span></span>|<span data-ttu-id="7130c-188">String</span><span class="sxs-lookup"><span data-stu-id="7130c-188">String</span></span>|            |
|<span data-ttu-id="7130c-189">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="7130c-189">servicePrincipalNames</span></span>|<span data-ttu-id="7130c-190">字符串</span><span class="sxs-lookup"><span data-stu-id="7130c-190">String</span></span>|<span data-ttu-id="7130c-191">标识关联应用程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="7130c-191">The URIs that identify the associated application.</span></span> <span data-ttu-id="7130c-192">有关详细信息，请参阅[应用程序对象和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="7130c-192">For more information, see [Application Objects and Service Principal Objects](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span>                            <span data-ttu-id="7130c-193">**备注**：不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-193">**Notes**: Not nullable.</span></span> <span data-ttu-id="7130c-194">多值属性上的筛选表达式需要**any**运算符;有关详细信息，请参阅[支持的查询、筛选器和分页选项](https://docs.microsoft.com/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-supported-queries-filters-and-paging-options)。</span><span class="sxs-lookup"><span data-stu-id="7130c-194">The **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://docs.microsoft.com/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-supported-queries-filters-and-paging-options).</span></span>            |
|<span data-ttu-id="7130c-195">tags</span><span class="sxs-lookup"><span data-stu-id="7130c-195">tags</span></span>|<span data-ttu-id="7130c-196">String</span><span class="sxs-lookup"><span data-stu-id="7130c-196">String</span></span>|                                        <span data-ttu-id="7130c-197">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="7130c-197">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="7130c-198">响应</span><span class="sxs-lookup"><span data-stu-id="7130c-198">Response</span></span>

<span data-ttu-id="7130c-199">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7130c-199">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7130c-200">示例</span><span class="sxs-lookup"><span data-stu-id="7130c-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7130c-201">请求</span><span class="sxs-lookup"><span data-stu-id="7130c-201">Request</span></span>
<span data-ttu-id="7130c-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7130c-202">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7130c-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="7130c-203">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7130c-204">C#</span><span class="sxs-lookup"><span data-stu-id="7130c-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7130c-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7130c-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7130c-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7130c-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7130c-207">响应</span><span class="sxs-lookup"><span data-stu-id="7130c-207">Response</span></span>
<span data-ttu-id="7130c-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7130c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
