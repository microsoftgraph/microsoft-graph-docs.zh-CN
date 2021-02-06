---
title: governanceRuleSetting 资源类型
description: 表示角色设置所组成的规则。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: b55ddfea8f46f9d064b4a032a804c2c5f4847d1a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132690"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="056c7-103">governanceRuleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="056c7-103">governanceRuleSetting resource type</span></span>

<span data-ttu-id="056c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="056c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="056c7-105">表示角色设置所组成的规则。</span><span class="sxs-lookup"><span data-stu-id="056c7-105">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="056c7-106">属性</span><span class="sxs-lookup"><span data-stu-id="056c7-106">Properties</span></span>
|<span data-ttu-id="056c7-107">属性</span><span class="sxs-lookup"><span data-stu-id="056c7-107">Property</span></span>      | <span data-ttu-id="056c7-108">类型</span><span class="sxs-lookup"><span data-stu-id="056c7-108">Type</span></span>         |<span data-ttu-id="056c7-109">说明</span><span class="sxs-lookup"><span data-stu-id="056c7-109">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="056c7-110">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="056c7-110">ruleIdentifier</span></span>|<span data-ttu-id="056c7-111">字符串</span><span class="sxs-lookup"><span data-stu-id="056c7-111">String</span></span>        |<span data-ttu-id="056c7-112">规则的 ID。</span><span class="sxs-lookup"><span data-stu-id="056c7-112">The id of the rule.</span></span> <span data-ttu-id="056c7-113">例如， ``ExpirationRule`` ``MfaRule`` 和 。</span><span class="sxs-lookup"><span data-stu-id="056c7-113">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="056c7-114">setting</span><span class="sxs-lookup"><span data-stu-id="056c7-114">setting</span></span>       |<span data-ttu-id="056c7-115">String</span><span class="sxs-lookup"><span data-stu-id="056c7-115">String</span></span>        |<span data-ttu-id="056c7-116">规则的设置。</span><span class="sxs-lookup"><span data-stu-id="056c7-116">The settings of the rule.</span></span> <span data-ttu-id="056c7-117">该值是 JSON 字符串，其对列表的格式为 Parameter_Name：Parameter_Value。</span><span class="sxs-lookup"><span data-stu-id="056c7-117">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="056c7-118">例如，`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="056c7-118">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="056c7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="056c7-119">JSON representation</span></span>

<span data-ttu-id="056c7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="056c7-120">Here is a JSON representation of the resource.</span></span>

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


