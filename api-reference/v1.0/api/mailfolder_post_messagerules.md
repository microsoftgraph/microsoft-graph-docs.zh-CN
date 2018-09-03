# <a name="create-rule"></a><span data-ttu-id="56f0c-101">创建规则</span><span class="sxs-lookup"><span data-stu-id="56f0c-101">Create rule</span></span>


<span data-ttu-id="56f0c-102">通过指定一组条件和操作来创建 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56f0c-102">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="56f0c-103">如果用户收件箱中的传入邮件符合指定条件，Outlook 就会执行这些操作。</span><span class="sxs-lookup"><span data-stu-id="56f0c-103">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="56f0c-104">权限</span><span class="sxs-lookup"><span data-stu-id="56f0c-104">Permissions</span></span>
<span data-ttu-id="56f0c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="56f0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56f0c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="56f0c-107">Permission type</span></span>      | <span data-ttu-id="56f0c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56f0c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56f0c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56f0c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="56f0c-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56f0c-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="56f0c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56f0c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56f0c-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56f0c-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="56f0c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="56f0c-113">Application</span></span> | <span data-ttu-id="56f0c-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56f0c-114">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="56f0c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56f0c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="56f0c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="56f0c-116">Request headers</span></span>
| <span data-ttu-id="56f0c-117">名称</span><span class="sxs-lookup"><span data-stu-id="56f0c-117">Name</span></span>       | <span data-ttu-id="56f0c-118">说明</span><span class="sxs-lookup"><span data-stu-id="56f0c-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56f0c-119">授权</span><span class="sxs-lookup"><span data-stu-id="56f0c-119">Authorization</span></span>  | <span data-ttu-id="56f0c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56f0c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="56f0c-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="56f0c-122">Request body</span></span>
<span data-ttu-id="56f0c-123">在请求正文中，提供适用于规则的参数。</span><span class="sxs-lookup"><span data-stu-id="56f0c-123">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="56f0c-124">以下是在创建规则时通常使用的正文参数。</span><span class="sxs-lookup"><span data-stu-id="56f0c-124">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="56f0c-125">可以根据情况在请求正文中指定任何其他可写的 **messageRule** 属性。</span><span class="sxs-lookup"><span data-stu-id="56f0c-125">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="56f0c-126">名称</span><span class="sxs-lookup"><span data-stu-id="56f0c-126">Name</span></span>       | <span data-ttu-id="56f0c-127">类型</span><span class="sxs-lookup"><span data-stu-id="56f0c-127">Type</span></span>|<span data-ttu-id="56f0c-128">说明</span><span class="sxs-lookup"><span data-stu-id="56f0c-128">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="56f0c-129">actions</span><span class="sxs-lookup"><span data-stu-id="56f0c-129">actions</span></span>|[<span data-ttu-id="56f0c-130">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="56f0c-130">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="56f0c-131">满足相应条件（如果有的话）时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="56f0c-131">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="56f0c-132">必需。</span><span class="sxs-lookup"><span data-stu-id="56f0c-132">Required.</span></span>|
|<span data-ttu-id="56f0c-133">conditions</span><span class="sxs-lookup"><span data-stu-id="56f0c-133">conditions</span></span>|[<span data-ttu-id="56f0c-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="56f0c-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="56f0c-135">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="56f0c-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="56f0c-136">可选。</span><span class="sxs-lookup"><span data-stu-id="56f0c-136">Optional.</span></span>|
|<span data-ttu-id="56f0c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="56f0c-137">displayName</span></span>| <span data-ttu-id="56f0c-138">字符串</span><span class="sxs-lookup"><span data-stu-id="56f0c-138">String</span></span>  | <span data-ttu-id="56f0c-139">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="56f0c-139">The display name of the rule.</span></span> <span data-ttu-id="56f0c-140">必需。</span><span class="sxs-lookup"><span data-stu-id="56f0c-140">Required.</span></span>|
|<span data-ttu-id="56f0c-141">exceptions</span><span class="sxs-lookup"><span data-stu-id="56f0c-141">exceptions</span></span>| [<span data-ttu-id="56f0c-142">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="56f0c-142">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="56f0c-143">表示规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="56f0c-143">Represents exception conditions for the rule.</span></span> <span data-ttu-id="56f0c-144">可选。</span><span class="sxs-lookup"><span data-stu-id="56f0c-144">Optional.</span></span> |
|<span data-ttu-id="56f0c-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="56f0c-145">isEnabled</span></span> | <span data-ttu-id="56f0c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f0c-146">Boolean</span></span> | <span data-ttu-id="56f0c-147">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="56f0c-147">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="56f0c-148">可选。</span><span class="sxs-lookup"><span data-stu-id="56f0c-148">Optional.</span></span> |
|<span data-ttu-id="56f0c-149">Sequence</span><span class="sxs-lookup"><span data-stu-id="56f0c-149">sequence</span></span>| <span data-ttu-id="56f0c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="56f0c-150">Int32</span></span> | <span data-ttu-id="56f0c-151">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="56f0c-151">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="56f0c-152">必需。</span><span class="sxs-lookup"><span data-stu-id="56f0c-152">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="56f0c-153">响应</span><span class="sxs-lookup"><span data-stu-id="56f0c-153">Response</span></span>
<span data-ttu-id="56f0c-154">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="56f0c-154">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56f0c-155">示例</span><span class="sxs-lookup"><span data-stu-id="56f0c-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56f0c-156">请求</span><span class="sxs-lookup"><span data-stu-id="56f0c-156">Request</span></span>
<span data-ttu-id="56f0c-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56f0c-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
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
##### <a name="response"></a><span data-ttu-id="56f0c-158">响应</span><span class="sxs-lookup"><span data-stu-id="56f0c-158">Response</span></span>
<span data-ttu-id="56f0c-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56f0c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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