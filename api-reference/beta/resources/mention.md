---
title: 提及资源类型
description: 表示基于人员的电子邮件地址的人员通知。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3780c4b01fc6dc81418034931f37e84d1e295b41
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522699"
---
# <a name="mention-resource-type"></a><span data-ttu-id="6a2ef-103">提及资源类型</span><span class="sxs-lookup"><span data-stu-id="6a2ef-103">mention resource type</span></span>

<span data-ttu-id="6a2ef-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6a2ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a2ef-105">表示基于人员的电子邮件地址的人员通知。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-105">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="6a2ef-106">这种类型的通知也称为 @ 提到。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-106">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="6a2ef-107">[邮件](../resources/message.md)资源支持**提到**。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-107">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="6a2ef-108">它包含一个**mentionsPreview**属性，该属性指示该邮件实例中是否提到已登录用户。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-108">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="6a2ef-109">它还包括**提及**导航属性，该属性支持获取提及的详细信息，或删除该实例中的提及。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-109">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="6a2ef-110">创建邮件时，应用程序可以通过在**提及**属性中添加提及`POST`的内容，在同一请求中创建记录。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-110">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="6a2ef-111">使用`$filter`查询`GET`参数的请求，应用程序可以返回登录用户的邮箱中提及用户的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-111">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="6a2ef-112">使用`GET` `$expand`查询参数的请求可让应用展开特定邮件中的所有提及。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-112">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="6a2ef-113">允许在邮件中使用应用程序集和获取提及的机制启用轻量通知，其中提出提及的用户可以保留在现有上下文中（例如，撰写邮件正文），而应用会设置基础**提及**属性。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-113">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="6a2ef-114">提到的`GET` `$filter`人员可以通过或`$expand`查询参数轻松了解是否以及在请求中提及的情况。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-114">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="6a2ef-115">例如，在 Outlook 邮件客户端中，当用户在撰写`@`邮件时键入时，Outlook 允许用户选择或输入名称来完成 @-提及。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-115">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="6a2ef-116">Outlook 在创建和发送邮件或事件之前设置**提及**属性。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-116">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="6a2ef-117">Outlook 还使用`GET`与`$filter`和`$expand`的操作，以让登录用户查找提及用户的邮件，提醒用户执行操作项目或讨论，这样可以更快地响应。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-117">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6a2ef-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a2ef-118">JSON representation</span></span>

<span data-ttu-id="6a2ef-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-119">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6a2ef-120">属性</span><span class="sxs-lookup"><span data-stu-id="6a2ef-120">Properties</span></span>
| <span data-ttu-id="6a2ef-121">属性</span><span class="sxs-lookup"><span data-stu-id="6a2ef-121">Property</span></span>     | <span data-ttu-id="6a2ef-122">类型</span><span class="sxs-lookup"><span data-stu-id="6a2ef-122">Type</span></span>   |<span data-ttu-id="6a2ef-123">说明</span><span class="sxs-lookup"><span data-stu-id="6a2ef-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a2ef-124">application</span><span class="sxs-lookup"><span data-stu-id="6a2ef-124">application</span></span> | <span data-ttu-id="6a2ef-125">String</span><span class="sxs-lookup"><span data-stu-id="6a2ef-125">String</span></span> | <span data-ttu-id="6a2ef-126">在其中创建提及的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-126">The name of the application where the mention is created.</span></span> <span data-ttu-id="6a2ef-127">可选。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-127">Optional.</span></span> <span data-ttu-id="6a2ef-128">不会对**邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-128">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="6a2ef-129">clientReference</span><span class="sxs-lookup"><span data-stu-id="6a2ef-129">clientReference</span></span> | <span data-ttu-id="6a2ef-130">String</span><span class="sxs-lookup"><span data-stu-id="6a2ef-130">String</span></span> | <span data-ttu-id="6a2ef-131">代表资源实例的父项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-131">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="6a2ef-132">可选。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-132">Optional.</span></span> <span data-ttu-id="6a2ef-133">不会对**邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-133">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="6a2ef-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="6a2ef-134">createdBy</span></span>  | [<span data-ttu-id="6a2ef-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6a2ef-135">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="6a2ef-136">提出提及的用户的电子邮件信息。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-136">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="6a2ef-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2ef-137">createdDateTime</span></span>  |<span data-ttu-id="6a2ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2ef-138">DateTimeOffset</span></span> |<span data-ttu-id="6a2ef-139">在客户端上创建提及的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-139">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="6a2ef-140">deepLink</span><span class="sxs-lookup"><span data-stu-id="6a2ef-140">deepLink</span></span> | <span data-ttu-id="6a2ef-141">String</span><span class="sxs-lookup"><span data-stu-id="6a2ef-141">String</span></span> | <span data-ttu-id="6a2ef-142">指向资源实例中提及的上下文的深层 web 链接。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-142">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="6a2ef-143">可选。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-143">Optional.</span></span> <span data-ttu-id="6a2ef-144">不会对**邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-144">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="6a2ef-145">id</span><span class="sxs-lookup"><span data-stu-id="6a2ef-145">id</span></span> | <span data-ttu-id="6a2ef-146">String</span><span class="sxs-lookup"><span data-stu-id="6a2ef-146">String</span></span>| <span data-ttu-id="6a2ef-147">资源实例中提及的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-147">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="6a2ef-148">所</span><span class="sxs-lookup"><span data-stu-id="6a2ef-148">mentioned</span></span> | [<span data-ttu-id="6a2ef-149">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6a2ef-149">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="6a2ef-150">提到的人员的电子邮件信息。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-150">The email information of the mentioned person.</span></span> <span data-ttu-id="6a2ef-151">必填。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-151">Required.</span></span> |
|<span data-ttu-id="6a2ef-152">mentionText</span><span class="sxs-lookup"><span data-stu-id="6a2ef-152">mentionText</span></span> | <span data-ttu-id="6a2ef-153">String</span><span class="sxs-lookup"><span data-stu-id="6a2ef-153">String</span></span> | <span data-ttu-id="6a2ef-154">可选。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-154">Optional.</span></span> <span data-ttu-id="6a2ef-155">不会对**邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-155">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="6a2ef-156">若要获取邮件中提及的内容，请改为查看邮件的**bodyPreview**属性。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-156">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="6a2ef-157">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2ef-157">serverCreatedDateTime</span></span> | <span data-ttu-id="6a2ef-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2ef-158">DateTimeOffset</span></span> | <span data-ttu-id="6a2ef-159">在服务器上创建提及的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-159">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="6a2ef-160">可选。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-160">Optional.</span></span> <span data-ttu-id="6a2ef-161">不会对**邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-161">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6a2ef-162">关系</span><span class="sxs-lookup"><span data-stu-id="6a2ef-162">Relationships</span></span>
<span data-ttu-id="6a2ef-163">无</span><span class="sxs-lookup"><span data-stu-id="6a2ef-163">None</span></span>


## <a name="methods"></a><span data-ttu-id="6a2ef-164">方法</span><span class="sxs-lookup"><span data-stu-id="6a2ef-164">Methods</span></span>

| <span data-ttu-id="6a2ef-165">方法</span><span class="sxs-lookup"><span data-stu-id="6a2ef-165">Method</span></span>           | <span data-ttu-id="6a2ef-166">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a2ef-166">Return Type</span></span>    |<span data-ttu-id="6a2ef-167">说明</span><span class="sxs-lookup"><span data-stu-id="6a2ef-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a2ef-168">[Post](../api/user-sendmail.md#request-2)和 send</span><span class="sxs-lookup"><span data-stu-id="6a2ef-168">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="6a2ef-169">无</span><span class="sxs-lookup"><span data-stu-id="6a2ef-169">None</span></span> | <span data-ttu-id="6a2ef-170">创建并将提及作为新邮件的一部分发送。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-170">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="6a2ef-171">[发布](../api/user-post-messages.md#request-2)到新草稿</span><span class="sxs-lookup"><span data-stu-id="6a2ef-171">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="6a2ef-172">包含一个或多个**提及**对象的[邮件](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-172">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="6a2ef-173">创建新邮件的草稿并包含一个或多个**提及**的对象。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-173">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="6a2ef-174">[获取](../api/user-list-messages.md#request-2)涉及我的邮件</span><span class="sxs-lookup"><span data-stu-id="6a2ef-174">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="6a2ef-175">[message](../resources/message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a2ef-175">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="6a2ef-176">获取已登录用户邮箱中的所有邮件，其中包含此用户的**提及**。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-176">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="6a2ef-177">[获取](../api/message-get.md#request-2)邮件及其提及内容</span><span class="sxs-lookup"><span data-stu-id="6a2ef-177">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="6a2ef-178">[message](../resources/message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a2ef-178">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="6a2ef-179">获取邮件并展开邮件中每个**提及**的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-179">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="6a2ef-180">[删除](../api/message-delete.md#request-2)提及</span><span class="sxs-lookup"><span data-stu-id="6a2ef-180">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="6a2ef-181">无</span><span class="sxs-lookup"><span data-stu-id="6a2ef-181">None</span></span> |<span data-ttu-id="6a2ef-182">在已登录用户的邮箱中删除指定邮件中指定的提及项。</span><span class="sxs-lookup"><span data-stu-id="6a2ef-182">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

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
