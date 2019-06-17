---
title: embeddedSIMActivationCode 资源类型
description: 移动运营商提供的嵌入的 SIM 激活代码。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c96bc6530de0e8e6d1fde95fa71ffb6f1bdedb18
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994879"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="eac3d-103">embeddedSIMActivationCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="eac3d-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="eac3d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eac3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eac3d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eac3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eac3d-106">移动运营商提供的嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="eac3d-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="eac3d-107">属性</span><span class="sxs-lookup"><span data-stu-id="eac3d-107">Properties</span></span>
|<span data-ttu-id="eac3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="eac3d-108">Property</span></span>|<span data-ttu-id="eac3d-109">类型</span><span class="sxs-lookup"><span data-stu-id="eac3d-109">Type</span></span>|<span data-ttu-id="eac3d-110">说明</span><span class="sxs-lookup"><span data-stu-id="eac3d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac3d-111">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="eac3d-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="eac3d-112">String</span><span class="sxs-lookup"><span data-stu-id="eac3d-112">String</span></span>|<span data-ttu-id="eac3d-113">由移动运营商提供的此嵌入的 SIM 激活代码的集成电路卡标识符 (ICCID)。</span><span class="sxs-lookup"><span data-stu-id="eac3d-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="eac3d-114">输入必须与以下正则表达式匹配: ' ^\[0-9\]{19}\[0-9\]？ $ '。</span><span class="sxs-lookup"><span data-stu-id="eac3d-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="eac3d-115">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="eac3d-115">matchingIdentifier</span></span>|<span data-ttu-id="eac3d-116">String</span><span class="sxs-lookup"><span data-stu-id="eac3d-116">String</span></span>|<span data-ttu-id="eac3d-117">GSMA Association SGP RSP 技术规范部分中指定的 MatchingIdentifier (MatchingID) 4.1。</span><span class="sxs-lookup"><span data-stu-id="eac3d-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="eac3d-118">输入必须与以下正则表达式匹配: ' ^\[Z0-9\-\]\* $ '。</span><span class="sxs-lookup"><span data-stu-id="eac3d-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="eac3d-119">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="eac3d-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="eac3d-120">String</span><span class="sxs-lookup"><span data-stu-id="eac3d-120">String</span></span>|<span data-ttu-id="eac3d-121">在 GSM 关联 SPG .22 RSP 技术规范中指定的 SM + 服务器的完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="eac3d-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="eac3d-122">输入必须与以下正则表达式匹配: "^ (\[Z0-9\]+ (\[-a-Z0-9\]+) \*\.) +\[-za-Z\]{2,}$"。</span><span class="sxs-lookup"><span data-stu-id="eac3d-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eac3d-123">关系</span><span class="sxs-lookup"><span data-stu-id="eac3d-123">Relationships</span></span>
<span data-ttu-id="eac3d-124">无</span><span class="sxs-lookup"><span data-stu-id="eac3d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eac3d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eac3d-125">JSON Representation</span></span>
<span data-ttu-id="eac3d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eac3d-126">Here is a JSON representation of the resource.</span></span>
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





