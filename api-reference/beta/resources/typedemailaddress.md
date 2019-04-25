---
title: typedEmailAddress 资源类型
description: 表示联系人的名称、电子邮件地址及其对应的电子邮件地址类型。
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576456"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="fa78d-103">typedEmailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa78d-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa78d-104">表示[联系人](contact.md)的名称、电子邮件地址及其对应的电子邮件地址类型。</span><span class="sxs-lookup"><span data-stu-id="fa78d-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fa78d-105">属性</span><span class="sxs-lookup"><span data-stu-id="fa78d-105">Properties</span></span>
| <span data-ttu-id="fa78d-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa78d-106">Property</span></span>     | <span data-ttu-id="fa78d-107">类型</span><span class="sxs-lookup"><span data-stu-id="fa78d-107">Type</span></span>   |<span data-ttu-id="fa78d-108">说明</span><span class="sxs-lookup"><span data-stu-id="fa78d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa78d-109">address</span><span class="sxs-lookup"><span data-stu-id="fa78d-109">address</span></span>|<span data-ttu-id="fa78d-110">String</span><span class="sxs-lookup"><span data-stu-id="fa78d-110">String</span></span>|<span data-ttu-id="fa78d-111">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="fa78d-111">The email address of a contact.</span></span>|
|<span data-ttu-id="fa78d-112">name</span><span class="sxs-lookup"><span data-stu-id="fa78d-112">name</span></span>|<span data-ttu-id="fa78d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="fa78d-113">String</span></span>|<span data-ttu-id="fa78d-114">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fa78d-114">The display name of a contact.</span></span>|
|<span data-ttu-id="fa78d-115">type</span><span class="sxs-lookup"><span data-stu-id="fa78d-115">type</span></span> |<span data-ttu-id="fa78d-116">String</span><span class="sxs-lookup"><span data-stu-id="fa78d-116">String</span></span> |<span data-ttu-id="fa78d-117">电子邮件地址的类型。</span><span class="sxs-lookup"><span data-stu-id="fa78d-117">The type of email address.</span></span> <span data-ttu-id="fa78d-118">可取值为：`unknown`、`work`、`personal`、`main` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="fa78d-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="fa78d-119">默认值为`unknown`, 表示尚未将**地址**设置为特定类型。</span><span class="sxs-lookup"><span data-stu-id="fa78d-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="fa78d-120">otherLabel</span><span class="sxs-lookup"><span data-stu-id="fa78d-120">otherLabel</span></span> |<span data-ttu-id="fa78d-121">String</span><span class="sxs-lookup"><span data-stu-id="fa78d-121">String</span></span>  |<span data-ttu-id="fa78d-122">若要指定自定义类型的电子邮件地址\*\*\*\* , 请`other`将 "类型" 设置为, 并将**otherLabel**分配给自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="fa78d-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="fa78d-123">例如, 您可以对志愿者活动使用特定的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="fa78d-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="fa78d-124">将\*\*\*\* "类型`other`" 设置为, 并将**otherLabel**设置为自`Volunteer work`定义字符串, 例如。</span><span class="sxs-lookup"><span data-stu-id="fa78d-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa78d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa78d-125">JSON representation</span></span>

<span data-ttu-id="fa78d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa78d-126">Here is a JSON representation of the resource</span></span>

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
