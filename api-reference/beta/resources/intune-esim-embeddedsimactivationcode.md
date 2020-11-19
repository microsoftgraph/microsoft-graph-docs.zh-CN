---
title: embeddedSIMActivationCode 资源类型
description: 移动运营商提供的嵌入的 SIM 激活代码。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea17bc01e37b8e44f3fc904918f76859a9fcb40f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288465"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="98ace-103">embeddedSIMActivationCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="98ace-103">embeddedSIMActivationCode resource type</span></span>

<span data-ttu-id="98ace-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98ace-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98ace-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98ace-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98ace-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98ace-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98ace-107">移动运营商提供的嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="98ace-107">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="98ace-108">属性</span><span class="sxs-lookup"><span data-stu-id="98ace-108">Properties</span></span>
|<span data-ttu-id="98ace-109">属性</span><span class="sxs-lookup"><span data-stu-id="98ace-109">Property</span></span>|<span data-ttu-id="98ace-110">类型</span><span class="sxs-lookup"><span data-stu-id="98ace-110">Type</span></span>|<span data-ttu-id="98ace-111">Description</span><span class="sxs-lookup"><span data-stu-id="98ace-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98ace-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="98ace-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="98ace-113">字符串</span><span class="sxs-lookup"><span data-stu-id="98ace-113">String</span></span>|<span data-ttu-id="98ace-114">由移动运营商提供的嵌入的 SIM 激活代码 (ICCID) 的集成电路卡标识符。</span><span class="sxs-lookup"><span data-stu-id="98ace-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="98ace-115">输入必须与以下正则表达式匹配： ' ^ \[ 0-9 \] {19} \[ 0-9 \] ？ $ '。</span><span class="sxs-lookup"><span data-stu-id="98ace-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="98ace-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="98ace-116">matchingIdentifier</span></span>|<span data-ttu-id="98ace-117">字符串</span><span class="sxs-lookup"><span data-stu-id="98ace-117">String</span></span>|<span data-ttu-id="98ace-118">MatchingIdentifier (MatchingID) 在 GSMA Association SGP RSP 技术规范部分中指定4.1。</span><span class="sxs-lookup"><span data-stu-id="98ace-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="98ace-119">输入必须与以下正则表达式匹配： ' ^ \[ Z0-9 \- \] \* $ '。</span><span class="sxs-lookup"><span data-stu-id="98ace-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="98ace-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="98ace-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="98ace-121">字符串</span><span class="sxs-lookup"><span data-stu-id="98ace-121">String</span></span>|<span data-ttu-id="98ace-122">在 GSM 关联 SPG .22 RSP 技术规范中指定的 SM + 服务器的完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="98ace-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="98ace-123">输入必须与以下正则表达式匹配： "^ (\[ Z0-9 \] + (- \[ Z0 \] +) \* \.) + \[ a za-Z \] {2,} $"。</span><span class="sxs-lookup"><span data-stu-id="98ace-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98ace-124">关系</span><span class="sxs-lookup"><span data-stu-id="98ace-124">Relationships</span></span>
<span data-ttu-id="98ace-125">无</span><span class="sxs-lookup"><span data-stu-id="98ace-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98ace-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98ace-126">JSON Representation</span></span>
<span data-ttu-id="98ace-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98ace-127">Here is a JSON representation of the resource.</span></span>
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




