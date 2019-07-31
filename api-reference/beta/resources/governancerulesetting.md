---
title: governanceRuleSetting 资源类型
description: 表示角色设置所组成的规则。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bfc3bb7895a3ec66a32456b48901fc456d3c3b2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971866"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="947b2-103">governanceRuleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="947b2-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="947b2-104">表示角色设置所组成的规则。</span><span class="sxs-lookup"><span data-stu-id="947b2-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="947b2-105">属性</span><span class="sxs-lookup"><span data-stu-id="947b2-105">Properties</span></span>
|<span data-ttu-id="947b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="947b2-106">Property</span></span>      | <span data-ttu-id="947b2-107">类型</span><span class="sxs-lookup"><span data-stu-id="947b2-107">Type</span></span>         |<span data-ttu-id="947b2-108">说明</span><span class="sxs-lookup"><span data-stu-id="947b2-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="947b2-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="947b2-109">ruleIdentifier</span></span>|<span data-ttu-id="947b2-110">String</span><span class="sxs-lookup"><span data-stu-id="947b2-110">String</span></span>        |<span data-ttu-id="947b2-111">规则的 id。</span><span class="sxs-lookup"><span data-stu-id="947b2-111">The id of the rule.</span></span> <span data-ttu-id="947b2-112">例如``ExpirationRule``和``MfaRule``。</span><span class="sxs-lookup"><span data-stu-id="947b2-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="947b2-113">setting</span><span class="sxs-lookup"><span data-stu-id="947b2-113">setting</span></span>       |<span data-ttu-id="947b2-114">String</span><span class="sxs-lookup"><span data-stu-id="947b2-114">String</span></span>        |<span data-ttu-id="947b2-115">规则的设置。</span><span class="sxs-lookup"><span data-stu-id="947b2-115">The settings of the rule.</span></span> <span data-ttu-id="947b2-116">该值是一个包含 Parameter_Name: Parameter_Value 格式的对列表的 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="947b2-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="947b2-117">例如，`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="947b2-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="947b2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="947b2-118">JSON representation</span></span>

<span data-ttu-id="947b2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="947b2-119">Here is a JSON representation of the resource.</span></span>

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
