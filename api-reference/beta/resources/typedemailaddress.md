---
title: typedEmailAddress 资源类型
description: 表示的名称、 电子邮件地址和其相应的电子邮件地址类型的联系人。
localization_priority: Normal
ms.openlocfilehash: c77d3dddc3e2bfcac47e6ed245dad9223fe7f08c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871265"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="00f3d-103">typedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="00f3d-103">typedEmailAddress resource type</span></span>

> <span data-ttu-id="00f3d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00f3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00f3d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00f3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00f3d-106">表示的名称、 电子邮件地址和其相应的电子邮件地址类型的[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="00f3d-106">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="00f3d-107">属性</span><span class="sxs-lookup"><span data-stu-id="00f3d-107">Properties</span></span>
| <span data-ttu-id="00f3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="00f3d-108">Property</span></span>     | <span data-ttu-id="00f3d-109">类型</span><span class="sxs-lookup"><span data-stu-id="00f3d-109">Type</span></span>   |<span data-ttu-id="00f3d-110">说明</span><span class="sxs-lookup"><span data-stu-id="00f3d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00f3d-111">address</span><span class="sxs-lookup"><span data-stu-id="00f3d-111">address</span></span>|<span data-ttu-id="00f3d-112">String</span><span class="sxs-lookup"><span data-stu-id="00f3d-112">String</span></span>|<span data-ttu-id="00f3d-113">联系人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="00f3d-113">The email address of a contact.</span></span>|
|<span data-ttu-id="00f3d-114">name</span><span class="sxs-lookup"><span data-stu-id="00f3d-114">name</span></span>|<span data-ttu-id="00f3d-115">字符串</span><span class="sxs-lookup"><span data-stu-id="00f3d-115">String</span></span>|<span data-ttu-id="00f3d-116">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="00f3d-116">The display name of a contact.</span></span>|
|<span data-ttu-id="00f3d-117">type</span><span class="sxs-lookup"><span data-stu-id="00f3d-117">type</span></span> |<span data-ttu-id="00f3d-118">字符串</span><span class="sxs-lookup"><span data-stu-id="00f3d-118">String</span></span> |<span data-ttu-id="00f3d-119">电子邮件地址类型。</span><span class="sxs-lookup"><span data-stu-id="00f3d-119">The type of email address.</span></span> <span data-ttu-id="00f3d-120">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="00f3d-120">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="00f3d-121">默认值是`unknown`，这意味着**地址**尚未设置为特定的类型。</span><span class="sxs-lookup"><span data-stu-id="00f3d-121">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="00f3d-122">otherLabel</span><span class="sxs-lookup"><span data-stu-id="00f3d-122">otherLabel</span></span> |<span data-ttu-id="00f3d-123">字符串</span><span class="sxs-lookup"><span data-stu-id="00f3d-123">String</span></span>  |<span data-ttu-id="00f3d-124">若要指定自定义类型的电子邮件地址，请将**类型**设置为`other`，并将**otherLabel**分配给自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="00f3d-124">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="00f3d-125">例如，您可以使用特定的电子邮件地址您自愿活动。</span><span class="sxs-lookup"><span data-stu-id="00f3d-125">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="00f3d-126">**类型**设置为`other`，如设置为自定义字符串**otherLabel** `Volunteer work`。</span><span class="sxs-lookup"><span data-stu-id="00f3d-126">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="00f3d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00f3d-127">JSON representation</span></span>

<span data-ttu-id="00f3d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00f3d-128">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
