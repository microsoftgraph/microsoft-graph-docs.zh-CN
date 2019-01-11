---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dcdb371ddcf7887fee8169eb29bbd856e5b8ab2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806165"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="fec04-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="fec04-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="fec04-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fec04-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fec04-105">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="fec04-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="fec04-106">属性</span><span class="sxs-lookup"><span data-stu-id="fec04-106">Properties</span></span>
|<span data-ttu-id="fec04-107">属性</span><span class="sxs-lookup"><span data-stu-id="fec04-107">Property</span></span>|<span data-ttu-id="fec04-108">类型</span><span class="sxs-lookup"><span data-stu-id="fec04-108">Type</span></span>|<span data-ttu-id="fec04-109">说明</span><span class="sxs-lookup"><span data-stu-id="fec04-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fec04-110">address</span><span class="sxs-lookup"><span data-stu-id="fec04-110">address</span></span>|<span data-ttu-id="fec04-111">String</span><span class="sxs-lookup"><span data-stu-id="fec04-111">String</span></span>|<span data-ttu-id="fec04-112">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="fec04-112">Address to the proxy server.</span></span> <span data-ttu-id="fec04-113">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="fec04-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="fec04-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="fec04-114">exceptions</span></span>|<span data-ttu-id="fec04-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="fec04-115">String collection</span></span>|<span data-ttu-id="fec04-116">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="fec04-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="fec04-117">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="fec04-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="fec04-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="fec04-118">useForLocalAddresses</span></span>|<span data-ttu-id="fec04-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="fec04-119">Boolean</span></span>|<span data-ttu-id="fec04-120">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="fec04-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fec04-121">关系</span><span class="sxs-lookup"><span data-stu-id="fec04-121">Relationships</span></span>
<span data-ttu-id="fec04-122">无</span><span class="sxs-lookup"><span data-stu-id="fec04-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fec04-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fec04-123">JSON Representation</span></span>
<span data-ttu-id="fec04-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fec04-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



