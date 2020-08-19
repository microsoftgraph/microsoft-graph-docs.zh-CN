---
title: governanceRuleSetting 资源类型
description: 表示角色设置所组成的规则。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 45ae44dccba67ee0b03f1941dd27795a002e810b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809521"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="769db-103">governanceRuleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="769db-103">governanceRuleSetting resource type</span></span>

<span data-ttu-id="769db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="769db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="769db-105">表示角色设置所组成的规则。</span><span class="sxs-lookup"><span data-stu-id="769db-105">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="769db-106">属性</span><span class="sxs-lookup"><span data-stu-id="769db-106">Properties</span></span>
|<span data-ttu-id="769db-107">属性</span><span class="sxs-lookup"><span data-stu-id="769db-107">Property</span></span>      | <span data-ttu-id="769db-108">类型</span><span class="sxs-lookup"><span data-stu-id="769db-108">Type</span></span>         |<span data-ttu-id="769db-109">说明</span><span class="sxs-lookup"><span data-stu-id="769db-109">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="769db-110">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="769db-110">ruleIdentifier</span></span>|<span data-ttu-id="769db-111">String</span><span class="sxs-lookup"><span data-stu-id="769db-111">String</span></span>        |<span data-ttu-id="769db-112">规则的 id。</span><span class="sxs-lookup"><span data-stu-id="769db-112">The id of the rule.</span></span> <span data-ttu-id="769db-113">例如 ``ExpirationRule`` 和 ``MfaRule`` 。</span><span class="sxs-lookup"><span data-stu-id="769db-113">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="769db-114">setting</span><span class="sxs-lookup"><span data-stu-id="769db-114">setting</span></span>       |<span data-ttu-id="769db-115">String</span><span class="sxs-lookup"><span data-stu-id="769db-115">String</span></span>        |<span data-ttu-id="769db-116">规则的设置。</span><span class="sxs-lookup"><span data-stu-id="769db-116">The settings of the rule.</span></span> <span data-ttu-id="769db-117">此值是一个 JSON 字符串，其格式为 Parameter_Name： Parameter_Value 的一对列表。</span><span class="sxs-lookup"><span data-stu-id="769db-117">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="769db-118">例如，`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="769db-118">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="769db-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="769db-119">JSON representation</span></span>

<span data-ttu-id="769db-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="769db-120">Here is a JSON representation of the resource.</span></span>

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
