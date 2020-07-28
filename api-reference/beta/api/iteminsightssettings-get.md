---
title: 获取 itemInsights
description: 检索 itemInsightsSettings 对象的属性
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: f2d22f8e74aabd975f182b8cef783f8e94ba05d7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435010"
---
# <a name="get-iteminsightssettings"></a><span data-ttu-id="e2ad1-103">获取 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="e2ad1-103">Get itemInsightsSettings</span></span>

<span data-ttu-id="e2ad1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2ad1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2ad1-105">获取[itemInsightsSettings](../resources/iteminsightssettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-105">Get the properties of [itemInsightsSettings](../resources/iteminsightssettings.md) object.</span></span>

<span data-ttu-id="e2ad1-106">若要了解如何为你的组织自定义项目见解隐私，请参阅[自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e2ad1-107">权限</span><span class="sxs-lookup"><span data-stu-id="e2ad1-107">Permissions</span></span>

<span data-ttu-id="e2ad1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2ad1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2ad1-110">Permission type</span></span>      | <span data-ttu-id="e2ad1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2ad1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2ad1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2ad1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2ad1-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2ad1-113">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="e2ad1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2ad1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2ad1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-115">Not supported.</span></span>    |
|<span data-ttu-id="e2ad1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2ad1-116">Application</span></span> | <span data-ttu-id="e2ad1-117">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2ad1-117">User.Read, User.ReadWrite</span></span>  |

><span data-ttu-id="e2ad1-118">**注意：** 对此操作使用委派权限时，需要已登录用户拥有全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="e2ad1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2ad1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="e2ad1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2ad1-120">Request headers</span></span>

| <span data-ttu-id="e2ad1-121">名称</span><span class="sxs-lookup"><span data-stu-id="e2ad1-121">Name</span></span>       | <span data-ttu-id="e2ad1-122">说明</span><span class="sxs-lookup"><span data-stu-id="e2ad1-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e2ad1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2ad1-123">Authorization</span></span>  | <span data-ttu-id="e2ad1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2ad1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2ad1-126">Request body</span></span>

<span data-ttu-id="e2ad1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2ad1-128">响应</span><span class="sxs-lookup"><span data-stu-id="e2ad1-128">Response</span></span>

<span data-ttu-id="e2ad1-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[itemInsightsSettings](../resources/iteminsightssettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-129">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="e2ad1-130">**注意：** 此操作将验证指定的**itemInsightsSettings**资源的属性值的有效性。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-130">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="e2ad1-131">如果设置了**disabledForGroup**属性，则此操作不检查是否存在相应的 Azure AD 组。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-131">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="e2ad1-132">这意味着，如果您将**disabledForGroup**设置为不存在或随后删除的 Azure AD 组，则此操作将无法识别任何组成员身份并为任何特定用户禁用项目见解。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-132">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="e2ad1-133">如果将**isEnabledInOrganization**设置为 `true` ，该操作将为组织中的所有用户启用见解。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-133">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="e2ad1-134">示例</span><span class="sxs-lookup"><span data-stu-id="e2ad1-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2ad1-135">请求</span><span class="sxs-lookup"><span data-stu-id="e2ad1-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```

##### <a name="response"></a><span data-ttu-id="e2ad1-136">响应</span><span class="sxs-lookup"><span data-stu-id="e2ad1-136">Response</span></span>

<span data-ttu-id="e2ad1-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-137">Here is an example of the response.</span></span> 
> <span data-ttu-id="e2ad1-138">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-138">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e2ad1-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2ad1-139">All of the properties will be returned from an actual call.</span></span>

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
