---
title: embeddedSIMActivationCode 资源类型
description: 为移动运营商提供嵌入的 SIM 激活代码。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af8bf020953dbc014f42aa6d363d3ca9e30db8a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987403"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="51e2e-103">embeddedSIMActivationCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="51e2e-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="51e2e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="51e2e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51e2e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="51e2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51e2e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="51e2e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51e2e-107">为移动运营商提供嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="51e2e-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="51e2e-108">属性</span><span class="sxs-lookup"><span data-stu-id="51e2e-108">Properties</span></span>
|<span data-ttu-id="51e2e-109">属性</span><span class="sxs-lookup"><span data-stu-id="51e2e-109">Property</span></span>|<span data-ttu-id="51e2e-110">类型</span><span class="sxs-lookup"><span data-stu-id="51e2e-110">Type</span></span>|<span data-ttu-id="51e2e-111">说明</span><span class="sxs-lookup"><span data-stu-id="51e2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e2e-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="51e2e-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="51e2e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="51e2e-113">String</span></span>|<span data-ttu-id="51e2e-114">由移动运营商提供，此集成电路卡标识符 (ICCID) 嵌入 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="51e2e-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="51e2e-115">输入项必须匹配以下正则表达式: ^\[0-9\]{19}\[0-9\]?$。</span><span class="sxs-lookup"><span data-stu-id="51e2e-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="51e2e-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="51e2e-116">matchingIdentifier</span></span>|<span data-ttu-id="51e2e-117">字符串</span><span class="sxs-lookup"><span data-stu-id="51e2e-117">String</span></span>|<span data-ttu-id="51e2e-118">GSMA 关联 SGP.22 RSP 技术规范 4.1 节中的规定 MatchingIdentifier (MatchingID)。</span><span class="sxs-lookup"><span data-stu-id="51e2e-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="51e2e-119">输入项必须匹配以下正则表达式: ^\[a-zA-Z0-9\-\]\* $。</span><span class="sxs-lookup"><span data-stu-id="51e2e-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="51e2e-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="51e2e-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="51e2e-121">字符串</span><span class="sxs-lookup"><span data-stu-id="51e2e-121">String</span></span>|<span data-ttu-id="51e2e-122">SM 的完全限定的域名-DP + GSM 关联 SPG.22 RSP 技术规范中指定的服务器。</span><span class="sxs-lookup"><span data-stu-id="51e2e-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="51e2e-123">输入项必须匹配以下正则表达式: ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-ZA-Z\]{2,}$。</span><span class="sxs-lookup"><span data-stu-id="51e2e-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51e2e-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="51e2e-124">Relationships</span></span>
<span data-ttu-id="51e2e-125">无</span><span class="sxs-lookup"><span data-stu-id="51e2e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51e2e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51e2e-126">JSON Representation</span></span>
<span data-ttu-id="51e2e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51e2e-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```





