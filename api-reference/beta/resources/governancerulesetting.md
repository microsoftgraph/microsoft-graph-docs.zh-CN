---
title: governanceRuleSetting 资源类型
description: 表示角色设置所组成的规则。
localization_priority: Normal
ms.openlocfilehash: 433fc0d3ab3a524b86bbf1fc46dbe5185549473b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333718"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="bf92f-103">governanceRuleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf92f-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf92f-104">表示角色设置所组成的规则。</span><span class="sxs-lookup"><span data-stu-id="bf92f-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="bf92f-105">属性</span><span class="sxs-lookup"><span data-stu-id="bf92f-105">Properties</span></span>
|<span data-ttu-id="bf92f-106">属性</span><span class="sxs-lookup"><span data-stu-id="bf92f-106">Property</span></span>      | <span data-ttu-id="bf92f-107">类型</span><span class="sxs-lookup"><span data-stu-id="bf92f-107">Type</span></span>         |<span data-ttu-id="bf92f-108">说明</span><span class="sxs-lookup"><span data-stu-id="bf92f-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="bf92f-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="bf92f-109">ruleIdentifier</span></span>|<span data-ttu-id="bf92f-110">String</span><span class="sxs-lookup"><span data-stu-id="bf92f-110">String</span></span>        |<span data-ttu-id="bf92f-111">规则的 id。</span><span class="sxs-lookup"><span data-stu-id="bf92f-111">The id of the rule.</span></span> <span data-ttu-id="bf92f-112">例如``ExpirationRule``和``MfaRule``。</span><span class="sxs-lookup"><span data-stu-id="bf92f-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="bf92f-113">setting</span><span class="sxs-lookup"><span data-stu-id="bf92f-113">setting</span></span>       |<span data-ttu-id="bf92f-114">String</span><span class="sxs-lookup"><span data-stu-id="bf92f-114">String</span></span>        |<span data-ttu-id="bf92f-115">规则的设置。</span><span class="sxs-lookup"><span data-stu-id="bf92f-115">The settings of the rule.</span></span> <span data-ttu-id="bf92f-116">该值是一个包含 Parameter_Name: Parameter_Value 格式的对列表的 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="bf92f-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="bf92f-117">例如，`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="bf92f-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf92f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf92f-118">JSON representation</span></span>

<span data-ttu-id="bf92f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf92f-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
