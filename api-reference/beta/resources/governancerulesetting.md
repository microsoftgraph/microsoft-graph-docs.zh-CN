---
title: governanceRuleSetting 资源类型
description: 表示角色设置组成的规则。
ms.openlocfilehash: 486b5163c59772c971cfc1d61a98817b7f0c16f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045676"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="0c356-103">governanceRuleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c356-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="0c356-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c356-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c356-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c356-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c356-106">表示角色设置组成的规则。</span><span class="sxs-lookup"><span data-stu-id="0c356-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="0c356-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c356-107">Properties</span></span>
|<span data-ttu-id="0c356-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c356-108">Property</span></span>      | <span data-ttu-id="0c356-109">类型</span><span class="sxs-lookup"><span data-stu-id="0c356-109">Type</span></span>         |<span data-ttu-id="0c356-110">说明</span><span class="sxs-lookup"><span data-stu-id="0c356-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="0c356-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c356-111">ruleIdentifier</span></span>|<span data-ttu-id="0c356-112">字符串</span><span class="sxs-lookup"><span data-stu-id="0c356-112">String</span></span>        |<span data-ttu-id="0c356-113">规则的 id。</span><span class="sxs-lookup"><span data-stu-id="0c356-113">The id of the rule.</span></span> <span data-ttu-id="0c356-114">例如，``ExpirationRule``和``MfaRule``。</span><span class="sxs-lookup"><span data-stu-id="0c356-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="0c356-115">setting</span><span class="sxs-lookup"><span data-stu-id="0c356-115">setting</span></span>       |<span data-ttu-id="0c356-116">String</span><span class="sxs-lookup"><span data-stu-id="0c356-116">String</span></span>        |<span data-ttu-id="0c356-117">规则的设置。</span><span class="sxs-lookup"><span data-stu-id="0c356-117">The settings of the rule.</span></span> <span data-ttu-id="0c356-118">值为 string JSON 格式的 Parameter_Name:Parameter_Value 对的列表。</span><span class="sxs-lookup"><span data-stu-id="0c356-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="0c356-119">例如，`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="0c356-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c356-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c356-120">JSON representation</span></span>

<span data-ttu-id="0c356-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c356-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->