---
title: 更新 onPremisesPublishingProfile
description: 更新 onPremisesPublishingProfile 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b4d2eac82b47549633b03c39465e4107e4fcd8b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414497"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="59230-103">更新 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="59230-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59230-104">更新[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="59230-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59230-105">权限</span><span class="sxs-lookup"><span data-stu-id="59230-105">Permissions</span></span>

<span data-ttu-id="59230-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59230-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="59230-108">Permission type</span></span>                        | <span data-ttu-id="59230-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59230-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="59230-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59230-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="59230-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="59230-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="59230-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59230-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59230-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="59230-113">Not supported.</span></span> |
| <span data-ttu-id="59230-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="59230-114">Application</span></span>                            | <span data-ttu-id="59230-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59230-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59230-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59230-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="59230-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="59230-117">Request headers</span></span>

| <span data-ttu-id="59230-118">名称</span><span class="sxs-lookup"><span data-stu-id="59230-118">Name</span></span>       | <span data-ttu-id="59230-119">说明</span><span class="sxs-lookup"><span data-stu-id="59230-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="59230-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="59230-120">Authorization</span></span> | <span data-ttu-id="59230-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="59230-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="59230-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="59230-122">Request body</span></span>

<span data-ttu-id="59230-123">在请求正文中, 提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="59230-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="59230-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="59230-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="59230-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="59230-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59230-126">属性</span><span class="sxs-lookup"><span data-stu-id="59230-126">Property</span></span>     | <span data-ttu-id="59230-127">类型</span><span class="sxs-lookup"><span data-stu-id="59230-127">Type</span></span>        | <span data-ttu-id="59230-128">说明</span><span class="sxs-lookup"><span data-stu-id="59230-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59230-129">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="59230-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="59230-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="59230-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="59230-131">表示[hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="59230-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="59230-132">响应</span><span class="sxs-lookup"><span data-stu-id="59230-132">Response</span></span>

<span data-ttu-id="59230-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="59230-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="59230-134">示例</span><span class="sxs-lookup"><span data-stu-id="59230-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="59230-135">示例 1: 更新 hybridAgentUpdaterConfiguration 中的 updateWindow</span><span class="sxs-lookup"><span data-stu-id="59230-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="59230-136">下面的示例更新**hybridAgentUpdaterConfiguration**中的**updateWindow** 。</span><span class="sxs-lookup"><span data-stu-id="59230-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="59230-137">请求</span><span class="sxs-lookup"><span data-stu-id="59230-137">Request</span></span>

<span data-ttu-id="59230-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59230-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59230-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="59230-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
   "updateWindow" :
{
      "updateWindowStartTime" : "0:00:00",
      "updateWindowEndTime" : "23:59:00"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59230-140">C#</span><span class="sxs-lookup"><span data-stu-id="59230-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59230-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59230-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59230-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="59230-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="59230-143">响应</span><span class="sxs-lookup"><span data-stu-id="59230-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="59230-144">示例 2: 更新 hybridAgentUpdaterConfiguration 中的 deferUpdate</span><span class="sxs-lookup"><span data-stu-id="59230-144">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="59230-145">下面的示例更新**hybridAgentUpdaterConfiguration**中的**deferUpdate** 。</span><span class="sxs-lookup"><span data-stu-id="59230-145">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="59230-146">请求</span><span class="sxs-lookup"><span data-stu-id="59230-146">Request</span></span>

<span data-ttu-id="59230-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59230-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```

#### <a name="response"></a><span data-ttu-id="59230-148">响应</span><span class="sxs-lookup"><span data-stu-id="59230-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="59230-149">示例 3: 更新 hybridAgentUpdaterConfiguration 中的 allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="59230-149">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="59230-150">下面的示例更新**hybridAgentUpdaterConfiguration**中的**allowUpdateConfigurationOverride** 。</span><span class="sxs-lookup"><span data-stu-id="59230-150">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="59230-151">请求</span><span class="sxs-lookup"><span data-stu-id="59230-151">Request</span></span>

<span data-ttu-id="59230-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59230-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```

#### <a name="response"></a><span data-ttu-id="59230-153">响应</span><span class="sxs-lookup"><span data-stu-id="59230-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisespublishingprofile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
