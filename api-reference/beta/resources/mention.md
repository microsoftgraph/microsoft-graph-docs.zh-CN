---
title: 有提及资源类型
description: '代表到个人基于此人的电子邮件地址的通知。 也称为是通知的这种类型 '
ms.openlocfilehash: 7e70c6a84665b474ea4d8421f60e78687ebb49b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042221"
---
# <a name="mention-resource-type"></a><span data-ttu-id="3c79b-104">有提及资源类型</span><span class="sxs-lookup"><span data-stu-id="3c79b-104">mention resource type</span></span>

> <span data-ttu-id="3c79b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c79b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c79b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c79b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c79b-107">代表到个人基于此人的电子邮件地址的通知。</span><span class="sxs-lookup"><span data-stu-id="3c79b-107">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="3c79b-108">此类通知也称为是 @ 提及。</span><span class="sxs-lookup"><span data-stu-id="3c79b-108">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="3c79b-109">[消息](../resources/message.md)资源支持**提及**。</span><span class="sxs-lookup"><span data-stu-id="3c79b-109">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="3c79b-110">它包括**mentionsPreview**属性指示是否已登录的用户提及该消息实例中。</span><span class="sxs-lookup"><span data-stu-id="3c79b-110">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="3c79b-111">它还包括支持的某个提及，或删除某个提及该实例中的获取详细信息的**提到**导航属性。</span><span class="sxs-lookup"><span data-stu-id="3c79b-111">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="3c79b-112">应用程序时创建一条消息，可以在同一个创建某个提及`POST`通过包括提及的**提到**属性中的请求。</span><span class="sxs-lookup"><span data-stu-id="3c79b-112">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="3c79b-113">使用`GET`请求`$filter`查询参数，应用程序可返回所有邮件提及用户的登录用户邮箱中。</span><span class="sxs-lookup"><span data-stu-id="3c79b-113">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="3c79b-114">A`GET`请求`$expand`参数允许展开特定的邮件中的所有提及的应用程序的查询。</span><span class="sxs-lookup"><span data-stu-id="3c79b-114">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="3c79b-115">此机制的应用程序时让应用程序设置和获取提及在消息中的允许轻型通知，其中进行提及的用户，可以保持 （如撰写邮件正文） 的现有上下文中设置基础**提及**属性.</span><span class="sxs-lookup"><span data-stu-id="3c79b-115">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="3c79b-116">提到人员可以轻松地找到如果和通过其中提到这些`GET`请求与`$filter`或`$expand`查询参数。</span><span class="sxs-lookup"><span data-stu-id="3c79b-116">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="3c79b-117">例如，在 Outlook 邮件客户端，当用户键入时`@`Outlook 时写入一条消息，允许用户选择或输入要完成 @ 提及的名称。</span><span class="sxs-lookup"><span data-stu-id="3c79b-117">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="3c79b-118">创建和发送的邮件或事件之前，outlook 将**提到**属性设置。</span><span class="sxs-lookup"><span data-stu-id="3c79b-118">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="3c79b-119">Outlook 还使用`GET`操作`$filter`和`$expand`，使已登录的用户可以查找提及用户的消息，警报用户对拟办事项或讨论，从而实现更快地响应。</span><span class="sxs-lookup"><span data-stu-id="3c79b-119">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3c79b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c79b-120">JSON representation</span></span>

<span data-ttu-id="3c79b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c79b-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a><span data-ttu-id="3c79b-122">属性</span><span class="sxs-lookup"><span data-stu-id="3c79b-122">Properties</span></span>
| <span data-ttu-id="3c79b-123">属性</span><span class="sxs-lookup"><span data-stu-id="3c79b-123">Property</span></span>     | <span data-ttu-id="3c79b-124">类型</span><span class="sxs-lookup"><span data-stu-id="3c79b-124">Type</span></span>   |<span data-ttu-id="3c79b-125">说明</span><span class="sxs-lookup"><span data-stu-id="3c79b-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c79b-126">application</span><span class="sxs-lookup"><span data-stu-id="3c79b-126">application</span></span> | <span data-ttu-id="3c79b-127">字符串</span><span class="sxs-lookup"><span data-stu-id="3c79b-127">String</span></span> | <span data-ttu-id="3c79b-128">在其中创建提及的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="3c79b-128">The name of the application where the mention is created.</span></span> <span data-ttu-id="3c79b-129">可选。</span><span class="sxs-lookup"><span data-stu-id="3c79b-129">Optional.</span></span> <span data-ttu-id="3c79b-130">不使用和默认设置为 null 的**消息**。</span><span class="sxs-lookup"><span data-stu-id="3c79b-130">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="3c79b-131">clientReference</span><span class="sxs-lookup"><span data-stu-id="3c79b-131">clientReference</span></span> | <span data-ttu-id="3c79b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="3c79b-132">String</span></span> | <span data-ttu-id="3c79b-133">表示父资源实例的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3c79b-133">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="3c79b-134">可选。</span><span class="sxs-lookup"><span data-stu-id="3c79b-134">Optional.</span></span> <span data-ttu-id="3c79b-135">不使用和默认设置为 null 的**消息**。</span><span class="sxs-lookup"><span data-stu-id="3c79b-135">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="3c79b-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="3c79b-136">createdBy</span></span>  | [<span data-ttu-id="3c79b-137">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3c79b-137">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="3c79b-138">进行提及的用户的电子邮件信息。</span><span class="sxs-lookup"><span data-stu-id="3c79b-138">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="3c79b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c79b-139">createdDateTime</span></span>  |<span data-ttu-id="3c79b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c79b-140">DateTimeOffset</span></span> |<span data-ttu-id="3c79b-141">日期和时间在客户端上创建提及的。</span><span class="sxs-lookup"><span data-stu-id="3c79b-141">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="3c79b-142">deepLink</span><span class="sxs-lookup"><span data-stu-id="3c79b-142">deepLink</span></span> | <span data-ttu-id="3c79b-143">字符串</span><span class="sxs-lookup"><span data-stu-id="3c79b-143">String</span></span> | <span data-ttu-id="3c79b-144">深入 web 链接到的资源实例中提及的上下文。</span><span class="sxs-lookup"><span data-stu-id="3c79b-144">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="3c79b-145">可选。</span><span class="sxs-lookup"><span data-stu-id="3c79b-145">Optional.</span></span> <span data-ttu-id="3c79b-146">不使用和默认设置为 null 的**消息**。</span><span class="sxs-lookup"><span data-stu-id="3c79b-146">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="3c79b-147">id</span><span class="sxs-lookup"><span data-stu-id="3c79b-147">id</span></span> | <span data-ttu-id="3c79b-148">字符串</span><span class="sxs-lookup"><span data-stu-id="3c79b-148">String</span></span>| <span data-ttu-id="3c79b-149">资源实例中提及的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3c79b-149">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="3c79b-150">提到</span><span class="sxs-lookup"><span data-stu-id="3c79b-150">mentioned</span></span> | [<span data-ttu-id="3c79b-151">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3c79b-151">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="3c79b-152">被提及人员的电子邮件的信息。</span><span class="sxs-lookup"><span data-stu-id="3c79b-152">The email information of the mentioned person.</span></span> <span data-ttu-id="3c79b-153">必需。</span><span class="sxs-lookup"><span data-stu-id="3c79b-153">Required.</span></span> |
|<span data-ttu-id="3c79b-154">mentionText</span><span class="sxs-lookup"><span data-stu-id="3c79b-154">mentionText</span></span> | <span data-ttu-id="3c79b-155">字符串</span><span class="sxs-lookup"><span data-stu-id="3c79b-155">String</span></span> | <span data-ttu-id="3c79b-156">可选。</span><span class="sxs-lookup"><span data-stu-id="3c79b-156">Optional.</span></span> <span data-ttu-id="3c79b-157">不使用和默认设置为 null 的**消息**。</span><span class="sxs-lookup"><span data-stu-id="3c79b-157">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="3c79b-158">获取提及中一条消息，请参阅改为邮件的**bodyPreview**属性。</span><span class="sxs-lookup"><span data-stu-id="3c79b-158">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="3c79b-159">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c79b-159">serverCreatedDateTime</span></span> | <span data-ttu-id="3c79b-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c79b-160">DateTimeOffset</span></span> | <span data-ttu-id="3c79b-161">日期和时间是在服务器上创建提及的。</span><span class="sxs-lookup"><span data-stu-id="3c79b-161">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="3c79b-162">可选。</span><span class="sxs-lookup"><span data-stu-id="3c79b-162">Optional.</span></span> <span data-ttu-id="3c79b-163">不使用和默认设置为 null 的**消息**。</span><span class="sxs-lookup"><span data-stu-id="3c79b-163">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3c79b-164">Relationships</span><span class="sxs-lookup"><span data-stu-id="3c79b-164">Relationships</span></span>
<span data-ttu-id="3c79b-165">无</span><span class="sxs-lookup"><span data-stu-id="3c79b-165">None</span></span>


## <a name="methods"></a><span data-ttu-id="3c79b-166">方法</span><span class="sxs-lookup"><span data-stu-id="3c79b-166">Methods</span></span>

| <span data-ttu-id="3c79b-167">方法</span><span class="sxs-lookup"><span data-stu-id="3c79b-167">Method</span></span>           | <span data-ttu-id="3c79b-168">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c79b-168">Return Type</span></span>    |<span data-ttu-id="3c79b-169">说明</span><span class="sxs-lookup"><span data-stu-id="3c79b-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c79b-170">[Post](../api/user-sendmail.md#request-2)和发送</span><span class="sxs-lookup"><span data-stu-id="3c79b-170">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="3c79b-171">无</span><span class="sxs-lookup"><span data-stu-id="3c79b-171">None</span></span> | <span data-ttu-id="3c79b-172">创建和发送提及作为新邮件的一部分。</span><span class="sxs-lookup"><span data-stu-id="3c79b-172">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="3c79b-173">以新草稿的[文章](../api/user-post-messages.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="3c79b-173">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="3c79b-174">包含一个或多个**提及**对象的[消息](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="3c79b-174">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="3c79b-175">创建一个新的邮件草稿并包括一个或多个**提及**的对象。</span><span class="sxs-lookup"><span data-stu-id="3c79b-175">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="3c79b-176">[获取](../api/user-list-messages.md#request-2)邮件提及我</span><span class="sxs-lookup"><span data-stu-id="3c79b-176">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="3c79b-177">[邮件](../resources/message.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c79b-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="3c79b-178">获取包含**提及**的此用户的登录用户邮箱中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="3c79b-178">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="3c79b-179">一条消息的[获取](../api/message-get.md#request-2)和其提及</span><span class="sxs-lookup"><span data-stu-id="3c79b-179">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="3c79b-180">[邮件](../resources/message.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c79b-180">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="3c79b-181">收到一条消息，并展开的每个**提及**消息中的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3c79b-181">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="3c79b-182">[删除](../api/message-delete.md#request-2)某个提及</span><span class="sxs-lookup"><span data-stu-id="3c79b-182">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="3c79b-183">无</span><span class="sxs-lookup"><span data-stu-id="3c79b-183">None</span></span> |<span data-ttu-id="3c79b-184">删除中指定的消息已登录的用户邮箱中提及的指定。</span><span class="sxs-lookup"><span data-stu-id="3c79b-184">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->