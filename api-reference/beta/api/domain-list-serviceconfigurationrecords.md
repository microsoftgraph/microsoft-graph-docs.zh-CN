---
title: 列出 serviceConfigurationRecords
description: 检索启用域服务所需的 domainDnsRecord 对象列表。
author: lleonard-msft
ms.openlocfilehash: d61c3d1fc877b7e4902f79d1b8f92cc1ca9ad1c8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336615"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="ad087-103">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="ad087-103">List serviceConfigurationRecords</span></span>

> <span data-ttu-id="ad087-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad087-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad087-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad087-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad087-106">检索启用域服务所需的 [domainDnsRecord](../resources/domaindnsrecord.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ad087-106">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="ad087-p102">使用返回的列表将记录添加到域的区域文件。这可以通过域名注册机构或 DNS 服务器配置完成。</span><span class="sxs-lookup"><span data-stu-id="ad087-p102">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad087-109">权限</span><span class="sxs-lookup"><span data-stu-id="ad087-109">Permissions</span></span>

<span data-ttu-id="ad087-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad087-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad087-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad087-112">Permission type</span></span>      | <span data-ttu-id="ad087-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad087-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad087-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad087-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ad087-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad087-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="ad087-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad087-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad087-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad087-117">Not supported.</span></span>    |
|<span data-ttu-id="ad087-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad087-118">Application</span></span> | <span data-ttu-id="ad087-119">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad087-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad087-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad087-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad087-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ad087-121">Optional query parameters</span></span>

<span data-ttu-id="ad087-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ad087-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad087-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad087-123">Request headers</span></span>

| <span data-ttu-id="ad087-124">Name</span><span class="sxs-lookup"><span data-stu-id="ad087-124">Name</span></span>      |<span data-ttu-id="ad087-125">说明</span><span class="sxs-lookup"><span data-stu-id="ad087-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad087-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad087-126">Authorization</span></span>  | <span data-ttu-id="ad087-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad087-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad087-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad087-129">Content-Type</span></span>  | <span data-ttu-id="ad087-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ad087-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad087-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad087-131">Request body</span></span>

<span data-ttu-id="ad087-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad087-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad087-133">响应</span><span class="sxs-lookup"><span data-stu-id="ad087-133">Response</span></span>

<span data-ttu-id="ad087-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ad087-134">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad087-135">示例</span><span class="sxs-lookup"><span data-stu-id="ad087-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad087-136">请求</span><span class="sxs-lookup"><span data-stu-id="ad087-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="ad087-137">响应</span><span class="sxs-lookup"><span data-stu-id="ad087-137">Response</span></span>
<span data-ttu-id="ad087-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad087-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->