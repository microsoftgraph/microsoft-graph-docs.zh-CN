---
title: 更新 profileCardProperty
description: 更新 profileCardProperty 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 122b8c0007067dafd2f7326cffc1b4e3b1697890
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123843"
---
# <a name="update-profilecardproperty"></a><span data-ttu-id="bb4e1-103">更新 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="bb4e1-103">Update profileCardProperty</span></span>

<span data-ttu-id="bb4e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb4e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb4e1-105">更新[profileCardProperty](../resources/profilecardproperty.md)对象的属性（由其**directoryPropertyName**属性标识）。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-105">Update the properties of a [profileCardProperty](../resources/profilecardproperty.md) object, identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb4e1-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb4e1-106">Permissions</span></span>

<span data-ttu-id="bb4e1-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bb4e1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bb4e1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb4e1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb4e1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb4e1-109">Permission type</span></span>                        | <span data-ttu-id="bb4e1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb4e1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb4e1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb4e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb4e1-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bb4e1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb4e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb4e1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-114">Not supported.</span></span>                              |
| <span data-ttu-id="bb4e1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb4e1-115">Application</span></span>                            | <span data-ttu-id="bb4e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-116">Not supported.</span></span>                              |

><span data-ttu-id="bb4e1-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="bb4e1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb4e1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bb4e1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb4e1-119">Request headers</span></span>

| <span data-ttu-id="bb4e1-120">名称</span><span class="sxs-lookup"><span data-stu-id="bb4e1-120">Name</span></span>       | <span data-ttu-id="bb4e1-121">说明</span><span class="sxs-lookup"><span data-stu-id="bb4e1-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bb4e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb4e1-122">Authorization</span></span> | <span data-ttu-id="bb4e1-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="bb4e1-123">Bearer {token}.</span></span> <span data-ttu-id="bb4e1-124">Required.</span><span class="sxs-lookup"><span data-stu-id="bb4e1-124">Required.</span></span> |
| <span data-ttu-id="bb4e1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb4e1-125">Content-Type</span></span>  | <span data-ttu-id="bb4e1-126">application/json.</span><span class="sxs-lookup"><span data-stu-id="bb4e1-126">application/json.</span></span> <span data-ttu-id="bb4e1-127">Required.</span><span class="sxs-lookup"><span data-stu-id="bb4e1-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb4e1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb4e1-128">Request body</span></span>

<span data-ttu-id="bb4e1-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bb4e1-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bb4e1-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bb4e1-132">属性</span><span class="sxs-lookup"><span data-stu-id="bb4e1-132">Property</span></span>     | <span data-ttu-id="bb4e1-133">类型</span><span class="sxs-lookup"><span data-stu-id="bb4e1-133">Type</span></span>        | <span data-ttu-id="bb4e1-134">说明</span><span class="sxs-lookup"><span data-stu-id="bb4e1-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb4e1-135">批注</span><span class="sxs-lookup"><span data-stu-id="bb4e1-135">annotations</span></span>|<span data-ttu-id="bb4e1-136">profileCardAnnotation 集合</span><span class="sxs-lookup"><span data-stu-id="bb4e1-136">profileCardAnnotation collection</span></span>| <span data-ttu-id="bb4e1-137">包含管理员已选择指定的任何可选或本地化标签。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-137">Contains any alternative or localized labels an administrator has chosen to specify.</span></span>|
|<span data-ttu-id="bb4e1-138">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="bb4e1-138">directoryPropertyName</span></span>|<span data-ttu-id="bb4e1-139">String</span><span class="sxs-lookup"><span data-stu-id="bb4e1-139">String</span></span>|<span data-ttu-id="bb4e1-140">包含用于在配置文件卡片上呈现的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-140">Contains the name of the directory property which is intended to surface on the profile card.</span></span> |

## <a name="response"></a><span data-ttu-id="bb4e1-141">响应</span><span class="sxs-lookup"><span data-stu-id="bb4e1-141">Response</span></span>

<span data-ttu-id="bb4e1-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[profileCardProperty](../resources/profilecardproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-142">If successful, this method returns a `200 OK` response code and an updated [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb4e1-143">示例</span><span class="sxs-lookup"><span data-stu-id="bb4e1-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb4e1-144">请求</span><span class="sxs-lookup"><span data-stu-id="bb4e1-144">Request</span></span>

<span data-ttu-id="bb4e1-145">下面的示例为区域设置 "无 NB" 添加本地化的标签 "Kostnads Senter"。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-145">The following example adds a localized label "Kostnads Senter" for the locale "no-NB".</span></span>

# <a name="http"></a>[<span data-ttu-id="bb4e1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb4e1-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilecardproperty"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1
Content-type: application/json

{
  "annotations": [
    {
      "localizations": [
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="bb4e1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb4e1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb4e1-148">响应</span><span class="sxs-lookup"><span data-stu-id="bb4e1-148">Response</span></span>

<span data-ttu-id="bb4e1-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb4e1-149">The following is an example of the response.</span></span>

> <span data-ttu-id="bb4e1-150">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="bb4e1-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bb4e1-151">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bb4e1-151">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        },
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilecardproperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
