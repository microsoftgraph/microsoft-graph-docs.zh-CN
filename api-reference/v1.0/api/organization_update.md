# <a name="update-organization"></a><span data-ttu-id="fd18f-101">更新组织</span><span class="sxs-lookup"><span data-stu-id="fd18f-101">Update organization</span></span>

<span data-ttu-id="fd18f-102">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="fd18f-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd18f-103">权限</span><span class="sxs-lookup"><span data-stu-id="fd18f-103">Permissions</span></span>

<span data-ttu-id="fd18f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fd18f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd18f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd18f-106">Permission type</span></span> | <span data-ttu-id="fd18f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd18f-107">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd18f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd18f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fd18f-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd18f-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd18f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd18f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd18f-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd18f-111">Not supported.</span></span>    |
|<span data-ttu-id="fd18f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd18f-112">Application</span></span> | <span data-ttu-id="fd18f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd18f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd18f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd18f-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="fd18f-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd18f-115">Request headers</span></span>

| <span data-ttu-id="fd18f-116">名称</span><span class="sxs-lookup"><span data-stu-id="fd18f-116">Name</span></span>       | <span data-ttu-id="fd18f-117">类型</span><span class="sxs-lookup"><span data-stu-id="fd18f-117">Type</span></span> | <span data-ttu-id="fd18f-118">说明</span><span class="sxs-lookup"><span data-stu-id="fd18f-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd18f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd18f-119">Authorization</span></span>  | <span data-ttu-id="fd18f-120">string</span><span class="sxs-lookup"><span data-stu-id="fd18f-120">string</span></span>  | <span data-ttu-id="fd18f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd18f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd18f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd18f-123">Request body</span></span>
<span data-ttu-id="fd18f-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="fd18f-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="fd18f-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="fd18f-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fd18f-126">为了实现最佳性能，不得添加尚未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="fd18f-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fd18f-127">属性</span><span class="sxs-lookup"><span data-stu-id="fd18f-127">Property</span></span>     | <span data-ttu-id="fd18f-128">类型</span><span class="sxs-lookup"><span data-stu-id="fd18f-128">Type</span></span>   |<span data-ttu-id="fd18f-129">说明</span><span class="sxs-lookup"><span data-stu-id="fd18f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd18f-130">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="fd18f-130">marketingNotificationEmails</span></span>|<span data-ttu-id="fd18f-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="fd18f-131">String collection</span></span>|                                        <span data-ttu-id="fd18f-132">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fd18f-132">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="fd18f-133">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="fd18f-133">privacyProfile</span></span>|[<span data-ttu-id="fd18f-134">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="fd18f-134">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="fd18f-135">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="fd18f-135">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="fd18f-136">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="fd18f-136">securityComplianceNotificationMails</span></span>|<span data-ttu-id="fd18f-137">String collection</span><span class="sxs-lookup"><span data-stu-id="fd18f-137">String collection</span></span>||
|<span data-ttu-id="fd18f-138">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="fd18f-138">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="fd18f-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="fd18f-139">String collection</span></span>||
|<span data-ttu-id="fd18f-140">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="fd18f-140">technicalNotificationMails</span></span>|<span data-ttu-id="fd18f-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="fd18f-141">String collection</span></span>|                                        <span data-ttu-id="fd18f-142">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fd18f-142">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="fd18f-143">响应</span><span class="sxs-lookup"><span data-stu-id="fd18f-143">Response</span></span>

<span data-ttu-id="fd18f-144">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fd18f-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fd18f-145">示例</span><span class="sxs-lookup"><span data-stu-id="fd18f-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd18f-146">请求</span><span class="sxs-lookup"><span data-stu-id="fd18f-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="fd18f-147">响应</span><span class="sxs-lookup"><span data-stu-id="fd18f-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
