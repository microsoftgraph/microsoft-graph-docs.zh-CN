---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dfe20e52ad63cf1d0d6a958f2ef5f4f89a53ad6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260695"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="a99f1-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="a99f1-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="a99f1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a99f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a99f1-105">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="a99f1-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="a99f1-106">属性</span><span class="sxs-lookup"><span data-stu-id="a99f1-106">Properties</span></span>
|<span data-ttu-id="a99f1-107">属性</span><span class="sxs-lookup"><span data-stu-id="a99f1-107">Property</span></span>|<span data-ttu-id="a99f1-108">类型</span><span class="sxs-lookup"><span data-stu-id="a99f1-108">Type</span></span>|<span data-ttu-id="a99f1-109">说明</span><span class="sxs-lookup"><span data-stu-id="a99f1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a99f1-110">address</span><span class="sxs-lookup"><span data-stu-id="a99f1-110">address</span></span>|<span data-ttu-id="a99f1-111">String</span><span class="sxs-lookup"><span data-stu-id="a99f1-111">String</span></span>|<span data-ttu-id="a99f1-112">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="a99f1-112">Address to the proxy server.</span></span> <span data-ttu-id="a99f1-113">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="a99f1-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="a99f1-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="a99f1-114">exceptions</span></span>|<span data-ttu-id="a99f1-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="a99f1-115">String collection</span></span>|<span data-ttu-id="a99f1-116">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="a99f1-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="a99f1-117">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="a99f1-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="a99f1-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="a99f1-118">useForLocalAddresses</span></span>|<span data-ttu-id="a99f1-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="a99f1-119">Boolean</span></span>|<span data-ttu-id="a99f1-120">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="a99f1-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a99f1-121">关系</span><span class="sxs-lookup"><span data-stu-id="a99f1-121">Relationships</span></span>
<span data-ttu-id="a99f1-122">无</span><span class="sxs-lookup"><span data-stu-id="a99f1-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a99f1-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a99f1-123">JSON Representation</span></span>
<span data-ttu-id="a99f1-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a99f1-124">Here is a JSON representation of the resource.</span></span>
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



