---
title: 从其他用户身份发送 Outlook 邮件
description: 使用“代理发送”和“代表发送”权限，从 Microsoft Graph 中的其他用户身份或共享邮箱发送 Outlook 邮件。
author: jasonjoh
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d384e060060804ddbafb03ea054b7609bbccd71b
ms.sourcegitcommit: d9d8b908061b3680e8a52790a6c9aaf8e51ceea0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2019
ms.locfileid: "28685675"
---
# <a name="send-outlook-messages-from-another-user"></a><span data-ttu-id="78597-103">从其他用户身份发送 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="78597-103">Send Outlook messages from another user</span></span>

<span data-ttu-id="78597-104">Exchange Online 提供的[邮箱权限](/Exchange/recipients/mailbox-permissions)允许用户从其他用户身份、通讯组列表、组、资源或共享邮箱发送邮件。</span><span class="sxs-lookup"><span data-stu-id="78597-104">Exchange Online provides [mailbox permissions](/Exchange/recipients/mailbox-permissions) that allow a user to send mail that appears to be sent from another user, distribution list, group, resource, or shared mailbox.</span></span> <span data-ttu-id="78597-105">Microsoft Graph 也支持此功能，但是最终结果各不相同，具体取决于在 Exchange Online 中授予的准确权限以及用于发送邮件的 API。</span><span class="sxs-lookup"><span data-stu-id="78597-105">Microsoft Graph supports this feature as well, but the end result varies depending on the exact permissions granted in Exchange Online and which API you use to send the mail.</span></span>

## <a name="permissions"></a><span data-ttu-id="78597-106">权限</span><span class="sxs-lookup"><span data-stu-id="78597-106">Permissions</span></span>

<span data-ttu-id="78597-107">两类权限适用于从其他用户身份发送邮件：[Microsoft Graph 权限](permissions-reference.md)和邮箱权限。</span><span class="sxs-lookup"><span data-stu-id="78597-107">Two types of permissions apply to sending messages from another user: [Microsoft Graph permissions](permissions-reference.md), and mailbox permissions.</span></span>

### <a name="microsoft-graph-permissions"></a><span data-ttu-id="78597-108">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="78597-108">Microsoft Graph permissions</span></span>

<span data-ttu-id="78597-109">若要从其他用户身份发送邮件，使用用户令牌的应用程序需使用 the **Mail.Send.Shared** 权限。</span><span class="sxs-lookup"><span data-stu-id="78597-109">In order to send messages from another user, applications that use user tokens use the **Mail.Send.Shared** permission.</span></span>

> [!NOTE]
> <span data-ttu-id="78597-110">使用应用程序令牌而不是用户令牌且已拥有管理员授予的 **Mail.Send** 权限的应用程序可以组织中的任何用户身份发送邮件，只需通过用户的邮箱正常发送邮件即可。</span><span class="sxs-lookup"><span data-stu-id="78597-110">Applications that use application tokens instead of user tokens and have the **Mail.Send** permission consented by an administrator can send mail as any user in the organization by sending the mail normally through the user's mailbox.</span></span>

### <a name="mailbox-permissions"></a><span data-ttu-id="78597-111">邮箱权限</span><span class="sxs-lookup"><span data-stu-id="78597-111">Mailbox permissions</span></span>

<span data-ttu-id="78597-112">以下两种权限会影响从其他用户身份发送邮件的最终结果：**代表发送**和**代理发送**。</span><span class="sxs-lookup"><span data-stu-id="78597-112">Two permissions affect the end result of sending a message from another user: **Send on Behalf** and **Send As**.</span></span> <span data-ttu-id="78597-113">使用 **Mail.Send.Shared** 权限登录应用程序的用户必须至少拥有这两种权限之一，这些权限已授予从其中发送邮件的邮箱、组或通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="78597-113">The user that is signed in to your application with the **Mail.Send.Shared** permission MUST have at least one of these permissions granted to the mailbox, group, or distribution list that the mail is from.</span></span>

#### <a name="send-on-behalf"></a><span data-ttu-id="78597-114">代表发送</span><span class="sxs-lookup"><span data-stu-id="78597-114">Send on Behalf</span></span>

<span data-ttu-id="78597-115">使用此权限时，电子邮件的收件人将在其电子邮件客户端收到此邮件是使用你的应用程序代表其他用户发送的指示。</span><span class="sxs-lookup"><span data-stu-id="78597-115">With this permission, the recipient of the email has an indication in their email client that the message was sent by the user of your application on behalf of another user.</span></span>

![指示邮件是由一个用户代表另一个用户发送的 Outlook 网页版屏幕截图](images/outlook-sent-on-behalf.png)

<span data-ttu-id="78597-117">它在 Microsoft Graph 显示为 `sender`（实际发送邮件的用户）和 `from`（代表发送邮件的用户/组/等）属性。</span><span class="sxs-lookup"><span data-stu-id="78597-117">This is exposed in Microsoft Graph as the `sender` (user that actually sent the message) and `from` (user/group/etc. that the message appears to be from) properties.</span></span>

```json
{
  "id": "AAMkAGE1...",
  "subject": "Send mail test",
  "sender": {
    "emailAddress": {
      "name": "Adele Vance",
      "address": "AdeleV@contoso.com"
    }
  },
  "from": {
    "emailAddress": {
      "name": "Pradeep Gupta",
      "address": "PradeepG@contoso.com"
    }
  }
}
```

<span data-ttu-id="78597-118">用户可以[使用 Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926) 将其自己邮箱的这种权限授予其他用户。</span><span class="sxs-lookup"><span data-stu-id="78597-118">A user can grant this permission for their own mailbox to another user by [using Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926).</span></span> <span data-ttu-id="78597-119">管理员可以在 [Office 365 管理中心](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide)为任何邮箱、组或通讯组列表授予此权限。</span><span class="sxs-lookup"><span data-stu-id="78597-119">Administrators can grant this permission for any mailbox, group, or distribution list in the [Office 365 admin center](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide).</span></span>

#### <a name="send-as"></a><span data-ttu-id="78597-120">代理发送</span><span class="sxs-lookup"><span data-stu-id="78597-120">Send As</span></span>

<span data-ttu-id="78597-121">使用此权限时，不会显示邮件是以其他用户身份发送的指示。</span><span class="sxs-lookup"><span data-stu-id="78597-121">With this permission, there is no indication that the message was sent as a different user.</span></span> <span data-ttu-id="78597-122">`sender` 和 `from` 属性具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="78597-122">The `sender` and `from` properties have the same value.</span></span>

<span data-ttu-id="78597-123">用户无法为其邮箱授予此权限。</span><span class="sxs-lookup"><span data-stu-id="78597-123">Users cannot grant this permission to their mailboxes.</span></span> <span data-ttu-id="78597-124">管理员可以在 Office 365 管理中心授予此权限。</span><span class="sxs-lookup"><span data-stu-id="78597-124">Admins can grant this permission in the Office 365 admin center.</span></span>

## <a name="sending-with-microsoft-graph"></a><span data-ttu-id="78597-125">通过 Microsoft Graph 发送</span><span class="sxs-lookup"><span data-stu-id="78597-125">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="78597-126">可以通过[直接发送](/graph/api/user-sendmail?view=graph-rest-1.0)或[创建草稿](/graph/api/user-post-messages?view=graph-rest-1.0)然后再[发送](/graph/api/message-send?view=graph-rest-1.0)这两种方式，从其他用户身份发送邮件。</span><span class="sxs-lookup"><span data-stu-id="78597-126">You can send messages from another user by either [sending directly](/graph/api/user-sendmail?view=graph-rest-1.0) or by [creating a draft](/graph/api/user-post-messages?view=graph-rest-1.0) and then [sending it](/graph/api/message-send?view=graph-rest-1.0).</span></span>

<span data-ttu-id="78597-127">如要从其他用户身份发送，请设置要从其中向用户电子邮件地址发送的[邮件](/graph/api/resources/message?view=graph-rest-1.0)上的 `from` 属性。</span><span class="sxs-lookup"><span data-stu-id="78597-127">In order to send from another user, set the `from` property on the [message](/graph/api/resources/message?view=graph-rest-1.0) sent to the email address of the user to send from.</span></span> <span data-ttu-id="78597-128">无需设置 `sender` 属性 - Microsoft Graph 将会根据授予已登录用户的邮箱权限进行相应的设置。</span><span class="sxs-lookup"><span data-stu-id="78597-128">You don't need to set the `sender` property - Microsoft Graph will set it appropriately, based on the mailbox permissions granted to the user who has signed in.</span></span>

<span data-ttu-id="78597-129">例如，若要从 `sales@contoso.com` 组发送邮件，请按如下所示配置邮件。</span><span class="sxs-lookup"><span data-stu-id="78597-129">For example, to send mail from the `sales@contoso.com` group, configure the message as follows.</span></span>

```json
{
  "subject": "January sales report",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "MeganB@contoso.com"
      }
    }
  ],
  "from": [
    {
      "emailAddress": {
        "address": "sales@contoso.com"
      }
    }
  ]
}
```

## <a name="sent-items-behavior"></a><span data-ttu-id="78597-130">已发送邮件行为</span><span class="sxs-lookup"><span data-stu-id="78597-130">Sent Items behavior</span></span>

<span data-ttu-id="78597-131">邮件发送完毕后，可将其保存至发送用户的“已发送邮件”文件夹、发件人用户的“已发送邮件”文件夹或两者。</span><span class="sxs-lookup"><span data-stu-id="78597-131">After the message is sent, it can be saved to the sending user's Sent Items folder, the from user's Sent Items folder, or both.</span></span> <span data-ttu-id="78597-132">也可以完全不保存。</span><span class="sxs-lookup"><span data-stu-id="78597-132">It can also not be saved at all.</span></span>

> [!NOTE]
> <span data-ttu-id="78597-133">如果邮件是从没有邮箱的地址（例如通讯组列表）发送，则发件人用户没有“已发送邮件”。</span><span class="sxs-lookup"><span data-stu-id="78597-133">If the message is sent from an address that does not have a mailbox (a distribution list, for example), there is no Sent Items for the from user.</span></span>

- <span data-ttu-id="78597-134">如果应用程序通过使用 `/me` 终结点（或 `/users/{user-id}`，其中 `user-id` 对应于已登录的用户）发送，邮件则会默认保存至发送用户的“已发送邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="78597-134">If your application sends by using the `/me` endpoint (or `/users/{user-id}` where the `user-id` corresponds to the signed in user), by default, the message will be saved in the sending user's Sent Items folder.</span></span>
- <span data-ttu-id="78597-135">如果应用程序通过使用 `/users/{user-id}`（其中 `user-id` 对应于已登录的用户）发送，邮件则会默认保存至发件人用户的“已发送邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="78597-135">If your application sends by using the `/users/{user-id}` where the `user-id` corresponds to the from user, by default, the message will be saved in the from user's Sent Items folder.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="78597-136">若要以此方式发送，除了**代表发送**或**代理发送**权限之外，发送用户还必须具有**完全访问**邮箱权限。</span><span class="sxs-lookup"><span data-stu-id="78597-136">In order to send this way, the sending user must have the **Full Access** mailbox permission in addition to either the **Send on Behalf** or **Send As** permission.</span></span>

<span data-ttu-id="78597-137">以下其他外部因素可能会改变默认行为：</span><span class="sxs-lookup"><span data-stu-id="78597-137">The default behavior can be changed by other outside factors:</span></span>

- <span data-ttu-id="78597-138">管理员将发件人用户的邮箱更新为[始终将从代理发送的邮件副本保存](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox)至其“已发送邮件”。</span><span class="sxs-lookup"><span data-stu-id="78597-138">Administrators can update the from user's mailbox to [always save a copy of messages sent from a delegate](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox) to their Sent Items.</span></span>
- <span data-ttu-id="78597-139">通过在 [send mail](/graph/api/user-sendmail?view=graph-rest-1.0) 请求中将 `saveToSentItems` 属性设为 `true`，可以防止邮件被保存至“已发送邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="78597-139">By setting the `saveToSentItems` property to `true` in a [send mail](/graph/api/user-sendmail?view=graph-rest-1.0) request, you can prevent the item from being saved to the Sent Items folder.</span></span> <span data-ttu-id="78597-140">但是，如果管理员已配置“始终保存副本”设置，则邮件将被保存至发件人用户的“已发送邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="78597-140">However, if an administrator has configured the "always save a copy" setting, the message will still be saved to the from user's Sent Items.</span></span>

## <a name="examples"></a><span data-ttu-id="78597-141">示例</span><span class="sxs-lookup"><span data-stu-id="78597-141">Examples</span></span>

### <a name="example-1-successful-send-through-me-endpoint"></a><span data-ttu-id="78597-142">示例 1：通过 /me 终结点成功发送</span><span class="sxs-lookup"><span data-stu-id="78597-142">Example 1: Successful send through /me endpoint</span></span>

<span data-ttu-id="78597-143">在此示例中，Adele Vance 已为 Allan Deyoung 的邮箱授予**代表发送**权限。</span><span class="sxs-lookup"><span data-stu-id="78597-143">In this example, Adele Vance has been granted **Send on Behalf** permission to Allan Deyoung's mailbox.</span></span>

#### <a name="request"></a><span data-ttu-id="78597-144">请求</span><span class="sxs-lookup"><span data-stu-id="78597-144">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Expense reports",
    "body": {
      "contentType": "text",
      "content": "Have you submitted your expense reports yet?"
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": [
      {
        "emailAddress": {
          "address": "AllanD@contoso.com"
        }
      }
    ]
  }
}
```

#### <a name="response"></a><span data-ttu-id="78597-145">响应</span><span class="sxs-lookup"><span data-stu-id="78597-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-unsuccessful-attempt-to-send-without-permissions"></a><span data-ttu-id="78597-146">示例 2：在无权限的情况下，尝试发送失败</span><span class="sxs-lookup"><span data-stu-id="78597-146">Example 2: Unsuccessful attempt to send without permissions</span></span>

<span data-ttu-id="78597-147">在此示例中，Adele Vance 尝试从 Patti Fernandez 身份发送电子邮件，但他并没有被授予**代表发送**或**代理发送**权限。</span><span class="sxs-lookup"><span data-stu-id="78597-147">In this example, Adele Vance attempts to send an email from Patti Fernandez, but has not been granted either the **Send on Behalf** or **Send As** permission.</span></span> <span data-ttu-id="78597-148">响应中包含 `ErrorSendAsDenied` 错误。</span><span class="sxs-lookup"><span data-stu-id="78597-148">The response contains a `ErrorSendAsDenied`.</span></span>

<!-- markdownlint-disable MD024 -->

#### <a name="request"></a><span data-ttu-id="78597-149">请求</span><span class="sxs-lookup"><span data-stu-id="78597-149">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Support ticket",
    "body": {
      "contentType": "text",
      "content": "I noticed you opened a support ticket yesterday..."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": [
      {
        "emailAddress": {
          "address": "PattiF@contoso.com"
        }
      }
    ]
  }
}
```

#### <a name="response"></a><span data-ttu-id="78597-150">响应</span><span class="sxs-lookup"><span data-stu-id="78597-150">Response</span></span>

```http
HTTP/1.1 403 Forbidden
Content-Type: application/json

{
  "error": {
    "code": "ErrorSendAsDenied",
    "message": "The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account., Cannot submit message.",
    "innerError": {
      "request-id": "24e7991e-01ae-4cc2-8e06-532a96fd8948",
      "date": "2019-01-16T18:53:25"
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="78597-151">后续步骤</span><span class="sxs-lookup"><span data-stu-id="78597-151">Next steps</span></span>

<span data-ttu-id="78597-152">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="78597-152">Find out more about:</span></span>

- [<span data-ttu-id="78597-153">为什么与 Outlook 邮件集成</span><span class="sxs-lookup"><span data-stu-id="78597-153">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="78597-154">Microsoft Graph v1.0 中的[使用邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) 和邮件 API [用例](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="78597-154">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-send-mail-from-other-user.md:
      Exception processing links.
    System.ArgumentException: Link Definition was null. Link text: !NOTE
      at ApiDoctor.Validation.DocFile.get_LinkDestinations()
      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
