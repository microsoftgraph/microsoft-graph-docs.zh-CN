# <a name="create-rule"></a><span data-ttu-id="099ad-101">创建规则</span><span class="sxs-lookup"><span data-stu-id="099ad-101">Create rule</span></span>


<span data-ttu-id="099ad-102">通过指定一组条件和操作来创建 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="099ad-102">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="099ad-103">如果用户收件箱中的传入邮件符合指定条件，Outlook 就会执行这些操作。</span><span class="sxs-lookup"><span data-stu-id="099ad-103">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="099ad-104">权限</span><span class="sxs-lookup"><span data-stu-id="099ad-104">Permissions</span></span>
<span data-ttu-id="099ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="099ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="099ad-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="099ad-107">Permission type</span></span>      | <span data-ttu-id="099ad-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="099ad-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="099ad-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="099ad-109">Delegated (work or school account)</span></span> | <span data-ttu-id="099ad-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="099ad-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="099ad-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="099ad-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="099ad-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="099ad-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="099ad-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="099ad-113">Application</span></span> | <span data-ttu-id="099ad-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="099ad-114">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="099ad-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="099ad-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="099ad-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="099ad-116">Request headers</span></span>
| <span data-ttu-id="099ad-117">名称</span><span class="sxs-lookup"><span data-stu-id="099ad-117">Name</span></span>       | <span data-ttu-id="099ad-118">说明</span><span class="sxs-lookup"><span data-stu-id="099ad-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="099ad-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="099ad-119">Authorization</span></span>  | <span data-ttu-id="099ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="099ad-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="099ad-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="099ad-122">Request body</span></span>
<span data-ttu-id="099ad-123">在请求正文中，提供适用于规则的参数。</span><span class="sxs-lookup"><span data-stu-id="099ad-123">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="099ad-124">以下是在创建规则时通常使用的正文参数。</span><span class="sxs-lookup"><span data-stu-id="099ad-124">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="099ad-125">可以根据情况在请求正文中指定任何其他可写的 **messageRule** 属性。</span><span class="sxs-lookup"><span data-stu-id="099ad-125">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

### <a name="request-parameters"></a><span data-ttu-id="099ad-126">请求参数</span><span class="sxs-lookup"><span data-stu-id="099ad-126">Request parameters</span></span>
| <span data-ttu-id="099ad-127">名称</span><span class="sxs-lookup"><span data-stu-id="099ad-127">Name</span></span>       | <span data-ttu-id="099ad-128">类型</span><span class="sxs-lookup"><span data-stu-id="099ad-128">Type</span></span>|<span data-ttu-id="099ad-129">说明</span><span class="sxs-lookup"><span data-stu-id="099ad-129">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="099ad-130">actions</span><span class="sxs-lookup"><span data-stu-id="099ad-130">Actions</span></span>|[<span data-ttu-id="099ad-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="099ad-131">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="099ad-132">满足相应条件（如果有的话）时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="099ad-132">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="099ad-133">必需。</span><span class="sxs-lookup"><span data-stu-id="099ad-133">Required.</span></span>|
|<span data-ttu-id="099ad-134">conditions</span><span class="sxs-lookup"><span data-stu-id="099ad-134">Conditions</span></span>|[<span data-ttu-id="099ad-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="099ad-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="099ad-136">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="099ad-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="099ad-137">可选。</span><span class="sxs-lookup"><span data-stu-id="099ad-137">Optional.</span></span>|
|<span data-ttu-id="099ad-138">displayName</span><span class="sxs-lookup"><span data-stu-id="099ad-138">displayName</span></span>| <span data-ttu-id="099ad-139">String</span><span class="sxs-lookup"><span data-stu-id="099ad-139">String</span></span>  | <span data-ttu-id="099ad-140">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="099ad-140">The name of the new formatting rule.</span></span> <span data-ttu-id="099ad-141">必需。</span><span class="sxs-lookup"><span data-stu-id="099ad-141">Required.</span></span>|
|<span data-ttu-id="099ad-142">exceptions</span><span class="sxs-lookup"><span data-stu-id="099ad-142">exceptions</span></span>| [<span data-ttu-id="099ad-143">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="099ad-143">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="099ad-144">表示规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="099ad-144">Represents exception conditions for the rule.</span></span> <span data-ttu-id="099ad-145">可选。</span><span class="sxs-lookup"><span data-stu-id="099ad-145">Optional.</span></span> |
|<span data-ttu-id="099ad-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="099ad-146">isEnabled</span></span> | <span data-ttu-id="099ad-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="099ad-147">Boolean</span></span> | <span data-ttu-id="099ad-148">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="099ad-148">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="099ad-149">可选。</span><span class="sxs-lookup"><span data-stu-id="099ad-149">Optional.</span></span> |
|<span data-ttu-id="099ad-150">Sequence</span><span class="sxs-lookup"><span data-stu-id="099ad-150">Sequence</span></span>| <span data-ttu-id="099ad-151">Int32</span><span class="sxs-lookup"><span data-stu-id="099ad-151">Int32</span></span> | <span data-ttu-id="099ad-152">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="099ad-152">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="099ad-153">必需。</span><span class="sxs-lookup"><span data-stu-id="099ad-153">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="099ad-154">响应</span><span class="sxs-lookup"><span data-stu-id="099ad-154">Response</span></span>
<span data-ttu-id="099ad-155">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="099ad-155">If successful, this method returns a `201 Created` response code and a **settingStateDeviceSummary** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="099ad-156">示例</span><span class="sxs-lookup"><span data-stu-id="099ad-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="099ad-157">请求</span><span class="sxs-lookup"><span data-stu-id="099ad-157">Request</span></span>
<span data-ttu-id="099ad-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="099ad-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messagerules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
##### <a name="response"></a><span data-ttu-id="099ad-159">响应</span><span class="sxs-lookup"><span data-stu-id="099ad-159">Response</span></span>
<span data-ttu-id="099ad-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="099ad-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
      "stopProcessingRules":true,
      "forwardTo":[
        {
          "emailAddress":{
            "name":"Alex Wilbur",
            "address":"AlexW@contoso.onmicrosoft.com"
          }
        }
      ]
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->