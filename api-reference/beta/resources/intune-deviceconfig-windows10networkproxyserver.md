---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32cf4d75b6d030ea40459447abc2e37d9257870a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729629"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="c429f-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="c429f-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="c429f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c429f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c429f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c429f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c429f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c429f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c429f-107">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="c429f-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="c429f-108">属性</span><span class="sxs-lookup"><span data-stu-id="c429f-108">Properties</span></span>
|<span data-ttu-id="c429f-109">属性</span><span class="sxs-lookup"><span data-stu-id="c429f-109">Property</span></span>|<span data-ttu-id="c429f-110">类型</span><span class="sxs-lookup"><span data-stu-id="c429f-110">Type</span></span>|<span data-ttu-id="c429f-111">说明</span><span class="sxs-lookup"><span data-stu-id="c429f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c429f-112">address</span><span class="sxs-lookup"><span data-stu-id="c429f-112">address</span></span>|<span data-ttu-id="c429f-113">String</span><span class="sxs-lookup"><span data-stu-id="c429f-113">String</span></span>|<span data-ttu-id="c429f-114">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="c429f-114">Address to the proxy server.</span></span> <span data-ttu-id="c429f-115">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="c429f-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="c429f-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="c429f-116">exceptions</span></span>|<span data-ttu-id="c429f-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="c429f-117">String collection</span></span>|<span data-ttu-id="c429f-118">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="c429f-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="c429f-119">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="c429f-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="c429f-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="c429f-120">useForLocalAddresses</span></span>|<span data-ttu-id="c429f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c429f-121">Boolean</span></span>|<span data-ttu-id="c429f-122">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="c429f-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c429f-123">关系</span><span class="sxs-lookup"><span data-stu-id="c429f-123">Relationships</span></span>
<span data-ttu-id="c429f-124">无</span><span class="sxs-lookup"><span data-stu-id="c429f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c429f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c429f-125">JSON Representation</span></span>
<span data-ttu-id="c429f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c429f-126">Here is a JSON representation of the resource.</span></span>
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





