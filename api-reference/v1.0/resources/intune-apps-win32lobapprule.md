---
title: win32LobAppRule 资源类型
description: 用于存储 Win32 LOB 应用的检测或要求规则数据的基复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1494aa6089bac73ae14612804009237bb9a5b2fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758958"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="1a34a-103">win32LobAppRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a34a-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="1a34a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a34a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a34a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a34a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a34a-106">用于存储 Win32 LOB 应用的检测或要求规则数据的基复杂类型。</span><span class="sxs-lookup"><span data-stu-id="1a34a-106">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="1a34a-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a34a-107">Properties</span></span>
|<span data-ttu-id="1a34a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a34a-108">Property</span></span>|<span data-ttu-id="1a34a-109">类型</span><span class="sxs-lookup"><span data-stu-id="1a34a-109">Type</span></span>|<span data-ttu-id="1a34a-110">说明</span><span class="sxs-lookup"><span data-stu-id="1a34a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a34a-111">ruleType</span><span class="sxs-lookup"><span data-stu-id="1a34a-111">ruleType</span></span>|[<span data-ttu-id="1a34a-112">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="1a34a-112">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="1a34a-113">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="1a34a-113">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="1a34a-114">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="1a34a-114">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a34a-115">关系</span><span class="sxs-lookup"><span data-stu-id="1a34a-115">Relationships</span></span>
<span data-ttu-id="1a34a-116">无</span><span class="sxs-lookup"><span data-stu-id="1a34a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a34a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a34a-117">JSON Representation</span></span>
<span data-ttu-id="1a34a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a34a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRule",
  "ruleType": "String"
}
```




