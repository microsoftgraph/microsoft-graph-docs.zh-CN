---
title: 更新 activitybasedtimeoutpolicy
description: 更新 activityBasedTimeoutPolicy 对象的属性。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f1ff25719bf8fa93f29f2191e63288c78af9dde9
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917097"
---
# <a name="update-activitybasedtimeoutpolicy"></a><span data-ttu-id="8052d-103">更新 activitybasedtimeoutpolicy</span><span class="sxs-lookup"><span data-stu-id="8052d-103">Update activitybasedtimeoutpolicy</span></span>

<span data-ttu-id="8052d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8052d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8052d-105">更新[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8052d-105">Update the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8052d-106">权限</span><span class="sxs-lookup"><span data-stu-id="8052d-106">Permissions</span></span>

<span data-ttu-id="8052d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8052d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8052d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8052d-109">Permission type</span></span>                        | <span data-ttu-id="8052d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8052d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8052d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8052d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8052d-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8052d-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8052d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8052d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8052d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8052d-114">Not supported.</span></span> |
| <span data-ttu-id="8052d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8052d-115">Application</span></span>                            | <span data-ttu-id="8052d-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8052d-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8052d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8052d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8052d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8052d-118">Request headers</span></span>

| <span data-ttu-id="8052d-119">名称</span><span class="sxs-lookup"><span data-stu-id="8052d-119">Name</span></span>       | <span data-ttu-id="8052d-120">说明</span><span class="sxs-lookup"><span data-stu-id="8052d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8052d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8052d-121">Authorization</span></span> | <span data-ttu-id="8052d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8052d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8052d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="8052d-124">Content-type</span></span> | <span data-ttu-id="8052d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8052d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8052d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8052d-127">Request body</span></span>

<span data-ttu-id="8052d-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8052d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8052d-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8052d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8052d-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8052d-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8052d-131">属性</span><span class="sxs-lookup"><span data-stu-id="8052d-131">Property</span></span>     | <span data-ttu-id="8052d-132">类型</span><span class="sxs-lookup"><span data-stu-id="8052d-132">Type</span></span>        | <span data-ttu-id="8052d-133">说明</span><span class="sxs-lookup"><span data-stu-id="8052d-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8052d-134">定义</span><span class="sxs-lookup"><span data-stu-id="8052d-134">definition</span></span>|<span data-ttu-id="8052d-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="8052d-135">String collection</span></span>| <span data-ttu-id="8052d-136">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="8052d-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="8052d-137">必需。</span><span class="sxs-lookup"><span data-stu-id="8052d-137">Required.</span></span>|
|<span data-ttu-id="8052d-138">description</span><span class="sxs-lookup"><span data-stu-id="8052d-138">description</span></span>|<span data-ttu-id="8052d-139">String</span><span class="sxs-lookup"><span data-stu-id="8052d-139">String</span></span>| <span data-ttu-id="8052d-140">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="8052d-140">Description for this policy.</span></span>|
|<span data-ttu-id="8052d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8052d-141">displayName</span></span>|<span data-ttu-id="8052d-142">String</span><span class="sxs-lookup"><span data-stu-id="8052d-142">String</span></span>| <span data-ttu-id="8052d-143">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8052d-143">Display name for this policy.</span></span> <span data-ttu-id="8052d-144">必需。</span><span class="sxs-lookup"><span data-stu-id="8052d-144">Required.</span></span>|
|<span data-ttu-id="8052d-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="8052d-145">isOrganizationDefault</span></span>|<span data-ttu-id="8052d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8052d-146">Boolean</span></span>|<span data-ttu-id="8052d-147">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="8052d-147">If set to true, activates this policy.</span></span> <span data-ttu-id="8052d-148">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="8052d-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="8052d-149">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="8052d-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="8052d-150">响应</span><span class="sxs-lookup"><span data-stu-id="8052d-150">Response</span></span>

<span data-ttu-id="8052d-p108">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8052d-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8052d-153">示例</span><span class="sxs-lookup"><span data-stu-id="8052d-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8052d-154">请求</span><span class="sxs-lookup"><span data-stu-id="8052d-154">Request</span></span>

<span data-ttu-id="8052d-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8052d-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8052d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="8052d-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_activitybasedtimeoutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "type": "type-value"
}
```
# <a name="c"></a>[<span data-ttu-id="8052d-157">C#</span><span class="sxs-lookup"><span data-stu-id="8052d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8052d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8052d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8052d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8052d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8052d-160">Java</span><span class="sxs-lookup"><span data-stu-id="8052d-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8052d-161">响应</span><span class="sxs-lookup"><span data-stu-id="8052d-161">Response</span></span>

<span data-ttu-id="8052d-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8052d-162">The following is an example of the response.</span></span>

> <span data-ttu-id="8052d-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8052d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update activitybasedtimeoutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
