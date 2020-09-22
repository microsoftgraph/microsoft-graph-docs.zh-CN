---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58fd5fb0e46b7458cf9c96c4f1b5d541ba60bf3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091577"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="e5862-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5862-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="e5862-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5862-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5862-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5862-106">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="e5862-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e5862-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5862-107">Properties</span></span>
|<span data-ttu-id="e5862-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5862-108">Property</span></span>|<span data-ttu-id="e5862-109">类型</span><span class="sxs-lookup"><span data-stu-id="e5862-109">Type</span></span>|<span data-ttu-id="e5862-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5862-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5862-111">address</span><span class="sxs-lookup"><span data-stu-id="e5862-111">address</span></span>|<span data-ttu-id="e5862-112">String</span><span class="sxs-lookup"><span data-stu-id="e5862-112">String</span></span>|<span data-ttu-id="e5862-113">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="e5862-113">Address to the proxy server.</span></span> <span data-ttu-id="e5862-114">以以下格式指定地址 \<server\> \[ ：\<port\>\]</span><span class="sxs-lookup"><span data-stu-id="e5862-114">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="e5862-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="e5862-115">exceptions</span></span>|<span data-ttu-id="e5862-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="e5862-116">String collection</span></span>|<span data-ttu-id="e5862-117">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="e5862-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="e5862-118">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="e5862-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="e5862-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="e5862-119">useForLocalAddresses</span></span>|<span data-ttu-id="e5862-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5862-120">Boolean</span></span>|<span data-ttu-id="e5862-121">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="e5862-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5862-122">关系</span><span class="sxs-lookup"><span data-stu-id="e5862-122">Relationships</span></span>
<span data-ttu-id="e5862-123">无</span><span class="sxs-lookup"><span data-stu-id="e5862-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5862-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5862-124">JSON Representation</span></span>
<span data-ttu-id="e5862-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5862-125">Here is a JSON representation of the resource.</span></span>
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









