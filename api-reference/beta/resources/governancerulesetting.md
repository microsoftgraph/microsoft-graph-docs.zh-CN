---
title: governanceRuleSetting 资源类型
description: 表示角色设置组成的规则。
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522236"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="78ac4-103">governanceRuleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="78ac4-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78ac4-104">表示角色设置组成的规则。</span><span class="sxs-lookup"><span data-stu-id="78ac4-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="78ac4-105">属性</span><span class="sxs-lookup"><span data-stu-id="78ac4-105">Properties</span></span>
|<span data-ttu-id="78ac4-106">属性</span><span class="sxs-lookup"><span data-stu-id="78ac4-106">Property</span></span>      | <span data-ttu-id="78ac4-107">类型</span><span class="sxs-lookup"><span data-stu-id="78ac4-107">Type</span></span>         |<span data-ttu-id="78ac4-108">说明</span><span class="sxs-lookup"><span data-stu-id="78ac4-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="78ac4-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="78ac4-109">ruleIdentifier</span></span>|<span data-ttu-id="78ac4-110">String</span><span class="sxs-lookup"><span data-stu-id="78ac4-110">String</span></span>        |<span data-ttu-id="78ac4-111">规则的 id。</span><span class="sxs-lookup"><span data-stu-id="78ac4-111">The id of the rule.</span></span> <span data-ttu-id="78ac4-112">例如，``ExpirationRule``和``MfaRule``。</span><span class="sxs-lookup"><span data-stu-id="78ac4-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="78ac4-113">setting</span><span class="sxs-lookup"><span data-stu-id="78ac4-113">setting</span></span>       |<span data-ttu-id="78ac4-114">String</span><span class="sxs-lookup"><span data-stu-id="78ac4-114">String</span></span>        |<span data-ttu-id="78ac4-115">规则的设置。</span><span class="sxs-lookup"><span data-stu-id="78ac4-115">The settings of the rule.</span></span> <span data-ttu-id="78ac4-116">值为 string JSON 格式的 Parameter_Name:Parameter_Value 对的列表。</span><span class="sxs-lookup"><span data-stu-id="78ac4-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="78ac4-117">例如，`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="78ac4-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78ac4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78ac4-118">JSON representation</span></span>

<span data-ttu-id="78ac4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78ac4-119">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerulesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
