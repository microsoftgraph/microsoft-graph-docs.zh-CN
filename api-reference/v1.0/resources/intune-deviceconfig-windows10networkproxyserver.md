---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88cf36813a6ed7102807917caf0bca3e46744f5f
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748460"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="e8179-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8179-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="e8179-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8179-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8179-105">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="e8179-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e8179-106">属性</span><span class="sxs-lookup"><span data-stu-id="e8179-106">Properties</span></span>
|<span data-ttu-id="e8179-107">属性</span><span class="sxs-lookup"><span data-stu-id="e8179-107">Property</span></span>|<span data-ttu-id="e8179-108">类型</span><span class="sxs-lookup"><span data-stu-id="e8179-108">Type</span></span>|<span data-ttu-id="e8179-109">说明</span><span class="sxs-lookup"><span data-stu-id="e8179-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8179-110">address</span><span class="sxs-lookup"><span data-stu-id="e8179-110">address</span></span>|<span data-ttu-id="e8179-111">String</span><span class="sxs-lookup"><span data-stu-id="e8179-111">String</span></span>|<span data-ttu-id="e8179-112">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="e8179-112">Address to the proxy server.</span></span> <span data-ttu-id="e8179-113">在 "\>\[服务器：\<端口" \<格式中指定地址\>\]</span><span class="sxs-lookup"><span data-stu-id="e8179-113">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="e8179-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="e8179-114">exceptions</span></span>|<span data-ttu-id="e8179-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="e8179-115">String collection</span></span>|<span data-ttu-id="e8179-116">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="e8179-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="e8179-117">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="e8179-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="e8179-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="e8179-118">useForLocalAddresses</span></span>|<span data-ttu-id="e8179-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8179-119">Boolean</span></span>|<span data-ttu-id="e8179-120">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="e8179-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8179-121">关系</span><span class="sxs-lookup"><span data-stu-id="e8179-121">Relationships</span></span>
<span data-ttu-id="e8179-122">无</span><span class="sxs-lookup"><span data-stu-id="e8179-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8179-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8179-123">JSON Representation</span></span>
<span data-ttu-id="e8179-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8179-124">Here is a JSON representation of the resource.</span></span>
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




