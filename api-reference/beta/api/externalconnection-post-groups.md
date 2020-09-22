---
title: 创建 externalGroup
description: 创建新的 externalGroup 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: fb836591b86972144f3ff632f807f7e1d4c0e82c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193853"
---
# <a name="create-externalgroup"></a><span data-ttu-id="2f24b-103">创建 externalGroup</span><span class="sxs-lookup"><span data-stu-id="2f24b-103">Create externalGroup</span></span>

<span data-ttu-id="2f24b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f24b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f24b-105">创建新的 [externalGroup](../resources/externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f24b-105">Create a new [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f24b-106">权限</span><span class="sxs-lookup"><span data-stu-id="2f24b-106">Permissions</span></span>

<span data-ttu-id="2f24b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f24b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f24b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f24b-109">Permission type</span></span>                        | <span data-ttu-id="2f24b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f24b-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f24b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f24b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f24b-112">不支持</span><span class="sxs-lookup"><span data-stu-id="2f24b-112">Not supported</span></span>                               |
| <span data-ttu-id="2f24b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f24b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f24b-114">不支持</span><span class="sxs-lookup"><span data-stu-id="2f24b-114">Not supported</span></span>                               |
| <span data-ttu-id="2f24b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f24b-115">Application</span></span>                            | <span data-ttu-id="2f24b-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f24b-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="2f24b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f24b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a><span data-ttu-id="2f24b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f24b-118">Request headers</span></span>

| <span data-ttu-id="2f24b-119">名称</span><span class="sxs-lookup"><span data-stu-id="2f24b-119">Name</span></span>          | <span data-ttu-id="2f24b-120">说明</span><span class="sxs-lookup"><span data-stu-id="2f24b-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="2f24b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f24b-121">Authorization</span></span> | <span data-ttu-id="2f24b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f24b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2f24b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f24b-124">Content-Type</span></span>  | <span data-ttu-id="2f24b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2f24b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f24b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f24b-127">Request body</span></span>

<span data-ttu-id="2f24b-128">在请求正文中，提供 [externalGroup](../resources/externalgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f24b-128">In the request body, supply a JSON representation of the [externalGroup](../resources/externalgroup.md) object.</span></span>

<span data-ttu-id="2f24b-129">下表显示创建 [externalGroup](../resources/externalgroup.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f24b-129">The following table shows the properties that are required when you create the [externalGroup](../resources/externalgroup.md).</span></span>

| <span data-ttu-id="2f24b-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f24b-130">Property</span></span>    | <span data-ttu-id="2f24b-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f24b-131">Type</span></span>   | <span data-ttu-id="2f24b-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f24b-132">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2f24b-133">id</span><span class="sxs-lookup"><span data-stu-id="2f24b-133">id</span></span>          | <span data-ttu-id="2f24b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2f24b-134">String</span></span> | <span data-ttu-id="2f24b-135">连接中的外部组的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2f24b-135">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="2f24b-136">它必须是字母数字，最长可为128个字符。</span><span class="sxs-lookup"><span data-stu-id="2f24b-136">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="2f24b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2f24b-137">displayName</span></span> | <span data-ttu-id="2f24b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2f24b-138">String</span></span> | <span data-ttu-id="2f24b-139">外部组的友好名称。</span><span class="sxs-lookup"><span data-stu-id="2f24b-139">The friendly name of the external group.</span></span> <span data-ttu-id="2f24b-140">可选。</span><span class="sxs-lookup"><span data-stu-id="2f24b-140">Optional.</span></span>                                                                      |
| <span data-ttu-id="2f24b-141">说明</span><span class="sxs-lookup"><span data-stu-id="2f24b-141">description</span></span> | <span data-ttu-id="2f24b-142">字符串</span><span class="sxs-lookup"><span data-stu-id="2f24b-142">String</span></span> | <span data-ttu-id="2f24b-143">外部组的说明。</span><span class="sxs-lookup"><span data-stu-id="2f24b-143">The description of the external group.</span></span> <span data-ttu-id="2f24b-144">可选。</span><span class="sxs-lookup"><span data-stu-id="2f24b-144">Optional.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="2f24b-145">响应</span><span class="sxs-lookup"><span data-stu-id="2f24b-145">Response</span></span>

<span data-ttu-id="2f24b-146">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [externalGroup](../resources/externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f24b-146">If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f24b-147">示例</span><span class="sxs-lookup"><span data-stu-id="2f24b-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f24b-148">请求</span><span class="sxs-lookup"><span data-stu-id="2f24b-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="2f24b-149">响应</span><span class="sxs-lookup"><span data-stu-id="2f24b-149">Response</span></span>

<span data-ttu-id="2f24b-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2f24b-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
