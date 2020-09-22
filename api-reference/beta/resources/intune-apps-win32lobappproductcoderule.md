---
title: win32LobAppProductCodeRule 资源类型
description: 一个用于存储 Win32 LOB 应用程序的产品代码和版本规则数据的复杂类型。 不支持将此规则作为要求规则。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11990f4deddb7bf29b9b447ae65e1903f6ecbc2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092802"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="0c717-104">win32LobAppProductCodeRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c717-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="0c717-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c717-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c717-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0c717-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c717-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c717-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c717-108">一个用于存储 Win32 LOB 应用程序的产品代码和版本规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="0c717-108">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="0c717-109">不支持将此规则作为要求规则。</span><span class="sxs-lookup"><span data-stu-id="0c717-109">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="0c717-110">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="0c717-110">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c717-111">属性</span><span class="sxs-lookup"><span data-stu-id="0c717-111">Properties</span></span>
|<span data-ttu-id="0c717-112">属性</span><span class="sxs-lookup"><span data-stu-id="0c717-112">Property</span></span>|<span data-ttu-id="0c717-113">类型</span><span class="sxs-lookup"><span data-stu-id="0c717-113">Type</span></span>|<span data-ttu-id="0c717-114">说明</span><span class="sxs-lookup"><span data-stu-id="0c717-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c717-115">ruleType</span><span class="sxs-lookup"><span data-stu-id="0c717-115">ruleType</span></span>|[<span data-ttu-id="0c717-116">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="0c717-116">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="0c717-117">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="0c717-117">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="0c717-118">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="0c717-118">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="0c717-119">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="0c717-119">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="0c717-120">productCode</span><span class="sxs-lookup"><span data-stu-id="0c717-120">productCode</span></span>|<span data-ttu-id="0c717-121">String</span><span class="sxs-lookup"><span data-stu-id="0c717-121">String</span></span>|<span data-ttu-id="0c717-122">应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="0c717-122">The product code of the app.</span></span>|
|<span data-ttu-id="0c717-123">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="0c717-123">productVersionOperator</span></span>|[<span data-ttu-id="0c717-124">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="0c717-124">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="0c717-125">产品版本比较运算符。</span><span class="sxs-lookup"><span data-stu-id="0c717-125">The product version comparison operator.</span></span> <span data-ttu-id="0c717-126">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="0c717-126">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="0c717-127">productVersion</span><span class="sxs-lookup"><span data-stu-id="0c717-127">productVersion</span></span>|<span data-ttu-id="0c717-128">String</span><span class="sxs-lookup"><span data-stu-id="0c717-128">String</span></span>|<span data-ttu-id="0c717-129">产品版本比较值。</span><span class="sxs-lookup"><span data-stu-id="0c717-129">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c717-130">关系</span><span class="sxs-lookup"><span data-stu-id="0c717-130">Relationships</span></span>
<span data-ttu-id="0c717-131">无</span><span class="sxs-lookup"><span data-stu-id="0c717-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c717-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c717-132">JSON Representation</span></span>
<span data-ttu-id="0c717-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c717-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeRule",
  "ruleType": "String",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```






