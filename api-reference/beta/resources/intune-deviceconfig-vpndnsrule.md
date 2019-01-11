---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d09e26b105a139f04db34ba69184fcf60e9ef238
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868199"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="88444-103">vpnDnsRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="88444-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="88444-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88444-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88444-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88444-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88444-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88444-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88444-107">VPN DNS 规则定义。</span><span class="sxs-lookup"><span data-stu-id="88444-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="88444-108">属性</span><span class="sxs-lookup"><span data-stu-id="88444-108">Properties</span></span>
|<span data-ttu-id="88444-109">属性</span><span class="sxs-lookup"><span data-stu-id="88444-109">Property</span></span>|<span data-ttu-id="88444-110">类型</span><span class="sxs-lookup"><span data-stu-id="88444-110">Type</span></span>|<span data-ttu-id="88444-111">说明</span><span class="sxs-lookup"><span data-stu-id="88444-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88444-112">name</span><span class="sxs-lookup"><span data-stu-id="88444-112">name</span></span>|<span data-ttu-id="88444-113">字符串</span><span class="sxs-lookup"><span data-stu-id="88444-113">String</span></span>|<span data-ttu-id="88444-114">名称。</span><span class="sxs-lookup"><span data-stu-id="88444-114">Name.</span></span>|
|<span data-ttu-id="88444-115">服务器</span><span class="sxs-lookup"><span data-stu-id="88444-115">servers</span></span>|<span data-ttu-id="88444-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="88444-116">String collection</span></span>|<span data-ttu-id="88444-117">服务器。</span><span class="sxs-lookup"><span data-stu-id="88444-117">Servers.</span></span>|
|<span data-ttu-id="88444-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="88444-118">proxyServerUri</span></span>|<span data-ttu-id="88444-119">字符串</span><span class="sxs-lookup"><span data-stu-id="88444-119">String</span></span>|<span data-ttu-id="88444-120">代理服务器 Uri。</span><span class="sxs-lookup"><span data-stu-id="88444-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88444-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="88444-121">Relationships</span></span>
<span data-ttu-id="88444-122">无</span><span class="sxs-lookup"><span data-stu-id="88444-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88444-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88444-123">JSON Representation</span></span>
<span data-ttu-id="88444-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88444-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String"
}
```





