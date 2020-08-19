---
title: typedEmailAddress 资源类型
description: 表示联系人的名称、电子邮件地址及其对应的电子邮件地址类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 6641d05542fb6d6e376343dff98508183f5a012b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812763"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="6ccc2-103">typedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ccc2-103">typedEmailAddress resource type</span></span>

<span data-ttu-id="6ccc2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ccc2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ccc2-105">表示 [联系人](contact.md)的名称、电子邮件地址及其对应的电子邮件地址类型。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-105">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6ccc2-106">属性</span><span class="sxs-lookup"><span data-stu-id="6ccc2-106">Properties</span></span>
| <span data-ttu-id="6ccc2-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ccc2-107">Property</span></span>     | <span data-ttu-id="6ccc2-108">类型</span><span class="sxs-lookup"><span data-stu-id="6ccc2-108">Type</span></span>   |<span data-ttu-id="6ccc2-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ccc2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ccc2-110">address</span><span class="sxs-lookup"><span data-stu-id="6ccc2-110">address</span></span>|<span data-ttu-id="6ccc2-111">String</span><span class="sxs-lookup"><span data-stu-id="6ccc2-111">String</span></span>|<span data-ttu-id="6ccc2-112">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-112">The email address of a contact.</span></span>|
|<span data-ttu-id="6ccc2-113">name</span><span class="sxs-lookup"><span data-stu-id="6ccc2-113">name</span></span>|<span data-ttu-id="6ccc2-114">String</span><span class="sxs-lookup"><span data-stu-id="6ccc2-114">String</span></span>|<span data-ttu-id="6ccc2-115">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-115">The display name of a contact.</span></span>|
|<span data-ttu-id="6ccc2-116">type</span><span class="sxs-lookup"><span data-stu-id="6ccc2-116">type</span></span> |<span data-ttu-id="6ccc2-117">String</span><span class="sxs-lookup"><span data-stu-id="6ccc2-117">String</span></span> |<span data-ttu-id="6ccc2-118">电子邮件地址的类型。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-118">The type of email address.</span></span> <span data-ttu-id="6ccc2-119">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-119">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="6ccc2-120">默认值为 `unknown` ，表示尚未将 **地址** 设置为特定类型。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-120">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="6ccc2-121">otherLabel</span><span class="sxs-lookup"><span data-stu-id="6ccc2-121">otherLabel</span></span> |<span data-ttu-id="6ccc2-122">String</span><span class="sxs-lookup"><span data-stu-id="6ccc2-122">String</span></span>  |<span data-ttu-id="6ccc2-123">若要指定自定义类型的电子邮件地址，请将 " **类型** " 设置为 `other` ，并将 **otherLabel** 分配给自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-123">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="6ccc2-124">例如，您可以对志愿者活动使用特定的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-124">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="6ccc2-125">将 " **类型** " 设置为 `other` ，并将 **otherLabel** 设置为自定义字符串，例如 `Volunteer work` 。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-125">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ccc2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ccc2-126">JSON representation</span></span>

<span data-ttu-id="6ccc2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ccc2-127">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
