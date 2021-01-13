---
title: 提及资源类型
description: 表示根据用户的电子邮件地址向用户发送的通知。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 23d4ac1d98a65e206a476768569cca89fb295a61
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844856"
---
# <a name="mention-resource-type"></a><span data-ttu-id="9a0f7-103">提及资源类型</span><span class="sxs-lookup"><span data-stu-id="9a0f7-103">mention resource type</span></span>

<span data-ttu-id="9a0f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a0f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a0f7-105">表示根据用户的电子邮件地址向用户发送的通知。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-105">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="9a0f7-106">此类型的通知也称为 @-mentions。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-106">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="9a0f7-107">邮件 [资源](../resources/message.md) 支持 **提及**。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-107">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="9a0f7-108">它包括 **一个 mentionsPreview** 属性，该属性指示是否已在邮件实例中提及登录用户。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-108">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="9a0f7-109">它还包括 **提及** 导航属性，该属性支持获取提及的详细信息，或删除该实例中的提及。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-109">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="9a0f7-110">创建邮件时，应用可以通过将提及包括在提及属性中，在同一请求中 `POST` 创建 **提及** 。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-110">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="9a0f7-111">通过使用查询参数的请求，应用可以返回已登录用户邮箱中提及该用户 `GET` `$filter` 的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-111">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="9a0f7-112">通过 `GET` 查询参数 `$expand` 的请求，应用可以展开特定邮件中提及的所有内容。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-112">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="9a0f7-113">这种允许应用在邮件中设置和提及的机制可启用轻型通知，其中进行提及的用户可以保留在现有上下文中 (例如，在应用设置基础提及属性时) 撰写邮件正文。 </span><span class="sxs-lookup"><span data-stu-id="9a0f7-113">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="9a0f7-114">被提及人员可以轻松找出是否通过请求或查询参数提及 `GET` `$filter` 他们以及在何处 `$expand` 提及他们。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-114">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="9a0f7-115">例如，在 Outlook 邮件客户端中，当用户在编写邮件时进行输入时，Outlook 允许用户选择或输入名称以 `@` 完成 @-mention。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-115">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="9a0f7-116">Outlook 在 **创建和** 发送邮件或事件之前设置 mentions 属性。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-116">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="9a0f7-117">Outlook 还使用与登录用户一起的操作，并允许登录用户查找提及用户的邮件，以提醒用户操作项目或讨论，从而加快 `GET` `$filter` `$expand` 响应速度。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-117">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9a0f7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a0f7-118">JSON representation</span></span>

<span data-ttu-id="9a0f7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-119">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9a0f7-120">属性</span><span class="sxs-lookup"><span data-stu-id="9a0f7-120">Properties</span></span>
| <span data-ttu-id="9a0f7-121">属性</span><span class="sxs-lookup"><span data-stu-id="9a0f7-121">Property</span></span>     | <span data-ttu-id="9a0f7-122">类型</span><span class="sxs-lookup"><span data-stu-id="9a0f7-122">Type</span></span>   |<span data-ttu-id="9a0f7-123">说明</span><span class="sxs-lookup"><span data-stu-id="9a0f7-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a0f7-124">application</span><span class="sxs-lookup"><span data-stu-id="9a0f7-124">application</span></span> | <span data-ttu-id="9a0f7-125">String</span><span class="sxs-lookup"><span data-stu-id="9a0f7-125">String</span></span> | <span data-ttu-id="9a0f7-126">创建提及项的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-126">The name of the application where the mention is created.</span></span> <span data-ttu-id="9a0f7-127">可选。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-127">Optional.</span></span> <span data-ttu-id="9a0f7-128">不用于邮件，并且默认为 **null。**</span><span class="sxs-lookup"><span data-stu-id="9a0f7-128">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="9a0f7-129">clientReference</span><span class="sxs-lookup"><span data-stu-id="9a0f7-129">clientReference</span></span> | <span data-ttu-id="9a0f7-130">String</span><span class="sxs-lookup"><span data-stu-id="9a0f7-130">String</span></span> | <span data-ttu-id="9a0f7-131">表示资源实例的父级的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-131">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="9a0f7-132">可选。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-132">Optional.</span></span> <span data-ttu-id="9a0f7-133">不用于邮件，并且默认为 **null。**</span><span class="sxs-lookup"><span data-stu-id="9a0f7-133">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="9a0f7-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="9a0f7-134">createdBy</span></span>  | [<span data-ttu-id="9a0f7-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9a0f7-135">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="9a0f7-136">进行提及的用户的电子邮件信息。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-136">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="9a0f7-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a0f7-137">createdDateTime</span></span>  |<span data-ttu-id="9a0f7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a0f7-138">DateTimeOffset</span></span> |<span data-ttu-id="9a0f7-139">在客户端上创建提及的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-139">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="9a0f7-140">deepLink</span><span class="sxs-lookup"><span data-stu-id="9a0f7-140">deepLink</span></span> | <span data-ttu-id="9a0f7-141">String</span><span class="sxs-lookup"><span data-stu-id="9a0f7-141">String</span></span> | <span data-ttu-id="9a0f7-142">指向资源实例中提及内容上下文的深层 Web 链接。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-142">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="9a0f7-143">可选。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-143">Optional.</span></span> <span data-ttu-id="9a0f7-144">不用于邮件，并且默认为 **null。**</span><span class="sxs-lookup"><span data-stu-id="9a0f7-144">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="9a0f7-145">id</span><span class="sxs-lookup"><span data-stu-id="9a0f7-145">id</span></span> | <span data-ttu-id="9a0f7-146">String</span><span class="sxs-lookup"><span data-stu-id="9a0f7-146">String</span></span>| <span data-ttu-id="9a0f7-147">资源实例中提及的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-147">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="9a0f7-148">提及</span><span class="sxs-lookup"><span data-stu-id="9a0f7-148">mentioned</span></span> | [<span data-ttu-id="9a0f7-149">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9a0f7-149">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="9a0f7-150">被提及人员的电子邮件信息。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-150">The email information of the mentioned person.</span></span> <span data-ttu-id="9a0f7-151">必需。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-151">Required.</span></span> |
|<span data-ttu-id="9a0f7-152">mentionText</span><span class="sxs-lookup"><span data-stu-id="9a0f7-152">mentionText</span></span> | <span data-ttu-id="9a0f7-153">String</span><span class="sxs-lookup"><span data-stu-id="9a0f7-153">String</span></span> | <span data-ttu-id="9a0f7-154">可选。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-154">Optional.</span></span> <span data-ttu-id="9a0f7-155">不用于邮件，并且默认为 **null。**</span><span class="sxs-lookup"><span data-stu-id="9a0f7-155">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="9a0f7-156">若要获取邮件中的提及，请参阅邮件的 **bodyPreview** 属性。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-156">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="9a0f7-157">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a0f7-157">serverCreatedDateTime</span></span> | <span data-ttu-id="9a0f7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a0f7-158">DateTimeOffset</span></span> | <span data-ttu-id="9a0f7-159">在服务器上创建提及的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-159">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="9a0f7-160">可选。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-160">Optional.</span></span> <span data-ttu-id="9a0f7-161">不用于邮件，并且默认为 **null。**</span><span class="sxs-lookup"><span data-stu-id="9a0f7-161">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9a0f7-162">关系</span><span class="sxs-lookup"><span data-stu-id="9a0f7-162">Relationships</span></span>
<span data-ttu-id="9a0f7-163">无</span><span class="sxs-lookup"><span data-stu-id="9a0f7-163">None</span></span>


## <a name="methods"></a><span data-ttu-id="9a0f7-164">方法</span><span class="sxs-lookup"><span data-stu-id="9a0f7-164">Methods</span></span>

| <span data-ttu-id="9a0f7-165">方法</span><span class="sxs-lookup"><span data-stu-id="9a0f7-165">Method</span></span>           | <span data-ttu-id="9a0f7-166">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a0f7-166">Return Type</span></span>    |<span data-ttu-id="9a0f7-167">说明</span><span class="sxs-lookup"><span data-stu-id="9a0f7-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a0f7-168">[发布](../api/user-sendmail.md#request-2) 和发送</span><span class="sxs-lookup"><span data-stu-id="9a0f7-168">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="9a0f7-169">无</span><span class="sxs-lookup"><span data-stu-id="9a0f7-169">None</span></span> | <span data-ttu-id="9a0f7-170">创建新邮件的一部分并发送提及。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-170">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="9a0f7-171">[张贴](../api/user-post-messages.md#request-2) 到新草稿</span><span class="sxs-lookup"><span data-stu-id="9a0f7-171">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="9a0f7-172">[包含](../resources/message.md) 一个或多个 **提及对象** 的邮件。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-172">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="9a0f7-173">创建新邮件的草稿，并包括一个或多个 **提及** 对象。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-173">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="9a0f7-174">[获取](../api/user-list-messages.md#request-2) 提及我的消息</span><span class="sxs-lookup"><span data-stu-id="9a0f7-174">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="9a0f7-175">[message](../resources/message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a0f7-175">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="9a0f7-176">获取已登录用户的邮箱中包含此用户提及的所有邮件。 </span><span class="sxs-lookup"><span data-stu-id="9a0f7-176">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="9a0f7-177">[获取](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) 邮件及其提及内容</span><span class="sxs-lookup"><span data-stu-id="9a0f7-177">[Get](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) a message and its mentions</span></span> | <span data-ttu-id="9a0f7-178">[message](../resources/message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a0f7-178">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="9a0f7-179">获取邮件并展开邮件中每个 **提及** 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-179">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="9a0f7-180">[删除](../api/message-delete.md#request-2) 提及</span><span class="sxs-lookup"><span data-stu-id="9a0f7-180">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="9a0f7-181">无</span><span class="sxs-lookup"><span data-stu-id="9a0f7-181">None</span></span> |<span data-ttu-id="9a0f7-182">删除登录用户邮箱中指定邮件中指定的提及内容。</span><span class="sxs-lookup"><span data-stu-id="9a0f7-182">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


