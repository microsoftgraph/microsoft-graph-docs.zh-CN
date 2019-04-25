---
title: 获取 synchronizationTemplate
description: 按其标识符检索同步模板。
localization_priority: Normal
ms.openlocfilehash: 4fc13ee5d83d6501f75bb45ce69f189b8809270c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545167"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="05598-103">获取 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="05598-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05598-104">按其标识符检索同步模板。</span><span class="sxs-lookup"><span data-stu-id="05598-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="05598-105">权限</span><span class="sxs-lookup"><span data-stu-id="05598-105">Permissions</span></span>
<span data-ttu-id="05598-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05598-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="05598-108">Permission type</span></span>                        | <span data-ttu-id="05598-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05598-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="05598-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05598-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="05598-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05598-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="05598-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05598-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="05598-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="05598-113">Not supported.</span></span>|
|<span data-ttu-id="05598-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="05598-114">Application</span></span>                            |<span data-ttu-id="05598-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="05598-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="05598-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05598-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="05598-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="05598-117">Request headers</span></span>

| <span data-ttu-id="05598-118">名称</span><span class="sxs-lookup"><span data-stu-id="05598-118">Name</span></span>           | <span data-ttu-id="05598-119">类型</span><span class="sxs-lookup"><span data-stu-id="05598-119">Type</span></span>    | <span data-ttu-id="05598-120">说明</span><span class="sxs-lookup"><span data-stu-id="05598-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="05598-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05598-121">Authorization</span></span>  | <span data-ttu-id="05598-122">string</span><span class="sxs-lookup"><span data-stu-id="05598-122">string</span></span>  | <span data-ttu-id="05598-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05598-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05598-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="05598-125">Request body</span></span>

<span data-ttu-id="05598-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05598-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="05598-127">响应</span><span class="sxs-lookup"><span data-stu-id="05598-127">Response</span></span>

<span data-ttu-id="05598-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="05598-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="05598-129">示例</span><span class="sxs-lookup"><span data-stu-id="05598-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="05598-130">请求</span><span class="sxs-lookup"><span data-stu-id="05598-130">Request</span></span>
<span data-ttu-id="05598-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="05598-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="05598-132">响应</span><span class="sxs-lookup"><span data-stu-id="05598-132">Response</span></span>
<span data-ttu-id="05598-133">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="05598-133">The following is an example of a response.</span></span>
><span data-ttu-id="05598-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="05598-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="05598-135">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="05598-135">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
