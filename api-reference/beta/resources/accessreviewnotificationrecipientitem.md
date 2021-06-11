---
title: accessReviewNotificationRecipientItem 资源类型
description: 定义将接收通知的用户或组访问审阅通知。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3d6ed767f1350f3e4a43a1b31363920ffb58a9b5
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896731"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a><span data-ttu-id="ecbc9-103">accessReviewNotificationRecipientItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ecbc9-103">accessReviewNotificationRecipientItem resource type</span></span>

<span data-ttu-id="ecbc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecbc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


<span data-ttu-id="ecbc9-105">表示评价实例 [上的](accessreviewsv2-root.md) Azure AD 访问评审通知事件。</span><span class="sxs-lookup"><span data-stu-id="ecbc9-105">Represents an Azure AD [access review](accessreviewsv2-root.md) notification event on an instance of a review.</span></span> <span data-ttu-id="ecbc9-106">此项目包含电子邮件模板类型和收件人属性，以允许发送给定访问评审实例的某些类型的 [通知](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="ecbc9-106">This item contains an email template type and recipient properties to enable sending certain type of notifications for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ecbc9-107">属性</span><span class="sxs-lookup"><span data-stu-id="ecbc9-107">Properties</span></span>

| <span data-ttu-id="ecbc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="ecbc9-108">Property</span></span>                     | <span data-ttu-id="ecbc9-109">类型</span><span class="sxs-lookup"><span data-stu-id="ecbc9-109">Type</span></span>     | <span data-ttu-id="ecbc9-110">说明</span><span class="sxs-lookup"><span data-stu-id="ecbc9-110">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| <span data-ttu-id="ecbc9-111">notificationTemplateType</span><span class="sxs-lookup"><span data-stu-id="ecbc9-111">notificationTemplateType</span></span>  |<span data-ttu-id="ecbc9-112">String</span><span class="sxs-lookup"><span data-stu-id="ecbc9-112">String</span></span>  | <span data-ttu-id="ecbc9-113">指示要发送的访问评审电子邮件的类型。</span><span class="sxs-lookup"><span data-stu-id="ecbc9-113">Indicates the type of access review email to be sent.</span></span> <span data-ttu-id="ecbc9-114">支持的模板类型 `CompletedAdditionalRecipients` 是向收件人发送审阅完成通知的类型。</span><span class="sxs-lookup"><span data-stu-id="ecbc9-114">Supported template type is `CompletedAdditionalRecipients` which sends review completion notifications to the recipients.</span></span>|
| <span data-ttu-id="ecbc9-115">notificationRecipientScope</span><span class="sxs-lookup"><span data-stu-id="ecbc9-115">notificationRecipientScope</span></span> |[<span data-ttu-id="ecbc9-116">accessReviewNotificationRecipientScope</span><span class="sxs-lookup"><span data-stu-id="ecbc9-116">accessReviewNotificationRecipientScope</span></span>](../resources/accessreviewnotificationrecipientscope.md)  | <span data-ttu-id="ecbc9-117">确定通知电子邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="ecbc9-117">Determines the recipient of the notification email.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecbc9-118">关系</span><span class="sxs-lookup"><span data-stu-id="ecbc9-118">Relationships</span></span>
<span data-ttu-id="ecbc9-119">无。</span><span class="sxs-lookup"><span data-stu-id="ecbc9-119">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ecbc9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecbc9-120">JSON representation</span></span>

<span data-ttu-id="ecbc9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecbc9-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem",
  "openType": true
}
-->

```json
{
  "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientItem",
  "notificationRecipientScope": {
      "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientQueryScope"                
    },
  "notificationTemplateType": "String"
}
```
