---
title: 列表策略
description: 检索目录中的所有 policy 对象。
localization_priority: Normal
ms.openlocfilehash: 292eb457b87629d0034b97b3c781d75adc0da4e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538706"
---
# <a name="list-policies"></a><span data-ttu-id="af73b-103">列表策略</span><span class="sxs-lookup"><span data-stu-id="af73b-103">List Policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af73b-104">检索目录中的所有[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="af73b-104">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="af73b-105">权限</span><span class="sxs-lookup"><span data-stu-id="af73b-105">Permissions</span></span>
<span data-ttu-id="af73b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af73b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="af73b-108">Permission type</span></span>      | <span data-ttu-id="af73b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af73b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af73b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af73b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af73b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af73b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af73b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af73b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af73b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="af73b-113">Not supported.</span></span>    |
|<span data-ttu-id="af73b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="af73b-114">Application</span></span> | <span data-ttu-id="af73b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="af73b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af73b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af73b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="af73b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="af73b-117">Request headers</span></span>
| <span data-ttu-id="af73b-118">名称</span><span class="sxs-lookup"><span data-stu-id="af73b-118">Name</span></span>       | <span data-ttu-id="af73b-119">类型</span><span class="sxs-lookup"><span data-stu-id="af73b-119">Type</span></span> | <span data-ttu-id="af73b-120">说明</span><span class="sxs-lookup"><span data-stu-id="af73b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="af73b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af73b-121">Authorization</span></span>  | <span data-ttu-id="af73b-122">string</span><span class="sxs-lookup"><span data-stu-id="af73b-122">string</span></span>  | <span data-ttu-id="af73b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="af73b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af73b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="af73b-125">Request body</span></span>
<span data-ttu-id="af73b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af73b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af73b-127">响应</span><span class="sxs-lookup"><span data-stu-id="af73b-127">Response</span></span>

<span data-ttu-id="af73b-128">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="af73b-128">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="af73b-129">如果不成功 .。。</span><span class="sxs-lookup"><span data-stu-id="af73b-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="af73b-130">示例</span><span class="sxs-lookup"><span data-stu-id="af73b-130">Example</span></span>
<span data-ttu-id="af73b-131">下面的示例检索所有策略。</span><span class="sxs-lookup"><span data-stu-id="af73b-131">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="af73b-132">请求</span><span class="sxs-lookup"><span data-stu-id="af73b-132">Request</span></span>
<span data-ttu-id="af73b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af73b-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="af73b-134">响应</span><span class="sxs-lookup"><span data-stu-id="af73b-134">Response</span></span>
<span data-ttu-id="af73b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af73b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "value":[
        {
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
