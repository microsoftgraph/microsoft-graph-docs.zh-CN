---
title: 提及资源类型
description: 表示基于人员的电子邮件地址的人员通知。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a51a13d8aae562ab4a051124a1e0197065661058
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971592"
---
# <a name="mention-resource-type"></a><span data-ttu-id="f858e-103">提及资源类型</span><span class="sxs-lookup"><span data-stu-id="f858e-103">mention resource type</span></span>

<span data-ttu-id="f858e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f858e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f858e-105">表示基于人员的电子邮件地址的人员通知。</span><span class="sxs-lookup"><span data-stu-id="f858e-105">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="f858e-106">这种类型的通知也称为 @ 提到。</span><span class="sxs-lookup"><span data-stu-id="f858e-106">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="f858e-107">[邮件](../resources/message.md)资源支持**提到**。</span><span class="sxs-lookup"><span data-stu-id="f858e-107">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="f858e-108">它包含一个 **mentionsPreview** 属性，该属性指示该邮件实例中是否提到已登录用户。</span><span class="sxs-lookup"><span data-stu-id="f858e-108">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="f858e-109">它还包括 **提及** 导航属性，该属性支持获取提及的详细信息，或删除该实例中的提及。</span><span class="sxs-lookup"><span data-stu-id="f858e-109">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="f858e-110">创建邮件时，应用程序可以 `POST` 通过在 **提及** 属性中添加提及的内容，在同一请求中创建记录。</span><span class="sxs-lookup"><span data-stu-id="f858e-110">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="f858e-111">使用 `GET` 查询参数的请求 `$filter` ，应用程序可以返回登录用户的邮箱中提及用户的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="f858e-111">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="f858e-112">`GET`使用 `$expand` 查询参数的请求可让应用展开特定邮件中的所有提及。</span><span class="sxs-lookup"><span data-stu-id="f858e-112">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="f858e-113">允许在邮件中使用应用程序集和获取提及的机制启用轻量通知，其中提出提及的用户可以保留在现有上下文中 (例如，在应用程序设置基础 **提及** 属性时撰写邮件正文) 。</span><span class="sxs-lookup"><span data-stu-id="f858e-113">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="f858e-114">提到的人员可以通过 `GET` `$filter` 或查询参数轻松了解是否以及在请求中提及的情况 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="f858e-114">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="f858e-115">例如，在 Outlook 邮件客户端中，当用户在 `@` 撰写邮件时键入时，Outlook 允许用户选择或输入名称来完成 @-提及。</span><span class="sxs-lookup"><span data-stu-id="f858e-115">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="f858e-116">Outlook 在创建和发送邮件或事件之前设置 **提及** 属性。</span><span class="sxs-lookup"><span data-stu-id="f858e-116">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="f858e-117">Outlook 还使用 `GET` 与和的操作， `$filter` `$expand` 以让登录用户查找提及用户的邮件，提醒用户执行操作项目或讨论，这样可以更快地响应。</span><span class="sxs-lookup"><span data-stu-id="f858e-117">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f858e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f858e-118">JSON representation</span></span>

<span data-ttu-id="f858e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f858e-119">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f858e-120">属性</span><span class="sxs-lookup"><span data-stu-id="f858e-120">Properties</span></span>
| <span data-ttu-id="f858e-121">属性</span><span class="sxs-lookup"><span data-stu-id="f858e-121">Property</span></span>     | <span data-ttu-id="f858e-122">类型</span><span class="sxs-lookup"><span data-stu-id="f858e-122">Type</span></span>   |<span data-ttu-id="f858e-123">说明</span><span class="sxs-lookup"><span data-stu-id="f858e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f858e-124">application</span><span class="sxs-lookup"><span data-stu-id="f858e-124">application</span></span> | <span data-ttu-id="f858e-125">String</span><span class="sxs-lookup"><span data-stu-id="f858e-125">String</span></span> | <span data-ttu-id="f858e-126">在其中创建提及的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="f858e-126">The name of the application where the mention is created.</span></span> <span data-ttu-id="f858e-127">可选。</span><span class="sxs-lookup"><span data-stu-id="f858e-127">Optional.</span></span> <span data-ttu-id="f858e-128">不会对 **邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="f858e-128">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="f858e-129">clientReference</span><span class="sxs-lookup"><span data-stu-id="f858e-129">clientReference</span></span> | <span data-ttu-id="f858e-130">String</span><span class="sxs-lookup"><span data-stu-id="f858e-130">String</span></span> | <span data-ttu-id="f858e-131">代表资源实例的父项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f858e-131">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="f858e-132">可选。</span><span class="sxs-lookup"><span data-stu-id="f858e-132">Optional.</span></span> <span data-ttu-id="f858e-133">不会对 **邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="f858e-133">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="f858e-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="f858e-134">createdBy</span></span>  | [<span data-ttu-id="f858e-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f858e-135">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="f858e-136">提出提及的用户的电子邮件信息。</span><span class="sxs-lookup"><span data-stu-id="f858e-136">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="f858e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f858e-137">createdDateTime</span></span>  |<span data-ttu-id="f858e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f858e-138">DateTimeOffset</span></span> |<span data-ttu-id="f858e-139">在客户端上创建提及的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f858e-139">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="f858e-140">deepLink</span><span class="sxs-lookup"><span data-stu-id="f858e-140">deepLink</span></span> | <span data-ttu-id="f858e-141">String</span><span class="sxs-lookup"><span data-stu-id="f858e-141">String</span></span> | <span data-ttu-id="f858e-142">指向资源实例中提及的上下文的深层 web 链接。</span><span class="sxs-lookup"><span data-stu-id="f858e-142">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="f858e-143">可选。</span><span class="sxs-lookup"><span data-stu-id="f858e-143">Optional.</span></span> <span data-ttu-id="f858e-144">不会对 **邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="f858e-144">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="f858e-145">id</span><span class="sxs-lookup"><span data-stu-id="f858e-145">id</span></span> | <span data-ttu-id="f858e-146">String</span><span class="sxs-lookup"><span data-stu-id="f858e-146">String</span></span>| <span data-ttu-id="f858e-147">资源实例中提及的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f858e-147">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="f858e-148">所</span><span class="sxs-lookup"><span data-stu-id="f858e-148">mentioned</span></span> | [<span data-ttu-id="f858e-149">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f858e-149">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="f858e-150">提到的人员的电子邮件信息。</span><span class="sxs-lookup"><span data-stu-id="f858e-150">The email information of the mentioned person.</span></span> <span data-ttu-id="f858e-151">必需。</span><span class="sxs-lookup"><span data-stu-id="f858e-151">Required.</span></span> |
|<span data-ttu-id="f858e-152">mentionText</span><span class="sxs-lookup"><span data-stu-id="f858e-152">mentionText</span></span> | <span data-ttu-id="f858e-153">String</span><span class="sxs-lookup"><span data-stu-id="f858e-153">String</span></span> | <span data-ttu-id="f858e-154">可选。</span><span class="sxs-lookup"><span data-stu-id="f858e-154">Optional.</span></span> <span data-ttu-id="f858e-155">不会对 **邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="f858e-155">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="f858e-156">若要获取邮件中提及的内容，请改为查看邮件的 **bodyPreview** 属性。</span><span class="sxs-lookup"><span data-stu-id="f858e-156">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="f858e-157">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f858e-157">serverCreatedDateTime</span></span> | <span data-ttu-id="f858e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f858e-158">DateTimeOffset</span></span> | <span data-ttu-id="f858e-159">在服务器上创建提及的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f858e-159">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="f858e-160">可选。</span><span class="sxs-lookup"><span data-stu-id="f858e-160">Optional.</span></span> <span data-ttu-id="f858e-161">不会对 **邮件**使用和默认为 null。</span><span class="sxs-lookup"><span data-stu-id="f858e-161">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f858e-162">关系</span><span class="sxs-lookup"><span data-stu-id="f858e-162">Relationships</span></span>
<span data-ttu-id="f858e-163">无</span><span class="sxs-lookup"><span data-stu-id="f858e-163">None</span></span>


## <a name="methods"></a><span data-ttu-id="f858e-164">方法</span><span class="sxs-lookup"><span data-stu-id="f858e-164">Methods</span></span>

| <span data-ttu-id="f858e-165">方法</span><span class="sxs-lookup"><span data-stu-id="f858e-165">Method</span></span>           | <span data-ttu-id="f858e-166">返回类型</span><span class="sxs-lookup"><span data-stu-id="f858e-166">Return Type</span></span>    |<span data-ttu-id="f858e-167">说明</span><span class="sxs-lookup"><span data-stu-id="f858e-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f858e-168">[Post](../api/user-sendmail.md#request-2) 和 send</span><span class="sxs-lookup"><span data-stu-id="f858e-168">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="f858e-169">无</span><span class="sxs-lookup"><span data-stu-id="f858e-169">None</span></span> | <span data-ttu-id="f858e-170">创建并将提及作为新邮件的一部分发送。</span><span class="sxs-lookup"><span data-stu-id="f858e-170">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="f858e-171">[发布](../api/user-post-messages.md#request-2) 到新草稿</span><span class="sxs-lookup"><span data-stu-id="f858e-171">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="f858e-172">包含一个或多个**提及**对象的[邮件](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="f858e-172">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="f858e-173">创建新邮件的草稿并包含一个或多个 **提及** 的对象。</span><span class="sxs-lookup"><span data-stu-id="f858e-173">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="f858e-174">[获取](../api/user-list-messages.md#request-2) 涉及我的邮件</span><span class="sxs-lookup"><span data-stu-id="f858e-174">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="f858e-175">[message](../resources/message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f858e-175">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="f858e-176">获取已登录用户邮箱中的所有邮件，其中包含此用户的 **提及** 。</span><span class="sxs-lookup"><span data-stu-id="f858e-176">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="f858e-177">[获取](../api/message-get.md#example-2) 邮件及其提及内容</span><span class="sxs-lookup"><span data-stu-id="f858e-177">[Get](../api/message-get.md#example-2) a message and its mentions</span></span> | <span data-ttu-id="f858e-178">[message](../resources/message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f858e-178">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="f858e-179">获取邮件并展开邮件中每个 **提及** 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f858e-179">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="f858e-180">[删除](../api/message-delete.md#request-2) 提及</span><span class="sxs-lookup"><span data-stu-id="f858e-180">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="f858e-181">无</span><span class="sxs-lookup"><span data-stu-id="f858e-181">None</span></span> |<span data-ttu-id="f858e-182">在已登录用户的邮箱中删除指定邮件中指定的提及项。</span><span class="sxs-lookup"><span data-stu-id="f858e-182">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

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


