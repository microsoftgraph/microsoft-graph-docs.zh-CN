---
title: typedEmailAddress 资源类型
description: 表示的名称、 电子邮件地址和其相应的电子邮件地址类型的联系人。
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510706"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="2bbe1-103">typedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bbe1-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bbe1-104">表示的名称、 电子邮件地址和其相应的电子邮件地址类型的[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2bbe1-105">属性</span><span class="sxs-lookup"><span data-stu-id="2bbe1-105">Properties</span></span>
| <span data-ttu-id="2bbe1-106">属性</span><span class="sxs-lookup"><span data-stu-id="2bbe1-106">Property</span></span>     | <span data-ttu-id="2bbe1-107">类型</span><span class="sxs-lookup"><span data-stu-id="2bbe1-107">Type</span></span>   |<span data-ttu-id="2bbe1-108">说明</span><span class="sxs-lookup"><span data-stu-id="2bbe1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bbe1-109">address</span><span class="sxs-lookup"><span data-stu-id="2bbe1-109">address</span></span>|<span data-ttu-id="2bbe1-110">String</span><span class="sxs-lookup"><span data-stu-id="2bbe1-110">String</span></span>|<span data-ttu-id="2bbe1-111">联系人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-111">The email address of a contact.</span></span>|
|<span data-ttu-id="2bbe1-112">name</span><span class="sxs-lookup"><span data-stu-id="2bbe1-112">name</span></span>|<span data-ttu-id="2bbe1-113">String</span><span class="sxs-lookup"><span data-stu-id="2bbe1-113">String</span></span>|<span data-ttu-id="2bbe1-114">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-114">The display name of a contact.</span></span>|
|<span data-ttu-id="2bbe1-115">type</span><span class="sxs-lookup"><span data-stu-id="2bbe1-115">type</span></span> |<span data-ttu-id="2bbe1-116">字符串</span><span class="sxs-lookup"><span data-stu-id="2bbe1-116">String</span></span> |<span data-ttu-id="2bbe1-117">电子邮件地址类型。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-117">The type of email address.</span></span> <span data-ttu-id="2bbe1-118">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="2bbe1-119">默认值是`unknown`，这意味着**地址**尚未设置为特定的类型。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="2bbe1-120">otherLabel</span><span class="sxs-lookup"><span data-stu-id="2bbe1-120">otherLabel</span></span> |<span data-ttu-id="2bbe1-121">String</span><span class="sxs-lookup"><span data-stu-id="2bbe1-121">String</span></span>  |<span data-ttu-id="2bbe1-122">若要指定自定义类型的电子邮件地址，请将**类型**设置为`other`，并将**otherLabel**分配给自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="2bbe1-123">例如，您可以使用特定的电子邮件地址您自愿活动。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="2bbe1-124">**类型**设置为`other`，如设置为自定义字符串**otherLabel** `Volunteer work`。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2bbe1-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bbe1-125">JSON representation</span></span>

<span data-ttu-id="2bbe1-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bbe1-126">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
