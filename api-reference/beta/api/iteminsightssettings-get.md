---
title: 获取 itemInsights
description: 检索 itemInsightsSettings 对象的属性
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 62c1a0f2efda751153d42d985d196a69e35caee5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509635"
---
# <a name="get-iteminsightssettings"></a><span data-ttu-id="61f97-103">获取 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="61f97-103">Get itemInsightsSettings</span></span>

<span data-ttu-id="61f97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61f97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61f97-105">获取[itemInsightsSettings](../resources/iteminsightssettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="61f97-105">Get the properties of [itemInsightsSettings](../resources/iteminsightssettings.md) object.</span></span>

<span data-ttu-id="61f97-106">若要了解如何为你的组织自定义项目见解隐私，请参阅[自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="61f97-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="61f97-107">权限</span><span class="sxs-lookup"><span data-stu-id="61f97-107">Permissions</span></span>

<span data-ttu-id="61f97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61f97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61f97-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="61f97-110">Permission type</span></span>      | <span data-ttu-id="61f97-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61f97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61f97-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61f97-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61f97-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61f97-113">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="61f97-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61f97-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61f97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="61f97-115">Not supported.</span></span>    |
|<span data-ttu-id="61f97-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="61f97-116">Application</span></span> | <span data-ttu-id="61f97-117">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61f97-117">User.Read, User.ReadWrite</span></span>  |

><span data-ttu-id="61f97-118">**注意：** 对此操作使用委派权限时，需要已登录用户拥有全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="61f97-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="61f97-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61f97-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="61f97-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="61f97-120">Request headers</span></span>

| <span data-ttu-id="61f97-121">名称</span><span class="sxs-lookup"><span data-stu-id="61f97-121">Name</span></span>       | <span data-ttu-id="61f97-122">说明</span><span class="sxs-lookup"><span data-stu-id="61f97-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="61f97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61f97-123">Authorization</span></span>  | <span data-ttu-id="61f97-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61f97-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61f97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="61f97-126">Request body</span></span>

<span data-ttu-id="61f97-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61f97-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61f97-128">响应</span><span class="sxs-lookup"><span data-stu-id="61f97-128">Response</span></span>

<span data-ttu-id="61f97-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[itemInsightsSettings](../resources/iteminsightssettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="61f97-129">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="61f97-130">**注意：** 此操作将验证指定的**itemInsightsSettings**资源的属性值的有效性。</span><span class="sxs-lookup"><span data-stu-id="61f97-130">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="61f97-131">如果设置了**disabledForGroup**属性，则此操作不检查是否存在相应的 Azure AD 组。</span><span class="sxs-lookup"><span data-stu-id="61f97-131">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="61f97-132">这意味着，如果您将**disabledForGroup**设置为不存在或随后删除的 Azure AD 组，则此操作将无法识别任何组成员身份并为任何特定用户禁用项目见解。</span><span class="sxs-lookup"><span data-stu-id="61f97-132">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="61f97-133">如果将**isEnabledInOrganization**设置为 `true` ，该操作将为组织中的所有用户启用见解。</span><span class="sxs-lookup"><span data-stu-id="61f97-133">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="61f97-134">示例</span><span class="sxs-lookup"><span data-stu-id="61f97-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="61f97-135">请求</span><span class="sxs-lookup"><span data-stu-id="61f97-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="61f97-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="61f97-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="61f97-137">C#</span><span class="sxs-lookup"><span data-stu-id="61f97-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61f97-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61f97-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61f97-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61f97-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="61f97-140">响应</span><span class="sxs-lookup"><span data-stu-id="61f97-140">Response</span></span>

<span data-ttu-id="61f97-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="61f97-141">Here is an example of the response.</span></span> 
> <span data-ttu-id="61f97-142">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="61f97-142">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="61f97-143">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61f97-143">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "get_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
