---
title: win32LobAppRule 资源类型
description: 用于存储 Win32 LOB 应用程序的检测或要求规则数据的基本复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec25bb546cb38213f59f9a3ebece71de5db5e336
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706112"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="df4cf-103">win32LobAppRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="df4cf-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="df4cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df4cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df4cf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df4cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df4cf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df4cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df4cf-107">用于存储 Win32 LOB 应用程序的检测或要求规则数据的基本复杂类型。</span><span class="sxs-lookup"><span data-stu-id="df4cf-107">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="df4cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="df4cf-108">Properties</span></span>
|<span data-ttu-id="df4cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="df4cf-109">Property</span></span>|<span data-ttu-id="df4cf-110">类型</span><span class="sxs-lookup"><span data-stu-id="df4cf-110">Type</span></span>|<span data-ttu-id="df4cf-111">说明</span><span class="sxs-lookup"><span data-stu-id="df4cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df4cf-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="df4cf-112">ruleType</span></span>|[<span data-ttu-id="df4cf-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="df4cf-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="df4cf-114">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="df4cf-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="df4cf-115">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="df4cf-115">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df4cf-116">关系</span><span class="sxs-lookup"><span data-stu-id="df4cf-116">Relationships</span></span>
<span data-ttu-id="df4cf-117">无</span><span class="sxs-lookup"><span data-stu-id="df4cf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df4cf-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df4cf-118">JSON Representation</span></span>
<span data-ttu-id="df4cf-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df4cf-119">Here is a JSON representation of the resource.</span></span>
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





