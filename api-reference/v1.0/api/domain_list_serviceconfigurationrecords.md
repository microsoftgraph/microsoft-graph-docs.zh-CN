# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="7fe1b-101">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="7fe1b-101">List serviceConfigurationRecords</span></span>

<span data-ttu-id="7fe1b-102">检索启用域服务所需的 [domainDnsRecord](../resources/domaindnsrecord.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-102">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="7fe1b-p101">使用返回的列表将记录添加到域的区域文件。这可以通过域名注册机构或 DNS 服务器配置完成。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fe1b-105">权限</span><span class="sxs-lookup"><span data-stu-id="7fe1b-105">Permissions</span></span>

<span data-ttu-id="7fe1b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7fe1b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fe1b-108">Permission type</span></span>      | <span data-ttu-id="7fe1b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fe1b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fe1b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe1b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7fe1b-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fe1b-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="7fe1b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe1b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fe1b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-113">Not supported.</span></span>    |
|<span data-ttu-id="7fe1b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fe1b-114">Application</span></span> | <span data-ttu-id="7fe1b-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe1b-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fe1b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fe1b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fe1b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7fe1b-117">Optional query parameters</span></span>

<span data-ttu-id="7fe1b-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fe1b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fe1b-119">Request headers</span></span>

| <span data-ttu-id="7fe1b-120">名称</span><span class="sxs-lookup"><span data-stu-id="7fe1b-120">Name</span></span>      |<span data-ttu-id="7fe1b-121">说明</span><span class="sxs-lookup"><span data-stu-id="7fe1b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7fe1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fe1b-122">Authorization</span></span>  | <span data-ttu-id="7fe1b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fe1b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7fe1b-125">Content-Type</span></span>  | <span data-ttu-id="7fe1b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe1b-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fe1b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fe1b-127">Request body</span></span>

<span data-ttu-id="7fe1b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fe1b-129">响应</span><span class="sxs-lookup"><span data-stu-id="7fe1b-129">Response</span></span>

<span data-ttu-id="7fe1b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-130">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe1b-131">示例</span><span class="sxs-lookup"><span data-stu-id="7fe1b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fe1b-132">请求</span><span class="sxs-lookup"><span data-stu-id="7fe1b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="7fe1b-133">响应</span><span class="sxs-lookup"><span data-stu-id="7fe1b-133">Response</span></span>
<span data-ttu-id="7fe1b-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7fe1b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type":"microsoft.graph.domainDnsMxRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "@odata.type":"microsoft.graph.domainDnsTxtRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedService": "Email",
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