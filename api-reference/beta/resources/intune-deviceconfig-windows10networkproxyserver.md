---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56c4b4bd526c69bf9992673aa8ae93d723a2d9bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456951"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="96981-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="96981-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="96981-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96981-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96981-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96981-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96981-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96981-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96981-107">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="96981-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="96981-108">属性</span><span class="sxs-lookup"><span data-stu-id="96981-108">Properties</span></span>
|<span data-ttu-id="96981-109">属性</span><span class="sxs-lookup"><span data-stu-id="96981-109">Property</span></span>|<span data-ttu-id="96981-110">类型</span><span class="sxs-lookup"><span data-stu-id="96981-110">Type</span></span>|<span data-ttu-id="96981-111">说明</span><span class="sxs-lookup"><span data-stu-id="96981-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96981-112">address</span><span class="sxs-lookup"><span data-stu-id="96981-112">address</span></span>|<span data-ttu-id="96981-113">String</span><span class="sxs-lookup"><span data-stu-id="96981-113">String</span></span>|<span data-ttu-id="96981-114">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="96981-114">Address to the proxy server.</span></span> <span data-ttu-id="96981-115">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="96981-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="96981-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="96981-116">exceptions</span></span>|<span data-ttu-id="96981-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="96981-117">String collection</span></span>|<span data-ttu-id="96981-118">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="96981-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="96981-119">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="96981-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="96981-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="96981-120">useForLocalAddresses</span></span>|<span data-ttu-id="96981-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="96981-121">Boolean</span></span>|<span data-ttu-id="96981-122">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="96981-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96981-123">关系</span><span class="sxs-lookup"><span data-stu-id="96981-123">Relationships</span></span>
<span data-ttu-id="96981-124">无</span><span class="sxs-lookup"><span data-stu-id="96981-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96981-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96981-125">JSON Representation</span></span>
<span data-ttu-id="96981-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96981-126">Here is a JSON representation of the resource.</span></span>
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



